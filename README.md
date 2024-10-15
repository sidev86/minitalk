<h1>minitalk</h1>

<h2>Description</h2>

This project implements a communication system in the form of a client and a server, utilizing UNIX signals for message transmission.<br>
The server is designed to handle multiple client requests in sequence, efficiently processing messages while providing feedback.


<h2>Project Features</h2>


<ul>
    <li><strong>Server Initialization:</strong> The server must be started first, displaying its Process ID (PID) upon launch.</li>
    <li><strong>Client Parameters:</strong> The client requires two parameters:
        <ul>
            <li><strong>Server PID:</strong> The PID of the server to which the client will connect.</li>
            <li><strong>Message String:</strong> The string to be sent to the server.</li>
        </ul>
    </li>
    <li><strong>Message Transmission:</strong> The client sends the specified string to the server, which then prints the received message.</li>
    <li><strong>Performance:</strong> The server is required to display received strings quickly, ensuring minimal delay in message processing.</li>
    <li><strong>Signal Communication:</strong> Communication between the client and server is achieved solely through UNIX signals, specifically <code>SIGUSR1</code> and <code>SIGUSR2</code>.</li>
    <li><strong>Multi-client Support:</strong> The server can receive strings from multiple clients in succession without needing to restart.</li>
</ul>
