# cs390006-assignment-1-using-tcp-sockets-solved
**TO GET THIS SOLUTION VISIT:** [CS390006 Assignment 1-Using TCP Sockets Solved](https://www.ankitcodinghub.com/product/cs390006-cs-39006-assignment-1-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;116867&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;3&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (3 votes)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CS390006 Assignment 1-Using TCP Sockets Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (3 votes)    </div>
    </div>
&nbsp;

Problem 1(a):

In this assignment, you will write a client-server system using TCP sockets. Specifically, you will write two programs, a TCP client program and an iterative TCP server program. The client program will send a text file to the server program. The server will count the number of sentences, words, and characters in the file and send them back to the client. The client will then display it. The sequence of operations to be followed are shown below.

1. The server opens a TCP socket and waits for a request from the client.

2. The client reads the name of a text file from the user as a command line argument. It then looks for the file in the local directory. If the file is not there, it prints a suitable error message (“File not found”) and exits. If the file is found, the steps below are executed. You can assume that the file name has maximum 100 characters and the file, if found, will always be a text file containing English sentences.

3. The client establishes a connection to the server using the connect() call.

4. The client reads the contents of the file and sends it to the server using the TCP socket. Since the file can be arbitrarily long, the client cannot send the entire file in a single send() call, and sends the file in small chunks using multiple send() calls until the entire file is transferred. The chunk size used by the client is not known to the server.

5. The server receives the file, and computes the number of characters, number of words, and number of sentences in the paragraph, and sends these numbers back to the client using the same TCP socket. The server then waits for the next client request.

6. The client will print these numbers on the screen.

7. You can assume that in the file, each sentence is terminated with a full stop character only, and the fullstop character appears only at the end of sentences and nowhere else. Also, any sentence has at least one character which is not a fullstop.

Your code should satisfy the following conditions:

1. The maximum size of any buffer used by either the client or the server is 100 bytes (you can assume this is known to both client and server).

2. The client does not determine or send to the server the size of the file in any way.

3. You cannot use fopen/fscanf functions. You must use open/read functions to open and read the file.

4. The server is not allowed to write anything in a file. It should count on the fly from the buffer.

You can assume that only a single client will connect to the server at any one time.

Problem 1(b):
