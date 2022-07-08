Communicator - Written by Benjamin Jack Cullen

A Very Powerful Communications Tool - Project in early development.

Communicator is capable of potentially communicating with any IPv4, Domain Name, IPv6 and MAC addresses
and potentially anything in the Universe running and or not running a Communicator, this makes the 
Communicator very powerful. Use wisely.

The Communicator is a very powerful Communications Tool. The Communicator is not a place to meet people, its not a
chat lobby or meeting place and is certainly not a chat app.

Communicate with Machines and Humanoids. MAC support. (MAC may speak Chinese) Test a device that supports wake 
on LAN with: ￿￿￿呰蒴︠呰蒴︠呰蒴︠呰蒴︠呰蒴︠呰蒴︠呰蒴︠呰蒴︠呰蒴︠呰蒴︠呰蒴︠呰蒴︠呰蒴︠呰蒴︠呰蒴︠呰蒴︠
This example is how you would wake up a device. Upcoming, send string of bytes.
Please BE EXTREMELY CAREFUL.

Input sanitization is incomplete. Exercise extreme caution when entering data into input fields.
Name: no spaces
Address: IP/MAC space_delimiter PORT space_delimiter optional broadcast address

Communicator Standard Communication:
1. Messages encrypted with AES-256 32 bytes shared key.
2. Messages contain encrypted shared fingerprint and encrypted message. Key's are not transmitted by the
communicator and to read the 32x32 bytes fingerprint contained in a Communicator Standard Communication message you
will need the key.
3. The key is intended to make the communication more secure and the fingerprint is intended to provide some
reasonable assurance that you know who the sender is.
4. Fingerprint contained in AES-256 encrypted message is used to help assure you of the identity of the sender.
5. To send a Standard Communicator Communication use the Communicator. First a 32 character key and a 32x32 (1024)
character fingerprint must be generated and shared between the intended sender and recipient. It is strongly advised
to share a different key and fingerprint between each sender and recipient. This way you have a reasonable assurance
that you know who is communicating with you regardless of IP address and regardless of any other data.
6. The Communicator Server Data Handler performs dictionary attacks on incoming messages over 1024 bytes in order
to try and decrypt the message thereby identifying the sender and enabling the message to be read. This requires
the address book is properly configured.
7. The above comprises much of the Communicator Standard Communication.
8. It is also recommended sharing the key and fingerprint offline.
9. Green notification is for message delivered and Communicator Standard Communication received.


Communicator Non-Standard Communication:
1. The communicator filters any incoming message below 1024 bytes away from the decryption function, this among
other reasons allows a 'Communicator Non-Standard Communication' which allows for things like plain text to be sent
up to 1024 bytes and be received and receive notification.
2. Great for emergencies as this will not require a key or fingerprint however the communication will be insecure.
3. Amber notification is for Communicator Non-Standard Communication received. Potentially insecure message received
or key/fingerprint not found for message.


Key Trust Logic:
The Key Trust logic. A scenario involving two people and a stranger.
1. Person 1 creates a key and fingerprint for person 1 and person 2 to use.
2. Person 1 shares the key and fingerprint with person 2.
3. Person 2 could break the trust and share the key and fingerprint with the stranger however now the only person
who can be impersonated is person 2, which person 2 might likely not want.
4. If person 2 still went ahead and shared the key and fingerprint then not only can stranger (and anyone else who
now has the key and fingerprint) pretend to be person 2, they can also decrypt BOTH person 1 AND person 2's messages,
which is in neither persons favour.
5. Share a different key and fingerprint for each contact in the address book.


DOS & DDOS Protection Framework:
1. Easily Tunable Communicator Anti-DOS & Anti-DDOS Framework provides a certain level of protection.
2. Testing for DOS proves working. DDOS remains untested.


Python version - 3.9
Platform - Developed on Windows 10.

Pycrypto Installation:
1. If encounter error: error: command 'C:\\Program Files\\Microsoft Visual Studio\\2022\\Professional\\VC\\Tools\\MSVC\\14.31.31103\\bin\\HostX86\\x64\\cl.exe' failed with exit code 2
2. In Admin CMD Run: (adjust path according to your MVS version)
"C:\Program Files\Microsoft Visual Studio\2022\Professional\VC\Auxiliary\Build\vcvarsx86_amd64.bat"
3. Then Run: (adjust path according to your MVS version)
set CL=-FI"%VCINSTALLDIR%Tools\MSVC\14.16.27023\include\stdint.h
4. Then pip install pycrypto.

Donations are very much welcome: Paypal benjaminjc173@gmail.com
