The internet is a computer network that interconnects billions of computing devices throughout the world.
Devices connected to the internet are called **hosts** or **end systems**.
Hosts/end systems can be further divided into two categories: clients (which informally tend to be
dekstop and mobile PCs, smartphones and so on) and servers (which tend to be more powerful machines
that store and distribute web pages, stream video, relay email and so on. Today most servers reside in
large data centers. 

End systems are connected together by a network of communication links and packet switches. 
Communication links are made up of many different types of physical media including coaxial cable, copper
wire, optical fibre, and radio spectrum.
Different links transmit data at different rates.
The **tranmission rate** is measured in bits/second.

When transmitting data, the sending end system segments the data and adds header bytes to each segment.
The resulting **packets** are then sent through the network to the destination end system, where they are
reassembled into the original data.
A packet switch takes a packet arriving on one of its incoming communication links and forwards that
packet on one of its outgoing communication links. 
Two of the most common packet switches are routers and link layer switches. 
The sequence of packet switches traversed by a packet is known as its **route** or **path** through the network.

End systems access the internet through **internet services providers (ISPs)**. Each ISP is in itself a
network of communication links and packet switches. 
They provide a variety of types of network access including residential broadband access, local area network
and mobile wireless.
ISPs that provide internet access to end systems are themselves interconnected through national and 
international upper tier ISPs such as Level 3 communications, AT&T and NTT that consist of high speed routers
and fibre-optic links.

Each ISP network runs certain protocols and conforms to certain naming and address conventions. 
A protocol defines the format and order of messages exchanged between two or more communicating entities,
as well as the actions taken on the transmission or receipt of message or other event.
Two of the most important protocols are the **Internet Protocol (IP)** and **Transmission Control Protocal (TCP)**.

Internet standards are developed by the Internet Engineering Task Force (IETF).

The internet can also be though of as an *infrastructure that provides services to applications* such as
email, internet messaging, web surfing and streaming.
Internet applications run on end systems, not packet switches. End systems attached to the internet provide
a **socket interface** the specifies how a program running on one end system asks the internet infrastructure
to deliver data to a specific destination program running on another end system.

Access networks:
1. Digital subscriber line (DSL)
  * Each customer's DSL modem uses the existing telephone line to exchange data with the DSL access multiplexer (DSLAM)
  located in the telco's local central office (CO). 
  * The DSL modem takes digital data and translates it to high frequency tones for tranmission over telephone lines.
  * These analog signals are translated back in to digital format at the DSLAM.
  * A splitter separates telephone and data signals arriving to the home from CO and forwards the data to DSL mode.
  * Hundreds/thousands of houses connect to a single DSLAM.
  * Data and telephone signals are transmitted simultaneously but at different frequencies 
  * 0-4kHz phone; 4-50Khz upstream data; 50Khz-1MHz downstream data
  * This is known as frequency-division multiplexing.
  * Tranmission rates: 55 Mbps downstream; 15 Mbps upstream [ITU 2006 standard]
  * Transmission rate is limited by the distance between the home and CO, the gauge of the telephone line 
    and degree of electrical interference.
2. Cable internet access
  * Makes use of existing cable television infrastructure.
  * Fibre optics connect the cable head to neighborhood level junctions.
  * Traditional coaxial cable is used to reach individual homes from these junctions. 
  * Each junction typically supports 500 - 5000 homes.
  * Cable internet access requires a special cable modem which connects to the home PC through an ethernet port.
  * The cable modem termination system (CMTS) serves function equivalent to DSLAM. 
  * Tranmission rates: 42.8 Mbps downstream; 30.7 Mbps upstream
  * Notably, cable internet access is a shared broadcast medium. Every packet sent by the head end travels
    downstream to every home. Every packet sent by a home travels on the upstream channel to the head end.
  * Hence, is several users are downloading a video simultaneously, the actual downstream rate may be significantly 
    lower than the typical rate.
  * A distributed multiple access protocol is needed to coordinate tranmissions and avoid collisions.
3. Fibre to the home (FTTH)
  * Provide an optical fibre path from the CO directly to the home.
  * Much faster than cable and DSL
  * Direct fibre: One fibre leaving the CO for each home.
  * More commonly, each fibre leaving the CO is shared by many homes and split into individual fibres relatively close to the homes.
  * Two network architectures that perform this splitting: active optical networks (AONs) & passive optical networks (PONs)
4. Satellite link
5. Dial-up access
