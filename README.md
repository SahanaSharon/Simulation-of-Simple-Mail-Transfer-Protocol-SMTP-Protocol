Objective :

This project simulates how the Simple Mail Transfer Protocol (SMTP) works, demonstrating how an email is sent from a client to a server.

Working : 

1. Connection Begins - 

The client (like your email app or Python script) wants to send an email. It opens a connection to the SMTP server (like smtp.gmail.com) through port 25, 587, or 465.

2. Handshake - The client says "HELO" (or "EHLO") to introduce itself. The server replies: "Hello, I’m ready."

3. Sender Identifies- The client sends: MAIL FROM:<sender@example.com>The server replies:  OK

4. Recipient is Given - The client says: RCPT TO:<receiver@example.com>. Server checks if it can accept email for that user and replies: ✅ OK

5. Send the Message - The client says: DATA. Server replies: "Enter your message. End with a dot (.) on a new line". The client sends: Subject: Hello.This is a test email. The server responds: Message accepted!

6. End the Connection - The client says: QUIT. The server says: Goodbye, and the connection closes.
