<strong>Cybersecurity Incident Report</strong>
<p>
  <em>Section 1: Identify the type of attack that may have caused this network interruption</em>
  <p>This event is being caused by a DoS attack where the attacker is sending a large amount of SYN packet requests to the website, causing it to send the error message. This could be a DoS attack called SYN flooding.</p>
</p>
<p>
  <em>Section 2: Explain how the attack is causing the website to malfunction</em>
  <p>When website visitors try to establish a connection with the web server, a three-way handshake occurs using the TCP protocol. Explain the three steps of the handshake:</p>
  <ol>
    <li>SYN packet is sent to the destination, and that packet is asking the server for connection.</li>
    <li>Once the destination responds it will send a SYN-ACK packet to the source, accepting the request.</li>
    <li>The final ACK packet is sent to the source with the permission to connect.</li>
  </ol>
  <p>When a malicious actor sends a large number of SYN packets all at the same time it overwhelms the server. Causing it to take up all of the server's recources for accepting TCP connection requests.</p>
  <p>The logs show us that a source IP of 203.0.113.0 has sent a large amount of SYN packets to the server. Therefore, it has been overwhelmed by the SYN requests. And becuase the server's connections had all been taken up, it leads to no connections for new requests from customers.</p>
</p>
