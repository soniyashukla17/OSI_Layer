# OSI Layer
Contents:
- [What is the OSI model?](#what-is-the-osi-model)
- [History](#History)
- [Definitions](#Definitions)
- [OSI Layers](#OSI-Layers)
   - [L1 the physical layer](#l1-the-physical-layer)
   - [L2 the data link layer](#l2-the-data-link-layer)
   - [L3 the network layer](#l3-the-network-layer)
   - [L4 the transport layer](#l4-the-transport-layer)
   - [L5 the session layer](#l5-the-session-layer)
   - [L6 the presentation layer](#l6-the-presentation-layer)
   - [L7 the application layer](#l7-the-application-layer)
- [References](#References)

## What is the OSI model?

The **Open Systems Interconnection model (OSI model)** is a conceptual model that characterises and standardises the communication functions of a telecommunication or computing system without regard to its underlying internal structure and technology. Its goal is the interoperability of diverse communication systems with standard communication protocols.

The **OSI model** was developed starting in the late 1970s to support the emergence of the diverse computer networking methods that were competing for application in the large national networking efforts in the world. In the 1980s, the model became a working product of the Open Systems Interconnection group at the International Organization for Standardization (ISO). While attempting to provide a comprehensive description of networking, the model failed to garner reliance by the software architects in the design of the early Internet, which is reflected in the less prescriptive Internet Protocol Suite, principally sponsored under the auspices of the Internet Engineering Task Force (IETF).

## History

In the early- and mid-**1970s**, networking was largely either government-sponsored (NPL network in the UK, ARPANET in the US, CYCLADES in France) or vendor-developed with proprietary standards, such as IBM's Systems Network Architecture and Digital Equipment Corporation's DECnet. Public data networks were only just beginning to emerge, and these began to use the X.25 standard in the late 1970s.

## Definitions

Communication protocols enable an entity in one host to interact with a corresponding entity at the same layer in another host. Service definitions, like the OSI Model, abstractly describe the functionality provided to an (N)-layer by an (N-1) layer, where N is one of the seven layers of protocols operating in the local host.

Data processing by two communicating OSI-compatible devices proceeds as follows:
1. The data to be transmitted is composed at the topmost layer of the transmitting device (layer N) into a protocol data unit (PDU).
2. The PDU is passed to layer N-1, where it is known as the service data unit (SDU).
3. At layer N-1 the SDU is concatenated with a header, a footer, or both, producing a layer N-1 PDU. It is then passed to layer N-2.
4. The process continues until reaching the lowermost level, from which the data is transmitted to the receiving device.
5. At the receiving device the data is passed from the lowest to the highest layer as a series of SDUs while being successively stripped    from each layer's header or footer until reaching the topmost layer, where the last of the data is consumed.


## OSI Layers                                         .

![Screenshot (1)](https://user-images.githubusercontent.com/88364921/128641615-a68dfda2-f5ad-41c4-9075-44252deeb036.png)
![Screenshot (3)](https://user-images.githubusercontent.com/88364921/128641627-1590d970-1c06-4388-9db7-bb653e9ae1a4.png) 

Each layers are explained below in brief.

## L1 the physical layer

The **physical layer** is responsible for the transmission and reception of unstructured raw data between a device and a physical transmission medium. It converts the digital bits into electrical, radio, or optical signals. Layer specifications define characteristics such as voltage levels, the timing of voltage changes, physical data rates, maximum transmission distances, modulation scheme, channel access method and physical connectors. This includes the layout of pins, voltages, line impedance, cable specifications, signal timing and frequency for wireless devices. Bit rate control is done at the physical layer and may define transmission mode as simplex, half duplex, and full duplex. The components of a physical layer can be described in terms of a network topology. Physical layer specifications are included in the specifications for the ubiquitous Bluetooth, Ethernet, and USB standards. An example of a less well-known physical layer specification would be for the CAN standard.

## L2 the data link layer

The **data link layer** provides node-to-node data transfer???a link between two directly connected nodes. It detects and possibly corrects errors that may occur in the physical layer. It defines the protocol to establish and terminate a connection between two physically connected devices. It also defines the protocol for flow control between them.

## L3 the network layer

The **network layer** provides the functional and procedural means of transferring packets from one node to another connected in "different networks". A network is a medium to which many nodes can be connected, on which every node has an address and which permits nodes connected to it to transfer messages to other nodes connected to it by merely providing the content of a message and the address of the destination node and letting the network find the way to deliver the message to the destination node, possibly routing it through intermediate nodes.

## L4 the transport layer

The **transport layer** may control the reliability of a given link through flow control, segmentation/desegmentation, and error control. Some protocols are state- and connection-oriented. This means that the transport layer can keep track of the segments and retransmit those that fail delivery. The transport layer may also provide the acknowledgement of the successful data transmission and sends the next data if no errors occurred. The transport layer creates segments out of the message received from the application layer. Segmentation is the process of dividing a long message into smaller messages.

## L5 the session layer

The **session layer** controls the dialogues (connections) between computers. It establishes, manages and terminates the connections between the local and remote application. It provides for full-duplex, half-duplex, or simplex operation, and establishes procedures for checkpointing, suspending, restarting, and terminating a session. In the OSI model, this layer is responsible for gracefully closing a session. This layer is also responsible for session checkpointing and recovery, which is not usually used in the Internet Protocol Suite. The session layer is commonly implemented explicitly in application environments that use remote procedure calls.

## L6 the presentation layer

The **presentation layer** establishes context between application-layer entities, in which the application-layer entities may use different syntax and semantics if the presentation service provides a mapping between them. If a mapping is available, presentation protocol data units are encapsulated into session protocol data units and passed down the protocol stack.

## L7 the application layer

The **application layer** is the OSI layer closest to the end user, which means both the OSI application layer and the user interact directly with the software application. This layer interacts with software applications that implement a communicating component. Such application programs fall outside the scope of the OSI model. Application-layer functions typically include identifying communication partners, determining resource availability, and synchronizing communication.

## References

1. https://www.google.com/search?q=osi+layer+wikipedia&rlz=1C1VDKB_enIN965IN965&oq=osi+layer+wiki&aqs=chrome.0.0i20i263i512j69i57j0i22i30l2.5276j0j7&sourceid=chrome&ie=UTF-8

2. https://www.youtube.com/watch?v=LANW3m7UgWs
