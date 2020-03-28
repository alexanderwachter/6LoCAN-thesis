# Design and Implementation of 6LoCAN, a 6Lo adaption layer for Controller Area Networks

This work is my master thesis submitted to the university of technology Graz (TU Graz).

CC-BY
This work is licensed under a [Creative Commons Attribution 4.0 International License](http://creativecommons.org/licenses/by/4.0/).

## Abstract
Nowadays, there is an ongoing trend towards end-to-end IPv6 for con-
strained devices. This way, the devices can benefit from the vast amount
of application and transport layer protocols, defined on top of the Internet
Protocol. Examples for such application layer protocols are MQTT, CoAP,
HTTP, or transport layer protocols such as UDP, TCP, and TLS. However,
most devices on the Internet use Link-Layers that do not fit the needs of
constrained devices like power consumption, price, or PCB footprint.

The Controller Area Network (CAN) is a very robust and simple bus. Lots
of tiny microcontrollers have an integrated CAN controller that only needs
an external transceiver to connect to a bus. This bus is usually used in the
automotive and industrial domains. An example is the CANopen protocol,
designed and used for automation. However, the protocols for the CAN bus
serve a dedicated purpose and are not as flexible as the Internet Protocol.

Therefore, this work proposes 6LoCAN, an abstraction layer for the CAN
bus, which combines the great flexibility of IPv6 with the benefits of the
CAN bus. With 6LoCAN, it is possible to connect small microcontrollers to
the Internet, with only little effort. Those devices can then use application
layer protocols to communicate with devices that have Link-Layers of all
kinds, like Wi-Fi, Ethernet, or Bluetooth, without the need for a gateway.
Meanwhile, 6LoCAN has an IETF standard proposal and a reference imple-
mentation in the Zephyr Real-Time Operating System, as an outcome of
this work.
