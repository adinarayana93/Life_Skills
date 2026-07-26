# OSI Model

The OSI (Open Systems Interconnection) model is a reference model that
helps us understand how data moves from one computer to another over a
network. It divides network communication into seven layers. Each layer
has a specific responsibility, and together they make communication
between different systems easier to understand. The seven layers are
Application, Presentation, Session, Transport, Network, Data Link, and
Physical.

## 1. Application Layer

The Application layer is the top layer of the OSI model. It provides
network services that applications use to communicate over a network.
For example, web browsers, email applications, and file transfer
applications depend on protocols available at this layer.

Some common protocols are:

-   HTTP and HTTPS for web browsing.
-   FTP for file transfer.
-   SMTP for sending emails.
-   DNS for finding the IP address related to a domain name.

The application itself is not the Application layer. The layer provides
the network services and protocols needed by the application.

## 2. Presentation Layer

The Presentation layer makes sure that data is in a format that the
receiving system can understand. It mainly deals with the representation
of data.

Its common functions are:

-   Translation of data from one format to another.
-   Compression to reduce the size of data.
-   Encryption and decryption to protect data.

For example, compression can reduce the amount of data that needs to be
transferred, while encryption helps protect sensitive information during
communication.

## 3. Session Layer

The Session layer is responsible for creating, maintaining, and ending
communication sessions between applications.

Its main functions include:

-   Establishing a session.
-   Managing communication during the session.
-   Closing the session when communication is complete.
-   Providing synchronization or checkpoints when required.

In simple words, this layer manages the conversation between two
communicating systems.

## 4. Transport Layer

The Transport layer is responsible for end-to-end data delivery. It
divides large amounts of data into smaller units and helps the receiving
system put the data back together.

Two important protocols associated with transport functions are TCP and
UDP.

-   TCP provides reliable and connection-oriented communication. It is
    useful when complete and ordered delivery of data is important.
-   UDP provides connectionless communication with less overhead. It is
    useful in situations where speed is more important than
    retransmitting every lost packet.

The Transport layer also handles functions such as segmentation, flow
control, and error recovery.

## 5. Network Layer

The Network layer is responsible for moving data between different
networks. At this layer, data is handled as packets.

Its important functions are:

-   Logical addressing using IP addresses.
-   Routing packets from source to destination.
-   Choosing a suitable path for data to travel.

Routers mainly operate at this layer. IPv4 and IPv6 addresses help
identify the source and destination devices across networks.

## 6. Data Link Layer

The Data Link layer is responsible for transferring data over a local
network link. At this layer, the data unit is called a frame.

Some important functions are:

-   Framing the data received from the Network layer.
-   Using physical addresses such as MAC addresses.
-   Controlling access to the transmission medium.
-   Detecting errors in frames.

For example, when devices communicate over Ethernet or Wi-Fi, Data Link
layer functions help move frames across the local link.

## 7. Physical Layer

The Physical layer is the lowest layer of the OSI model. It is
responsible for transmitting raw bits through the physical medium.

Depending on the medium, bits can be represented using:

-   Electrical signals through copper cables.
-   Light signals through optical fibre.
-   Radio signals through wireless communication.

This layer deals with the physical transmission of 0s and 1s between
devices.

## How Data Moves Through the OSI Model

When data is sent from one computer, it moves from the Application layer
down to the Physical layer. As it moves down, the required information
is added by different layers so that the data can reach the correct
destination.

At the receiving computer, the process happens in the opposite
direction. The data moves from the Physical layer up to the Application
layer. Each layer processes the information related to it until the
original data is available to the receiving application.

A simple way to remember the flow is:

1.  Application, Presentation, and Session layers prepare and manage the
    data.
2.  Transport layer divides and manages the data for end-to-end
    delivery.
3.  Network layer adds logical addressing and routes packets.
4.  Data Link layer prepares frames for the local link.
5.  Physical layer sends the bits as signals.

## Why the OSI Model is Useful

The OSI model gives us a structured way to understand network
communication. Instead of looking at networking as one large process, we
can understand it layer by layer. It is also useful while
troubleshooting because a network problem can be checked based on the
layer where it occurs.

For example, a damaged cable can be considered a Physical layer problem,
an IP routing issue can be checked at the Network layer, and a problem
related to a web request can be investigated at the Application layer.

## Conclusion

The OSI model explains network communication using seven separate
layers, with each layer performing a particular job. Starting from
user-facing network services at the Application layer, data passes
through different stages until it is finally transmitted as signals by
the Physical layer. At the receiver, the process happens in reverse.
Understanding these layers gives a clear picture of how devices
communicate and also makes network problems easier to identify.

## References

-   [OSI Model Explained -
    YouTube](https://www.youtube.com/watch?v=vv4y_uOneC0)
-   [What Is the OSI Model? -
    IBM](https://www.ibm.com/think/topics/osi-model)
-   [What Is the OSI Model? -
    Cloudflare](https://www.cloudflare.com/learning/ddos/glossary/open-systems-interconnection-model-osi/)
