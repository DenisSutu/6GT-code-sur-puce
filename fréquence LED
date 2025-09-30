from pyb import Timer, Pin

timmer = pyb.Timer(5, freq=500)

channel = timmer.channel(3, Timer.PWM, pin=Pin('X1'), pulse_width_percent=100)
#channel.pulse_width_percent(100)

def dimm_high(duration):
    for i in range (100):
        channel.pulse_width_percent(i)
        pyb.delay(duration*10)

def dimm_low(duration):
    for i in range (100):
        channel.pulse_width_percent(100-i)
        pyb.delay(duration*10)
        
while True:
    dimm_high(10)
    dimm_low(15)
