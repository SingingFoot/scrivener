+++
title = "Quality of Service in MQTT Integration Setup"
description = "This is an area for technical documentation"
weight = 1
+++

You can select an MQTT **Quality of Service** (QoS) level during the Integration Setup procedure. We use MQTT QoS **level 0** (At most once) by default.

ThingsBoard supports MQTT QoS **level 1**, which means that a client receives a response to the publish message only after data is stored to **Cassandra DB**. Data duplicates which are possible with QoS **level 1** are just the overwrites to the corresponding Cassandra row and thus are not present in persisted data. This functionality provides reliable data delivery and persistence.

:::tip

**Quality of Service (QoS)** in MQTT messaging is an agreement between sender and receiver on the guarantee of delivering a message.

:::

There are three levels of **QoS**


|   Level 	|   Mark	        |   Explanation	         |
|---	    |---	            |---	                 |
|   0	    |   at most once	|This is the simplest, lowest-overhead method of sending a message. The client simply publishes the message, and there is no acknowledgement by the broker.      	|
|   1	    |   at least once       	|  This method guarantees that the message will be transferred successfully to the broker. The broker sends an acknowledgement back to the sender, but in the event that that the acknowledgement is lost the sender won't realise the message has got through, so will send the message again. The client will re-send until it gets the broker's acknowledgement. This means that sending is guaranteed, although the message may reach the broker more than once.	|
|   2	    |   exactly once        	| This is the highest level of service, in which there is a sequence of four messages between the sender and the receiver, a kind of handshake to confirm that the main message has been sent and that the acknowledgement has been received. When the handshake has been completed, both sender and receiver are sure that the message was sent exactly once.  	|

## Which QoS to use for your IoT application?

---

>**QoS 0 is the lowest-cost in terms of volume of data transfer. This is suitable when you have a reliable connection between device and broker.**

---

You should consider whether your IoT application can tolerate the loss of a message now and again. For example, if a device is monitoring something and sending cumulative readings, then the impact of a lost message will just be a delay in those readings reaching the server.

---

>**QoS 1 is a good choice if you need to be sure every message gets through, but your IoT application can tolerate receiving a message more than once.**

---

If the sending device is transmitting cumulative data readings from an asset, then QoS 1 may be suitable, because any incidences of a message being received more than once by the server should have little effect. But if the readings sent are some "change since last transmission" (for example, number of times a button was pressed), then a duplicate message may create misleading data in the portal.

One way to get around this is to ensure devices send every message with unique timestamp. Assetwolf will recognise a duplicate message based on the timestamp and will ignore it.

---

>**QoS 2 guarantees delivery exactly once, but has a relatively high cost in terms of data transfer.** 

---

Most applications should work without problem with QoS 2, but you should consider whether a lower-cost QoS would be suitable. Often through careful choice of fields in the data — using timestamps and cumulative data readings — is an easy way to avoid the overhead of QoS 2.

![Quality of Service Structure](/img/docusaurus/qos.jpeg "Quality of Service Structure")