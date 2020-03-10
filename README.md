# Firewall
## Description about firewall and how to improve security of our system:

## 1. How does Firewall help to secure pc?
Firstly to know about how the firewall works, we should know about what is firewall.

### What is firewall?
```
A firewall is a network security device that monitors incoming and outgoing network traffic and permits or blocks data packets based on a
set of security rules. Its purpose is to establish a barrier between your internal network and incoming traffic from external sources (such
as the internet) in order to block malicious traffic like viruses and hackers.
```
Basically, firewall is a network security system that monitors and controls incoming and outgoing network traffic on a predefined security
rules and establishes a barrier between a trusted internal network and untrusted external network.

Firewalls carefully analyze incoming traffic based on pre-established rules and filter traffic coming from unsecured or suspicious sources
to prevent attacks. Firewalls guard traffic at a computer’s entry point, called **ports**, which is where information is exchanged with 
external devices. For example, “**Source address 172.18.1.1 is allowed to reach destination 172.18.2.1 over port 22.**"

### For example:
Let us think of IP addresses as houses and ports as room no within the house. Only trusted people (source addresses) are allowed to enter 
the house (destination address) at all—then it’s further filtered so that people within the house are only allowed to access certain rooms 
(destination ports), depending on if they're the owner, a child, or a guest. The owner is allowed to any room (any port), while children 
and guests are allowed into a certain set of rooms (specific ports). And all of this is done by firewall.

**So firewall plays a vital role in securing our system from harmful outside network**. _As the name suggests, it creates a wall between inside and outside network and monitors each data packet if it is harmful or not._

### How does it help to secure our system?
Firewall match the network traffic against the rule set defined in its table. Once the rule is matched, associate action is applied to the network traffic. For example, Rules are defined as any employee from HR department cannot access the data from code server and at the same time another rule is defined like system administrator can access the data from both HR and technical department. Rules can be defined on the firewall based on the necessity and security policies of the organization.

From the perspective of a server, network traffic can be either outgoing or incoming. Firewall maintains a distinct set of rules for both the cases. Mostly the outgoing traffic, originated from the server itself, allowed to pass. Still, setting a rule on outgoing traffic is always better in order to achieve more security and prevent unwanted communication.

Incoming traffic is treated differently. Most traffic which reaches on the firewall is one of these three major Transport Layer protocols- TCP, UDP or ICMP. All these types have a source address and destination address. Also, TCP and UDP have port numbers. ICMP uses type code instead of port number which identifies purpose of that packet.

**Default policy**: It is very difficult to explicitly cover every possible rule on the firewall. For this reason, the firewall must always have a default policy. Default policy only consists of action (accept, reject or drop).

**Accept** : Allow the traffic

**Reject** : Block the traffic but reply with an “unreachable error”

**Drop** : Block the traffic with no reply

Suppose no rule is defined about SSH connection to the server on the firewall. So, it will follow the default policy. If default policy on the firewall is set to accept, then any computer outside of your office can establish an SSH connection to the server. Therefore, setting default policy as drop (or reject) is always a good practice.


## 2. As a system admin, what precautions you will take to secure your system?
There are numerous ways to protect and remove malware from our computers. No one method is enough to ensure your computer is secure. The 
more layers of defense, the harder for hackers to use your computer.

**Check out the 5 steps to protect your computer:**
1. Install Firewall
2. Install Antivirus Software
3. Install Anti-Spyware Software
4. Use Complex and Secure Passwords
5. Check on the Security Settings of the Browser
