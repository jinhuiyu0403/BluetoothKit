# 待办
去了facebook如果工作涉及到蓝牙的，就好好优化一下这个框架，做成世界上最好用的蓝牙框架

1，去掉service，纯粹的蓝牙通信框架，这样gatt也能回调，但是要避免close了外面还操作
2，增加对新接口的支持，包括扫描，mesh?
3，任务队列抽出来
4，多设备连接管理，活跃度监测，LRUCache队列
5，完善demo，增加分包发送
6，增加GattServer部分
7，Log的问题，增加开关，release版里不要带上日志
8，支持普通蓝牙连接
9，兼容性问题，比如高sdk版本接口
10，失败的提示，以打印出异常栈的形式，动态代理异常的就直接抛出，不要catch住
11，错误不要用constant int，别人在日志里看不懂
12，读写的时候失败，如果是没打开属性，就只打印warning，别直接失败。或者如果UUID不对，就提示
13，动态权限申请
14，支持广播的xml配置，动态生成解析类
15，支持notify打开失败的workaround
16，支持断线重连
17，支持classic蓝牙的连接

比如UUID不对，

参考别的开源框架，吸取精华，包括看有什么功能要完善的
看Issues里大家提出的问题