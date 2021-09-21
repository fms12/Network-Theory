
## Introduction of Data Link Layer

**The data link layer is responsible for the node to node
delivery of the message. The main function of this layer is
to make sure data transfer is error-free from one node to another, 
over the physical layer. When a packet arrives in a network, it is the responsibility of DLL to transmit it to the Host using its MAC address.** 

The working is as follows:

##
![Image](https://i.ibb.co/k6TR5qR/data-linklayer.png)
##

## Data Link Layer is divided into two sub layers :

Logical Link Control (LLC)
Media Access Control (MAC)

The packet received from the Network layer is further divided into frames depending on the frame size of NIC(Network Interface Card). DLL also encapsulates Sender and Receiver’s MAC address in the header.

The Receiver’s MAC address is obtained by placing an ARP(Address Resolution Protocol) request onto the wire asking "Who has that IP address?" and the destination host will reply with its MAC address.

Now let's see how the DLL works in a small office:

#

![Image](https://i.ibb.co/grkrtNX/3.png)

#

The switch is used to connect multiple computers or laptops which in turn is connected to a router. This is then connected to the internet. All the 1-to-1 connection is done using DLL. The setup is called LAN as they are all connected in Local Area Network.

Now let's see how the DLL works in a small office:

![Image](https://i.ibb.co/7pgxr7K/4.png)
#

## The functions of the Data Link layer are

1. **Framing**: Framing is a function of the data link layer. It provides a way for a sender to transmit a set of bits that are meaningful to the receiver. This can be accomplished by attaching special bit patterns to the beginning and end of the frame.

2. **Physical addressing**: After creating frames, Data link layer adds physical addresses (MAC address) of sender and/or receiver in the header of each frame.

3. **Error Detection**: Data link layer provides the mechanism of error control in which it detects and retransmits damaged or lost frames.

4. **Error and Flow Control**: The data rate must be constant on both sides else the data may get corrupted thus, flow control coordinates that amount of data that can be sent before receiving acknowledgement.

5. **Access control**: When a single communication channel is shared by multiple devices, MAC sub-layer of data link layer helps to determine which device has control over the channel at a given time.

** Packet in Data Link layer is referred as **Frame** 

** Data Link layer is handled by the NIC (Network Interface Card) and device drivers of host machines.\
*** Switch & Bridge are Data Link Layer devices.
