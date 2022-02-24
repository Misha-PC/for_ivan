1) В классе должны быть реализованы функции включения, отключения, установки яркости и инициализации светодиода.

```cpp
class Led{
private:
    int pin;
    int brightness;
    bool state;
    bool inverted;
    
public:
    void Led(int pin, bool inverted=false);
    void init();
    void on();
    void off();
    void set_brightness(int new_br);
};
```


2) пример использования класса:

2.1.
Создание экземпляра класса:
```cpp
    Led mySweetLed(13); 
```
2.2. 
Инициализация:
```cpp
    mySweetLed.init(); 
```
2.3. 
установка яркости:
```cpp
    mySweetLed.set_brightness( 127 );
```
2.4.
включение\отключение:
```cpp
    mySweetLed.on()
    mySweetLed.off()
```