Supported Boards
=================


Synthetic Board
----------------


This board generates synthetic data and you dont need real hardware to use it.

To choose this board in BoardShim class please specify:

- board_id: -1

Supported platforms:

- Windows >= 8.1
- Linux
- MacOS

Board Specs:

- num eeg(emg) channels: 8
- num acceleration channels: 3
- sampling rate: 256
- communication: None


OpenBCI Cyton
--------------

.. image:: https://farm5.staticflickr.com/4817/32567183898_10a4b56659.jpg

`Cyton geting started guide from OpenBCI <https://docs.openbci.com/Tutorials/00-Tutorials>`_.

To choose this board in BoardShim class please specify:

- board_id: 0
- serial_port field of BrainFlowInputStruct

Supported platforms:

- Windows >= 8.1
- Linux
- MacOS

Board Spec:

- num eeg(emg) channels: 8
- num acceleration channels: 3
- sampling rate: 250
- communication: serial port

OpenBCI Ganglion
-----------------

.. image:: https://live.staticflickr.com/65535/48288408326_7f078cd2eb.jpg

`Ganglion geting started guide from OpenBCI <https://docs.openbci.com/Tutorials/00-Tutorials>`_.

prepare_session args to select this board:

To choose this board in BoardShim class please specify:

- board_id: 1
- mac_address field of BrainFlowInputStruct, if its empty BrainFlow will try to autodiscover it

Supported platforms:

- Windows >= 10
- Linux
- MacOS

Additional configuration:

- If you use python bindings installed from PYPI on Windows you may need to install `redist_x64 <https://aka.ms/vs/16/release/vc_redist.x64.exe>`_ or `redist_x86 <https://aka.ms/vs/16/release/vc_redist.x86.exe>`_  (but more likely you have it preinstalled)
- For Linux/MacOS you need to use dongle, for Windows dongle is not required if you have Bluetooth on your laptop

Board Spec:

- num eeg(emg) channels: 4
- num acceleration channels: 3
- sampling rate: 200
- communication: Bluetooth Low Energy


OpenBCI Cyton Daisy
--------------------

.. image:: https://live.staticflickr.com/65535/48288597712_7ba142797e.jpg

`Cyton Daisy geting started guide from OpenBCI <https://docs.openbci.com/Tutorials/00-Tutorials>`_.

To choose this board in BoardShim class please specify:

- board_id: 2
- serial_port field of BrainFlowInputStruct

Supported platforms:

- Windows >= 8.1
- Linux
- MacOS

Board Spec:

- num eeg(emg) channels: 16
- num acceleration channels: 3
- sampling rate: 125
- communication: Bluetooth Low Energy


OpenBCI Ganglion with Wifi Shield
-----------------------------------

.. image:: https://live.staticflickr.com/65535/48836544227_05059fc450_b.jpg

`Wifi shield geting started guide from OpenBCI <https://docs.openbci.com/docs/01GettingStarted/01-Boards/WiFiGS>`_.

`Wifi shield programming guide from OpenBCI <https://docs.openbci.com/docs/05ThirdParty/03-WiFiShield/WiFiProgam>`_.

To choose this board in BoardShim class please specify:

- board_id: 4
- ip_address field of BrainFlowInputStruct should contain WiFi Shield Ip address(in direct mode its 192.168.4.1)
- ip_protocol field of BrainFlowInputStruct should be IpProtocolType.TCP
- ip_port field of BrainFlowInputStruct should be any local port which is free right now

Supported platforms:

- Windows >= 8.1
- Linux
- MacOS


Board Spec:

- num eeg(emg) channels: 4
- num acceleration channels: 3
- sampling rate: 1600
- communication: tcp socket to read data(local port 17982) and http to send commands



OpenBCI Cyton with Wifi Shield
---------------------------------

.. image:: https://live.staticflickr.com/65535/48836367066_a8c4b6d3be_b.jpg

`Wifi shield geting started guide from OpenBCI <https://docs.openbci.com/docs/01GettingStarted/01-Boards/WiFiGS>`_.

`Wifi shield programming guide from OpenBCI <https://docs.openbci.com/docs/05ThirdParty/03-WiFiShield/WiFiProgam>`_.

To choose this board in BoardShim class please specify:

- board_id: 5
- ip_address field of BrainFlowInputStruct should contain WiFi Shield Ip address(in direct mode its 192.168.4.1)
- ip_protocol field of BrainFlowInputStruct should be IpProtocolType.TCP
- ip_port field of BrainFlowInputStruct should be any local port which is free right now

Supported platforms:

- Windows >= 8.1
- Linux
- MacOS


Board Spec:

- num eeg(emg) channels: 8
- num acceleration channels: 3
- sampling rate: 1000
- communication: tcp socket to read data(local port 17982) and http to send commands


OpenBCI Cyton Daisy with Wifi Shield
--------------------------------------

.. image:: https://live.staticflickr.com/65535/48843419918_f11c90deb0_k.jpg

`Wifi shield geting started guide from OpenBCI <https://docs.openbci.com/docs/01GettingStarted/01-Boards/WiFiGS>`_.

`Wifi shield programming guide from OpenBCI <https://docs.openbci.com/docs/05ThirdParty/03-WiFiShield/WiFiProgam>`_.

To choose this board in BoardShim class please specify:

- board_id: 6
- ip_address field of BrainFlowInputStruct should contain WiFi Shield Ip address(in direct mode its 192.168.4.1)
- ip_protocol field of BrainFlowInputStruct should be IpProtocolType.TCP
- ip_port field of BrainFlowInputStruct should be any local port which is free right now

Supported platforms:

- Windows >= 8.1
- Linux
- MacOS

Board Spec:

- num eeg(emg) channels: 16
- num acceleration channels: 3
- sampling rate: 1000
- communication: tcp socket to read data(local port 17982) and http to send commands
