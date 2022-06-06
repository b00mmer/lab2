# Лабораторная работа №2
 Настройка административных ролей
 
1.	Топология

![alt-текст][Топология]

[Топология]:https://github.com/b00mmer/lab2/blob/main/%D0%A2%D0%BE%D0%BF%D0%BE%D0%BB%D0%BE%D0%B3%D0%B8%D1%8F.JPG "Топология"

2. Таблица адресации

![alt-текст][Таблица]

[Таблица]:https://github.com/b00mmer/lab2/blob/main/%D0%A2%D0%B0%D0%B1%D0%BB%D0%B8%D1%86%D0%B0%20%D0%B0%D0%B4%D1%80%D0%B5%D1%81%D0%B0%D1%86%D0%B8%D0%B8.JPG "Таблица адресации"

## Часть 1: Настройка основных параметров устройства

1. [Сетевые параметры маршрутизатора R1](https://github.com/b00mmer/lab2/blob/main/R1_running-config.txt)
2. [Сетевые параметры маршрутизатора R2](https://github.com/b00mmer/lab2/blob/main/R2_running-config.txt)
3. [Сетевые параметры маршрутизатора R3](https://github.com/b00mmer/lab2/blob/main/R3_running-config.txt)
4. Сетевые параметры Server 0

![alt-текст][Server0]

[Server0]:https://github.com/b00mmer/lab2/blob/main/Server0.JPG "Сетевые параметры Server 0"
5. Сетевые параметры Server 0

![alt-текст][PC0]

[PC0]:https://github.com/b00mmer/lab2/blob/main/PC-0.JPG "Сетевые параметры PC0"

6.  Проверьте связь между Server0 и PC0.

__ C:\>ping 192.168.1.3

Pinging 192.168.1.3 with 32 bytes of data:

Reply from 192.168.1.3: bytes=32 time<1ms TTL=125

Reply from 192.168.1.3: bytes=32 time=1ms TTL=125

Reply from 192.168.1.3: bytes=32 time=10ms TTL=125

Reply from 192.168.1.3: bytes=32 time=10ms TTL=125

Ping statistics for 192.168.1.3:

Packets: Sent = 4, Received = 4, Lost = 0 (0% loss),

Approximate round trip times in milli-seconds:

Minimum = 0ms, Maximum = 10ms, Average = 5ms
	
C:\>tracert 192.168.1.3

Tracing route to 192.168.1.3 over a maximum of 30 hops: 

  1   0 ms      0 ms      0 ms      192.168.3.1

  2   1 ms      1 ms      0 ms      10.2.2.2
  
  3   0 ms      0 ms      0 ms      10.1.1.1
  
  4   0 ms      0 ms      13 ms     192.168.1.3

Trace complete.

 Server0 -> PC0

Cisco Packet Tracer SERVER Command Line 1.0

C:\>tracert 192.168.3.3

Tracing route to 192.168.3.3 over a maximum of 30 hops: 

  1   0 ms      0 ms      0 ms      192.168.1.1
  2   0 ms      0 ms      0 ms      10.1.1.2
  3   0 ms      0 ms      0 ms      10.2.2.1
  4   0 ms      10 ms     11 ms     192.168.3.3

Trace complete.


C:\>ping 192.168.3.3

Pinging 192.168.3.3 with 32 bytes of data:

Reply from 192.168.3.3: bytes=32 time<1ms TTL=125

Reply from 192.168.3.3: bytes=32 time=1ms TTL=125

Reply from 192.168.3.3: bytes=32 time=17ms TTL=125

Reply from 192.168.3.3: bytes=32 time=10ms TTL=125

Ping statistics for 192.168.3.3:

Packets: Sent = 4, Received = 4, Lost = 0 (0% loss),

Approximate round trip times in milli-seconds:

Minimum = 0ms, Maximum = 17ms, Average = 7ms __

## Часть 2: Настройка административных ролей

1. [Сетевые параметры маршрутизатора R1](https://github.com/b00mmer/lab2/blob/main/R1_running-config_1.txt)
2. [Сетевые параметры маршрутизатора R3](https://github.com/b00mmer/lab2/blob/main/R3_running-config_1.txt)





