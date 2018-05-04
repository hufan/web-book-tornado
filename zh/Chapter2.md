# 2. web 的使用


-  1 . 使用前的准备
    - 接入以太网，web只能在局域网内打开使用

-  2 . web登录方式

    -  登录用户名和密码默认都是admin
    -  开发板上电后串口会打印web的log，log如下:
    ```
    Development server is running at http://192.168.30.121:8090/login
    ```
 &nbsp; &nbsp;&nbsp;&nbsp; &nbsp;
 在浏览器中输入 ``` http://192.168.30.121:8090/login ```(IP根据实际情况修改)，就可以看到登录界面
- 3 .  web 语言版本
    - web 界面提供了两种语言，中文和英文版本，默认的是英文版本。在界面的右上角有切换语言的按钮
    - 切换语言时会自动关闭以前打开的设备
- 4 .  同步处理
    - web demo和qt demo做了同步处理，qt端和web端可以同时打开同一个设备，但是设备的参数使用的是同一份。如qt端先打开RS232设备，web再次打开时则会读取qt端设置的参数来说使用，反之依然，如接到数据qt端和web端可以同时接受到数据并显示。RS232、RS485、CAN都有同样的处理
    - RS485、RS232界面的数据显示的是字符串格式

- 5 .  模块测试说明
   - LED
        - 在页面上会动态的读取开发板上LED的个数和状态并显示出来，也可在页面控制LED的亮灭

        - 界面如下：
        ![image](https://note.youdao.com/yws/api/personal/file/WEBbaa75739ab9c9d3a598dce8d86bf93c9?method=download&shareKey=505824325fa17c8de6c57a404fd4c70e)

    - RS232
        - 在页面可以测试开发板的RS232设备。先配置好参数，再打开设备，就可以测试收发数据了
        - 修改配置参数时会先关闭设备，需要再次打开

        - 界面如下：
        ![image](https://note.youdao.com/yws/api/personal/file/WEB6ab944d4d912edd3bd37990b0cae9197?method=download&shareKey=55e49e24feed774d994ff6415ad0f442)

    - RS485
        - 在页面可以测试开发板的RS485设备,先配置好参数，再打开设备，然后就可以收发数据了。修改配置参数时会先关闭设备，需要再次打开

        - 界面如下：        ![image](https://note.youdao.com/yws/api/personal/file/WEB5d074e5be690498c234605605218c76e?method=download&shareKey=b490052c8de7c0b057e24e2576548727)

    - CAN
        - 在页面可以测试开发板的CAN设备,先配置好参数，再打开设备，然后就可以收发数据了。注修改配置参数时会先关闭设备，需要再次打开
        - 界面如下 ![image](https://note.youdao.com/yws/api/personal/file/WEBe14f89943f31064fccfe54a7770d9b98?method=download&shareKey=c0cadfc921088cfb9d1e4661706bec70)

    - 网卡
        - 在页面可以实时的显示网卡状态，也可以修改设置网卡。  修改IP时需要注意，如果修改的是web server使用的网卡，会有提示窗口，确认修改后会修改开发板Ip，web 服务断开，开发板重启。

        - 界面如下：        ![image](https://note.youdao.com/yws/api/personal/file/WEBa4e1cc19251cc7190c30d85d844dae68?method=download&shareKey=071b840ee40086105c24b5e394e9134e)
    - 联系
        - 页面中提供了我司的地址和联系方式等信息。
        - 界面如下：
        ![image](https://note.youdao.com/yws/api/personal/file/WEB89559ee52c886116027a83f34d30a3dd?method=download&shareKey=cc33e5205dd01f74f2d35cd7dfa90f51)




