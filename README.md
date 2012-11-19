as3MQTT
=======

Pure Action Script 3 that implements the MQTT (Message Queue Telemetry Transport) protocol, a lightweight protocol for publish/subscribe messaging.

## Overview

MQ Telemetry Transport (MQTT) is a lightweight broker-based publish/subscribe messaging protocol designed to be open, simple, lightweight and easy to implement. These characteristics make it ideal for use in constrained environments, for example, but not limited to:

    #1.Where the network is expensive, has low bandwidth or is unreliable
    #2.When run on an embedded device with limited processor or memory resources

Features of the protocol include:

    #1.The publish/subscribe message pattern to provide one-to-many message distribution and decoupling of applications
    #2.A messaging transport that is agnostic to the content of the payload
    #3.The use of TCP/IP to provide basic network connectivity
    #4.Three qualities of service for message delivery:
        Qos(0):"At most once", where messages are delivered according to the best efforts of the underlying TCP/IP network. Message loss or duplication can occur. This level could be used, for example, with ambient sensor data where it does not matter if an individual reading is lost as the next one will be published soon after.
        Qos(1):"At least once", where messages are assured to arrive but duplicates may occur.
        Qos(2):"Exactly once", where message are assured to arrive exactly once. This level could be used, for example, with billing systems where duplicate or lost messages could lead to incorrect charges being applied.
    #5.A small transport overhead (the fixed-length header is just 2 bytes), and protocol exchanges minimised to reduce network traffic
    #6.A mechanism to notify interested parties to an abnormal disconnection of a client using the Last Will and Testament feature


## MQ Telemetry Transport (MQTT) V3.1 Protocol Specification

