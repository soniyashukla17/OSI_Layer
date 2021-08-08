# OSI Layer
Contents:
- [What is the OSI model?](#what-is-the-osi-model)
- [History](#History)
- [Definitions](#Definitions)
- [OSI Layers](#OSI Layers)
  - [Each Layers in Details](#Each Layers in Details)
   - [L1 the physical layer](#l1-the-physical-layer)
   - [L2 the data link layer](#l2-the-data-link-layer)
   - [L3 the network layer](#l3-the-network-layer)
   - [L4 the transport layer](#l4-the-transport-layer)
   - [L5 the session layer](#l5-the-session-layer)
   - [L6 the presentation layer](#l6-the-presentation-layer)
   - [L7 the application layer](#l7-the-application-layer)
## What is the OSI model?

The **Open Systems Interconnection model (OSI model)** is a conceptual model that characterises and standardises the communication functions of a telecommunication or computing system without regard to its underlying internal structure and technology. Its goal is the interoperability of diverse communication systems with standard communication protocols.

The model partitions the flow of data in a communication system into seven abstraction layers, from the physical implementation of transmitting bits across a communications medium to the highest-level representation of data of a distributed application. Each intermediate layer serves a class of functionality to the layer above it and is served by the layer below it. Classes of functionality are realized in software by standardized communication protocols.
    
The OSI model was developed starting in the late 1970s to support the emergence of the diverse computer networking methods that were competing for application in the large national networking efforts in the world. In the 1980s, the model became a working product of the Open Systems Interconnection group at the International Organization for Standardization (ISO). While attempting to provide a comprehensive description of networking, the model failed to garner reliance by the software architects in the design of the early Internet, which is reflected in the less prescriptive Internet Protocol Suite, principally sponsored under the auspices of the Internet Engineering Task Force (IETF).

## History

In the early- and mid-1970s, networking was largely either government-sponsored (NPL network in the UK, ARPANET in the US, CYCLADES in France) or vendor-developed with proprietary standards, such as IBM's Systems Network Architecture and Digital Equipment Corporation's DECnet. Public data networks were only just beginning to emerge, and these began to use the X.25 standard in the late 1970s.

The Experimental Packet Switched System in the UK circa 1973-5 identified the need for defining higher level protocols.[1] The UK National Computing Centre publication 'Why Distributed Computing' which came from considerable research into future configurations for computer systems,[3] resulted in the UK presenting the case for an international standards committee to cover this area at the ISO meeting in Sydney in March 1977.

## Definitions

Communication protocols enable an entity in one host to interact with a corresponding entity at the same layer in another host. Service definitions, like the OSI Model, abstractly describe the functionality provided to an (N)-layer by an (N-1) layer, where N is one of the seven layers of protocols operating in the local host.

Data processing by two communicating OSI-compatible devices proceeds as follows:
1. The data to be transmitted is composed at the topmost layer of the transmitting device (layer N) into a protocol data unit (PDU).
2. The PDU is passed to layer N-1, where it is known as the service data unit (SDU).
3. At layer N-1 the SDU is concatenated with a header, a footer, or both, producing a layer N-1 PDU. It is then passed to layer N-2.
4. The process continues until reaching the lowermost level, from which the data is transmitted to the receiving device.
5. At the receiving device the data is passed from the lowest to the highest layer as a series of SDUs while being successively stripped    from each layer's header or footer until reaching the topmost layer, where the last of the data is consumed.
