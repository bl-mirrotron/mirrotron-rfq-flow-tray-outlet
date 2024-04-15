# RFQ Outlet Flow Tray
* <a href="https://github.com/bl-mirrotron/mirrotron-rfq-flow-tray-outlet" target="_blank">Source code</a>
* [Cooling system overview](https://bl-mirrotron.github.io/#cooling-system)
* [Control system overview](https://bl-mirrotron.github.io/)

The function of the RFQ Outlet Flow Tray is to receive data and check alarm status from the <a href="https://bl-mirrotron.github.io/mirrotron-rfq-flow-cube/">RFQ Flow Cube</a> mounted on the outlet header as shown in Figure 1. The tray is installed on a Raspberry Pi ZeroW as shown in Figure 2. The Raspberry Pi ZeroW is actually mounted on the underside of the Flow cube as shown in Figure 3.

Because the cooling headers are located far from any Ethernet connection, the tray communicates with the <a href="https://bl-mirrotron.github.io/mirrotron-box/">Mirrotron application server</a> via wireless connections. A continuously changing watchdog signal verifies that the communication link is intact. The tray code is written in the <a href="https://nodered.org/" target="_blank">Node-RED</a> programming environment. The tray code uses the standard Blinky-Lite template for serial communication using Blinky-Bus as shown in Figure 4.

<p></p><p style="text-align:center;font-size: large;"><span style="font-weight: bold;color: green;">Figure 1. </span> <span style="font-style: italic;">Outlet Cooling Header.<br>From left to right: Temperature cube and tray, 5V power, 24V power, Flow cube and tray</span></p>
<div style="width:100%;text-align:center;"><img width="100%" style="border-style:solid;border-color:#1c6e97;" src="doc/RFQCoolingOutletHeader.jpg"/></div><br>

<p></p><p style="text-align:center;font-size: large;"><span style="font-weight: bold;color: green;">Figure 2. </span> <span style="font-style: italic;">Raspberry Pi ZeroW tray along with flow cube</span></p>
<div style="width:100%;text-align:center;"><img width="100%" style="border-style:solid;border-color:#1c6e97;" src="doc/flowCubeWithRPi.jpg"/></div><br>

<p></p><p style="text-align:center;font-size: large;"><span style="font-weight: bold;color: green;">Figure 3. </span> <span style="font-style: italic;">Raspberry Pi ZeroW tray mounted on flow cube</span></p>
<div style="width:100%;text-align:center;"><img width="100%" style="border-style:solid;border-color:#1c6e97;" src="doc/flowCubeWithTray.jpg"/></div><br>

<p></p><p style="text-align:center;font-size: large;"><span style="font-weight: bold;color: green;">Figure 4. </span> <span style="font-style: italic;">RFQ Outlet Flow Tray Node-RED flow</span></p>
<div style="width:100%;text-align:center;"><img width="100%" style="border-style:solid;border-color:#1c6e97;" src="doc/mirrotron-rfq-flow-tray-outlet.png"/></div><br>
