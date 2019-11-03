~~~
 $ sudo vi /etc/wpa_supplicant/wpa_supplicant.conf

    ctrl_interface=DIR=/var/run/wpa_supplicant GROUP=netdev
    update_config=1
    country=GB
    network={
            ssid="무선네트워크SSID"
            psk="패스워드"
    }
~~~

2. 와이파이 네트워크 인터페이스 내렸다 올리기
~~~
    $ sudo ifconfig wlan0 down
    $ sudo ifconfig wlan0 up
~~~
참고 : [https://www.withover.com/2018/08/wifi.html](https://www.withover.com/2018/08/wifi.html)
