# Packet Tracer - Implement a Small Network

## Addressing Table

<table class="Address">
  <tr>
    <th class="tg-yw4l"><b>Device</b></th>
    <th class="tg-yw4l"><b>Interface</b></th>
    <th class="tg-yw4l"><b>Address</b></th>
    <th class="tg-yw4l"><b>Subnet Mask</b></th>
    <th class="tg-yw4l"><b>Default Gateway</b></th>
  </tr>
  <tr>
    <td class="tg-yw4l" rowspan="2">RTA</td>
    <td class="tg-yw4l">G0/0</td>
    <td class="tg-yw4l">10.10.10.1</td>
    <td class="tg-yw4l">255.255.255.0</td>
    <td class="tg-yw4l">N/A</td>
  </tr>
  <tr>
    <td class="tg-yw4l">G0/1</td>
    <td class="tg-yw4l">10.10.20.1</td>
    <td class="tg-yw4l">255.255.255.0</td>
    <td class="tg-yw4l">N/A</td>
  </tr>
   <tr>
    <td class="tg-yw4l">SW1</td>
    <td class="tg-yw4l">VLAN</td>
    <td class="tg-yw4l">10.10.10.2</td>
    <td class="tg-yw4l">255.255.255.0</td>
    <td class="tg-yw4l"></td>
  </tr>
  <tr>
    <td class="tg-yw4l">SW2</td>
    <td class="tg-yw4l">VLAN</td>
    <td class="tg-yw4l">10.10.20.2</td>
    <td class="tg-yw4l">255.255.255.0</td>
    <td class="tg-yw4l"></td>
  </tr>
  <tr>
    <td class="tg-yw4l">PC-1</td>
    <td class="tg-yw4l">NIC</td>
    <td class="tg-yw4l"></td>
    <td class="tg-yw4l">255.255.255.0</td>
    <td class="tg-yw4l"></td>
  </tr>
  <tr>
    <td class="tg-yw4l">PC-2</td>
    <td class="tg-yw4l">NIC</td>
    <td class="tg-yw4l"></td>
    <td class="tg-yw4l">255.255.255.0</td>
    <td class="tg-yw4l"></td>
  </tr>
</table>

## Objectives
    -   Part 1: Create the Network Topology
    -   Part 2: Configure Devices and Verify Connectivity

## Instructions

### Part 1: Create the Network Topology
    -   Part 1: Create the Network Topology
        -   Step 1: Obtain the required devices.
            - Click the Network Devices icon in the bottom tool bar.
            - Click the router icon in the submenu.
            - Locate the 1941 router icon. Click and drag the icon for the 1941 router into the topology area.
            - Click the switch entry in the submenu.
            - Locate the 2960 switch icon. Click and drag the icon for the 2960 switch into the topology area.
            - Repeat the step above so that there are two 2960 switches in the topology area.
            - Click the End Devices icon.
            - Locate the PC icon. Drag two PCs to the topology area.
            - Arrange the devices into a layout that you can work with by clicking and dragging.
    - Step 2: Name the devices.
        -   The devices have default names that you will need to change. You will name the devices as shown in the Addressing Table. You are changing the display names of the devices. This is the text label that appears below each device. Your display names must match the information in the Addressing Table exactly. If a display name does not match, you will not be scored for your device configuration.
            - Click the device display name that is below the device icon. A text field should appear with a flashing insertion point. If the configuration window for the device appears, close it and try again, clicking a little further away from the device icon.
            - Replace the current display name with the appropriate display name from the Addressing Table.
            - Repeat until all devices are named.
    - Step 3: Connect the devices.
        -   Click the orange lightning bolt connections icon in the bottom toolbar.
        -   Locate the Copper Straight-Through cable icon. It looks like a solid black diagonal line.
        -   To connect the device, click the Copper Straight-Through cable icon and then click the first device that you want to connect. Select the correct port and then click the second device. Select the correct port and the devices will be connected.
        -   Connect the devices as specified in the table below.

<table class="Address">
  <tr>
    <th class="tg-yw4l"><b>From Device</b></th>
    <th class="tg-yw4l"><b>Port</b></th>
    <th class="tg-yw4l"><b>To Device</b></th>
    <th class="tg-yw4l"><b>Port</b></th>
  </tr>
  <tr>
    <td class="tg-yw4l" rowspan="2">RTA</td>
    <td class="tg-yw4l">G0/0</td>
    <td class="tg-yw4l">SW1</td>
    <td class="tg-yw4l">G0/1</td>
  </tr>
  <tr>
    <td class="tg-yw4l">G0/1</td>
    <td class="tg-yw4l">SW2</td>
    <td class="tg-yw4l">G0/1</td>

  </tr>
   <tr>
    <td class="tg-yw4l">SW1</td>
    <td class="tg-yw4l">F0/1</td>
    <td class="tg-yw4l">PC-1</td>
    <td class="tg-yw4l">FastEthernet0</td>
  </tr>
  <tr>
    <td class="tg-yw4l">SW2</td>
    <td class="tg-yw4l">F0/1</td>
    <td class="tg-yw4l">PC-2</td>
    <td class="tg-yw4l">FastEthernet0</td>
  </tr>
</table>

```bash
ตามขั้นตอนก็
1. กดที่ Router เลือก Router 1941 ลากออกมาที่หน้าต่าง 1 ตัว
2. กดที่ Switch เลือก Switch 2960 ลากออกมาที่หน้าต่าง 2 ตัว
3. กดที่ PC และลาก PC ออกมาที่หน้าต่าง 2 ตัว
4. ตั้งชื่อ Router ใหม่โดยคลิกที่ Router0 และแก้ชื่อให้เป็น RTA
5. ตั้งชื่อ Switch ใหม่โดยคลิกที่ชื่อ Switch0 และ Switch1 แก้เป็น SW1 และ SW2
6. ตั้งชื่อ PC ทั้งสองเครื่องใหม่เป็น PC-1 และ PC-2 
7. กดที่รูปสายฟ้าไปเลือก Copper Straight-Through 
    7.1 ต่อสายจาก RTA(Router) ช่อง GigabitEthernet0/0 ไปที่ SW1(Switch 1) ช่อง GigabitEthernet0/1
    7.2 ต่อสายจาก RTA(Router) ช่อง GigabitEthernet0/0 ไปที่ SW2(Switch 2) ช่อง GigabitEthernet0/1
    7.3 ต่อสายจาก SW1(Switch 1) ช่อง FastEthernet0/1 ไปที่ PC-1 ที่ช่อง FastEthernet0
    7.4 ต่อสายจาก SW2(Switch 2) ช่อง FastEthernet0/1 ไปที่ PC-2 ที่ช่อง FastEthernet0
```

![1](https://raw.githubusercontent.com/SunatP/ITCS391_Computer_Network_Lab/master/HW1/img/1.PNG)

### Part 2: Configure Devices

Record the PC addressing and gateway addresses in the addressing table. You can use any available address in the network for PC-1 and PC-2.

#### Step 1: Configure the router.
    a. Configure basic settings.
           1.Hostname as shown in the Addressing Table.
           2.Configure Ciscoenpa55 as the encrypted password.
           3.Configure Ciscolinepa55 as the password on the lines.
           4.All lines should accept connections. 
           5.Configure an appropriate message of the day banner.
    b. Configure interface settings.
           1.Addressing.
           2.Descriptions on the interfaces.
           3.Save your configuration.

#### Step 2: Configure switch SW1 and SW2.
    a.  Configure the default management interface so that it will accept connections over the network from local and remote hosts. Use the values in the addressing table.
    b.  Configure an encrypted password using the value in step 1a above.
    c.  Configure all lines to accept connections using the password from step 1a above.
    d.  Configure the switches so that they can send data to hosts on remote networks.
    e.  Save your configuration.

#### Step 3: Configure the hosts.
Configure addressing on the hosts. If your configurations are complete, you should be able to ping all devices in the topology.


#### ตั้งค่่า Router กันก่อน
มาว่ากันเรื่องของพาร์ทที่ 2 กันก่อนเราจะเริ่ม Setup ที่ Router กันก่อนเลย โดยดับเบิ้ลคลิกที่ RTA เพื่อตั้งค่า

```bash
         --- System Configuration Dialog ---

Would you like to enter the initial configuration dialog? [yes/no]: n

Press RETURN to get started!
```

ตรงนี้เราจะกด Enter เพื่อเริ่มทำการตั้งค่า

```bash
Router> # มันจะขึ้นแบบนี้มา
```

จากนั้นพิมพ์ **enable** แล้วกด enter
```bash
Router>enable 
```

จะได้แบบนี้

```C++
Router#     // ตอนแรกจะเป็น Router> แบบนี้
```
![2](https://raw.githubusercontent.com/SunatP/ITCS391_Computer_Network_Lab/master/HW1/img/2.PNG)

เราจะเริ่มทำการตั้งค่า ให้กับ Router ก่อนโดยใช้คำสั่งเปิด config t ก่อน

```C
Router#config t // แล้วกด enter จะได้แบบนี้
// แบบข้างล่างนี้
Enter configuration commands, one per line.  End with CNTL/Z.
Router(config)#
```

![3](https://raw.githubusercontent.com/SunatP/ITCS391_Computer_Network_Lab/master/HW1/img/3.PNG)

จากนั้นใช้คำสั่ง hostname RTA เพื่อตั้งชื่อ Router (RTA คือชื่อที่ทางแลปให้ตั้ง)

```C
Router(config)#hostname RTA
// จะได้แบบนี้
RTA(config)#
```

จะสังเกตได้ว่า Router(config) ได้เปลี่ยนเป็น RTA(config) เรียบร้อยแล้ว

![4](https://raw.githubusercontent.com/SunatP/ITCS391_Computer_Network_Lab/master/HW1/img/4.PNG)

ต่อมาเราจะตั้งรหัสผ่านให้กับตัว Router แบบ encrypt โดยรหัสผ่านนี้คือ **Ciscoenpa55** โดยวิธีตั้งคือ

```c
RTA(config)#enable secret Ciscoenpa55 // แล้วกด enter ไป router จะทำการจำรหัสผ่านไว้แล้ว
```

![5](https://raw.githubusercontent.com/SunatP/ITCS391_Computer_Network_Lab/master/HW1/img/5.PNG)

ต่อมาเราจะต้องตั้งรหัสผ่านสำหรับ line console เพื่อกันคนภายนอกเข้ามแก้ไขโดยใช้คำสั่งแบบนี้

```c
RTA(config)#line console 0 // แล้วกด enter จะได้แบบนี้
RTA(config-line)#
```

จากนั้นใช้คำสั่ง **password** ตามด้วยรหัสผ่านคือ **Ciscolinepa55** แล้วกด enter

```c
RTA(config-line)#password Ciscolinepa55
// จากนั้นใส่คำสั่ง login เข้าไปเพื่อเปิดการใช้รหัสผ่าน
RTA(config-line)#login
```

![6](https://raw.githubusercontent.com/SunatP/ITCS391_Computer_Network_Lab/master/HW1/img/6.PNG)

ระบบจะจดจำรหัสผ่านเรียบร้อย จากนั้นกด CTRL+Z เพื่อกลับไปหน้าหลักของ Router

```C
RTA(config-line)#^Z
RTA#
%SYS-5-CONFIG_I: Configured from console by console
RTA# 
```

![7](https://raw.githubusercontent.com/SunatP/ITCS391_Computer_Network_Lab/master/HW1/img/7.PNG)

ตรงนี้เราจะต้องตั้งค่า Banning หรือข้อความต้อนรับสำหรับผู้ที่เข้ามาตั้งค่าโดยใช้คำสั่ง

```C
RTA#config t
RTA(config)#banner motd ! // ตรงนี้จะเป็นการเปิดการตั้งค่า banner 
// กด Enter ไปจะได้แบบนี้
Enter TEXT message.  End with the character '!'.

## Welcome to Cisco Router ## // พิมพ์ประมาณนี้หรือแบบอื่นก็ได้แล้วกด enter
! // จากนั้นใช้เครื่องหมายตกใจหรืออัศเจรีย์แล้วกด Enter เพื่อจบการทำงาน
```

![8](https://raw.githubusercontent.com/SunatP/ITCS391_Computer_Network_Lab/master/HW1/img/8.PNG)

ต่อมาเราจะตั้งค่า Router ให้สามารถจ่าย IP Address ให้กับ GigabitEthernet port ทั้ง 2 โดยเริ่มที่ช่อง GigabitEthernet0/0 ก่อน โดยใช้คำสั่ง 
```c
RTA(config)#interface G0/0
RTA(config-if)#ip address 10.10.10.1 255.255.255.0
RTA(config-if)#no shutdown

RTA(config-if)#
%LINK-5-CHANGED: Interface GigabitEthernet0/0, changed state to up

%LINEPROTO-5-UPDOWN: Line protocol on Interface GigabitEthernet0/0, changed state to up

RTA(config-if)#

```

![9](https://raw.githubusercontent.com/SunatP/ITCS391_Computer_Network_Lab/master/HW1/img/9.PNG)

จากนั้นทำแบบนี้เช่นเดียวกับ GigabitEthernet0/1 แต่เปลี่ยน IP Address เป็น 10.10.20.1


```c
RTA(config)#interface G0/1
RTA(config-if)#ip address 10.10.20.1 255.255.255.0
RTA(config-if)#no shutdown

RTA(config-if)#
%LINK-5-CHANGED: Interface GigabitEthernet0/1, changed state to up

%LINEPROTO-5-UPDOWN: Line protocol on Interface GigabitEthernet0/1, changed state to up

RTA(config-if)#description GigabitLan // เราจะตั้งคำอธิบายให้ช่องG0/1
RTA(config-if)#exit
RTA(config)#interface G0/0
RTA(config-if)#description GigabitLan // เราจะตั้งคำอธิบายให้ช่องG0/0
RTA(config-if)#
```

![10](https://raw.githubusercontent.com/SunatP/ITCS391_Computer_Network_Lab/master/HW1/img/10.PNG)

จากนั้นเราจะทำการ backup configuration ของ Router ตัวนี้ไว้โดยใช้คำสั่ง


```C
RTA(config-if)#^Z // ตรงนี้กด CTRL + Z เพื่อออกมา
RTA#
%SYS-5-CONFIG_I: Configured from console by console

RTA#copy running-config startup-config // ใช้คำสั่งนี้เพื่อก๊อปปี้ไปเก็บไว้ จากนั้นกด enter
Destination filename [startup-config]?  // แล้วกด enter อีกที
Building configuration...
[OK]
RTA#
```

![11](https://raw.githubusercontent.com/SunatP/ITCS391_Computer_Network_Lab/master/HW1/img/11.PNG)

จากนั้นเราจะตั้งรหัสผ่านให้กับ VTY port อีกทีโดยใช้คำสั่ง
```c
RTA#conf t
RTA(config)#line vty 0 4
RTA(config-line)#password Ciscolinepa55
RTA(config-line)#login
RTA(config-line)#
```

![12](https://raw.githubusercontent.com/SunatP/ITCS391_Computer_Network_Lab/master/HW1/img/12.PNG)

จากนั้นกดปิดหน้าต่าง setup(CLI) ไปได้เลย

#### ต่อมาตั้งค่าที่ Switch ทั้งสอง

คลิกที่ SW1 หรือ SW2 ก็ได้แต่เราจะทำการ Setup ที่ SW1 ก่อนโดยทำแบบเดิมกับ Router เลย

```c
Switch>enable // ใช้คำสั่งเพื่อเปิดการตั้งค่า
Switch#
```

เราจะตั้งค่ารหัสผ่านกันก่อน

```c
Switch#conf t
Switch(config)#enable secret Ciscoenpa55
Switch(config)#line console 0
Switch(config-line)#password Ciscolinepa55
Switch(config-line)#login
Switch(config-line)#
```

![13](https://raw.githubusercontent.com/SunatP/ITCS391_Computer_Network_Lab/master/HW1/img/13.PNG)

จากนั้นกลับมาที่หน้าหลักโดยใช้ CTRL + Z 
```c
Switch(config-line)#^Z
Switch#
%SYS-5-CONFIG_I: Configured from console by console

Switch#
```
จากนั้นเราจะเริ่มตั้งค่า IP Address ให้กับ Switch กัน

```c
Switch#conf t
Switch(config)#interface vlan1
Switch(config-if)#ip address 10.10.10.2 255.255.255.0
Switch(config-if)#no shutdown
Switch(config-if)#exit
Switch(config)#ip default-gateway 10.10.10.1
Switch(config)#
```
ถ้าเป็น SW2 ก็แบบเดิมแค่เปลี่ยนบางอันเท่านั้นเป็นแบบนี้
```c
Switch#conf t
Switch(config)#interface vlan1
Switch(config-if)#ip address 10.10.20.2 255.255.255.0
Switch(config-if)#no shutdown
Switch(config-if)#exit
Switch(config)#ip default-gateway 10.10.20.1
Switch(config)#
```

จากนั้นเราจะตั้งรหัสผ่านให้กับ SW1 และ SW2 ผ่านช่อง VTY โดยใช้คำสั่ง
```c
Switch(config)#line vty 0 4
Switch(config-line)#password Ciscolinepa55
Switch(config-line)#
```

จากนั้นทำการ backup configuration โดยการใช้ CTRL + Z เพื่อออกมาที่หน้า Switch# 

```c
Switch(config-line)#^Z
Switch#
%SYS-5-CONFIG_I: Configured from console by console

Switch#copy running-config startup-config
Destination filename [startup-config]? 
Building configuration...
[OK]
Switch#
```
จากนั้นทำแบบนี้อีกรอบกับ SW2 

#### ต่อมา config ที่ PC ต่อ

ให้เรา่กดที่รูป computer เครื่องใดเครื่องหนึ่งก่อน เราจะใช้ PC-1 ในการตั้งค่าก่อน กดเข้ามาที่ PC-1 เสร็จแล้วไปกดที่ IP Configuration ให้เราแก้ IP Address Default GateWay และ Subnet Mask ตามนี้

```bash
IP Address : 10.10.10.3
Default GateWay : 10.10.10.1
Subnet Mask : 255.255.255.0
```
เครื่องที่ 2 ตั้งแบบนี้
```bash
IP Address : 10.10.20.3
Default GateWay : 10.10.20.1
Subnet Mask : 255.255.255.0
```

### เสร็จแล้ว

วิธีการทดสอบให้เรากดรูปจดหมายแล้วกดไปที่คอมพิวเตอร์สักเครื่องนึงแล้วกด ที่ปุ่ม Simulation  แล้วกดปุ่ม Play เพื่อทดสอบ