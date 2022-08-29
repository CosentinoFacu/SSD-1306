'''
Programa: Test de pantalla SSD1306

Proposito: Verificar funcionamento
de pantalla oled

Programadores: Facundo Cosentino, Sergio Zelaya
Fecha: 21/08/2022
'''
#Importamos Pin e I2C de machine 
from machine import Pin, I2C
#Importamos ssd1306
import ssd1306

import time

#Configuramos comunicacion I2C 
i2c = I2C(0,sda=Pin(21), scl=Pin(22),freq=400000)

#Configuramos pantalla ssd1306
display = ssd1306.SSD1306_I2C(128, 32, i2c)

#Mostramos mensaje
display.fill(0)
display.fill_rect(0, 0, 32, 32, 1)
display.fill_rect(2, 2, 28, 28, 0)
display.vline(9, 8, 22, 1)
display.vline(16, 2, 22, 1)
display.vline(23, 8, 22, 1)
display.fill_rect(26, 24, 2, 4, 1)
display.text('MicroPython', 40, 0, 1)
display.text('SSD1306', 40, 12, 1)
display.text('OLED 128x32', 40, 24, 1)
display.show()
