# iot

BME280 test code:
  import bme280
  import smbus2
  from time import sleep
  
  port = 1
  address = 0x77
  bus = smbus2.SMBus(port)
  
  bme280.load_calibration_params(bus, address)
  
  def get bme280data:
    bme280_data = bme280.sample(bus, address)
    print("temperature: %0.2f C" % (bme280_data.temperature),
          “humidity: %0.2f %% " % (bme280_data.humidity),
          "pressure: %0.2f Pa" % (bme280_data.pressure))
    sleep(10)
