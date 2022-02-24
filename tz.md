1) В классе должны быть реализованы функции включения, отключения, установки яркости и инициализации светодидода.

> class Led{
>   
>void Led(int pin, bool inverted=false);
>
> void init();
> 
>void on();
> 
> void off();
> 
> void set_brightness(int new_br);
> 
>
>};
 

2) пример использования класса:

2.1.
Создание экземпляра класса:
> Led mySweetLed(13); 

2.2. 
Инициализация:
> mySweetLed.init(); 

2.3. 
установка яркости:
> mySweetLed.set_brightness( 127 );

2.4.
включение\отключение:
> mySweetLed.on()
> 
> mySweetLed.off()