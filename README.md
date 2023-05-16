# Command_Pedia
In today's fast-paced and information-driven world, easy access to knowledge plays a
pivotal role in personal, educational, and professional growth. As the volume of
information continues to expand exponentially, there arises a pressing need for efficient,
reliable, and convenient platforms that empower individuals to navigate this vast sea of
knowledge. The Command Line Encyclopedia is a sophisticated server-client application
that utilizes socket programming and thread management to provide users with a
seamless command line interface for retrieving information on various topics. This
project aims to create an efficient and scalable system where multiple clients can connect
to a central server, submit their queries, and receive relevant information in real-time.The
user, acting as a client, interacts with the system through a terminal interface. By entering
a specific "topic" of interest, the client initiates a request to the server. The server, in turn,
processes the query by searching through an internally developed file system, which
contains a comprehensive collection of information. Once the requested information is
found, the server responds to the client, providing the relevant details.

## Features
● **Provides an easy access to information:** The application provides the user with
a seamless command line interface for retrieving information on various topics.
The client can make requests for information on a specific topic which are then
processed by the server by searching for information in an internal file system, and
the retrieved information is then passed on to the client. The application hence acts
as a comprehensive source of easily available knowledge for the client. <br><br>
● **Multiple connections can be established simultaneously:** The application uses
threading to enable the server to connect to multiple clients at once. Multiple users
can access the information simultaneously in this manner and this helps make the
application scalable for future use. <br><br>
● **Different operation modes:** The application can be used in two different
operation modes, user mode and admin mode. In the user mode, the already
available information can be accessed by the client. Whereas, in the admin mode,
the client can provide more topics and information to the server which are then
stored by the server and can be used for connections. <br><br>
● **Add information to the server:** The client can also add new topics and their
corresponding information to the server’s file system. This is done in the admin
mode. <br><br>
● **User registration and validation:** Users have to register themselves with the
server using a particular format. The server also validates the user’s name to
ensure that it is entered in the correct format. <br><br>
● **Termination:** The user can anytime choose to exit the application by entering ‘q’
as their input message. <br><br>

## Requirements
#### Technologies Used:
Socket Programming: For Client server interaction <br>
Threading: For entertaining multiple clients <br>
C language: For writing programs <br>
Inbuilt file system: For storing the information about various topics on the server side <br>

#### Pre-requisites:
Note: This project requires the Linux Operating System.
1. Clone the code from the following repository:
https://github.com/Isha9943/Command_Pedia
2. Compile the Server.c file and run it in a terminal window using the following
command:
$ gcc Server.c -o Server && ./Server
3. Open a new terminal window and compile and run the client file using the
following command:
$ gcc Client.c -o Client && ./Client

## Code Overview
#### Structure: 
The project consists of initially 2 folders and 2 major files. <br>
1. Folders:
   - Index: This stores the names of all the topics that the server contains the information about.
   - Topics: This contains the information about each topic present in the index folder.
2. Files:
   - Server.c: To implement a basic server that handles multiple client connections, allowing users to search for topics and admins to add new topics
   - Client.c: To establish a connection to a server, allows the user to send messages to the server, and receives messages from the server, using a multi-threaded approach.




