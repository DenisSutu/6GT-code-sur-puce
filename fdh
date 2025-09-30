from pyb import Timer, Pin
pot=pyb.ADC('X19')
timmer = pyb.Timer(5, freq=500)
channel = timmer.channel(3, Timer.PWM, pin=Pin('X1'), pulse_width_percent=100)

while True: 
   val_pot=pot.read()
   print(val_pot)
   intensity=(val_pot/4095)*100
   channel.pulse_width_percent(intensity)
   pyb.delay(100)
