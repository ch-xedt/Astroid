<img src="https://capsule-render.vercel.app/api?type=rect&color=2bdcfb&height=2&width=100%">

# <p align="center"> Astroid </p>


 <p align="center">
<sub><b>#####</b></sub>
</p>


 <p align="center">
<b>Astroid</b> is a lightweight, single-file web application that enables direct, peer-to-peer (P2P) file sharing between devices directly from the browser. <br>
</p>

 <p align="center">
Paired with end-to-end encryption and WebRTC technology, Astroid transfers files securely without ever uploading them to a central server or cloud storage.<br>
Because Astroid is completely static, self-hosting requires nothing more than a web server capable of serving HTML files.
</p>

<p align="center">
<sub><b>#####</b></sub>
</p>

---
 <br>


<p align="center">At its core, Astroid is designed around <code>privacy</code>, <code>speed</code>, and <code>simplicity</code>.<br> Because file payloads travel directly through WebRTC Data Channels, transfers operate at the full bandwidth available between devices without intermediary throttling or server-side bandwidth caps. Files are processed entirely in memory and streamed directly between browsers, ensuring that no data is ever uploaded, cached, or recorded on a distant server.
</p>

<p align="center">
To provide a seamless user experience, Astroid includes an automated local discovery mechanism. Devices connected to the same local network detect one another automatically through encrypted IP hash matching. When devices reside on different networks, behind aggressive firewalls, or across separate VPNs, users can establish a direct channel using secure sixteen-character room codes or shareable direct links.
</p>

<p align="center">
Signaling metadata is protected before leaving the user's device. While public MQTT brokers facilitate room discovery, all message contents, including session descriptions and candidate addresses, are encrypted client-side using AES-256-GCM. An eavesdropper monitoring the MQTT broker sees only encrypted payloads without readable metadata regarding file names, sizes, or participants.
Network observers, including public STUN servers and WebSockets infrastructure, can observe public IP addresses and connection timing. However, they remain incapable of inspecting payload data, room secrets, or file contents.
</p>

<p align="center">
<b>Note:</b> WebRTC must be enabled in all participating web browsers for direct peer-to-peer communication. Certain privacy-focused browser extensions, strict VPN configurations, or corporate firewalls that block WebRTC protocols or UDP traffic may prevent peers from establishing a direct connection.
</p>

<p align="center">
<sub><b>###########</b></sub>
</p>

<pre>Maximum File Batch Size:       Up to 500 MB per single batch</pre>
<pre>Maximum File Count:            Up to 100 files per transfer session</pre>
<pre>Session Capacity:              Up to 5 concurrent active transfer connections per client</pre>
<pre>Cryptographic Parameters:      AES-GCM 256-bit encryption combined with PBKDF2 key derivation using 100,000 iterations and SHA-256 hashing</pre>

<p align="center">
<sub><b>###############</b></sub>
</p>

<p align="center">

<sub>
<b>Open source. Every line is readable. Trust nothing you can't verify.<br></b>
</sub>
</p> <br>

<img src="https://capsule-render.vercel.app/api?type=rect&color=2bdcfb&height=2&width=100%">

<p align="center">
<sub>GNU GENERAL PUBLIC LICENSE V3</sub>
</p>

