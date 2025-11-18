from pyb import Timer, Pin

timmer = pyb.Timer(5, freq=500)
rouge = timmer.channel(3, Timer.PWM, pin=Pin('X1'), pulse_width_percent=39)
vert = timmer.channel(4, Timer.PWM, pin=Pin('X2'), pulse_width_percent=12)
bleu = timmer.channel(1, Timer.PWM, pin=Pin('X3'), pulse_width_percent=87)
