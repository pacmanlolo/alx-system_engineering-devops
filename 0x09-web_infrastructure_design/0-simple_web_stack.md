/**A user wants to access a website hosted on a one server web infrastructure via www.foobar.com

Let us go into details of the infrastructures used:
1.	Server:  This will host the website and store the web application, database, and any other files that are necessary.
2.	Domain name: Here, the domain name “foobar.com” is configured to point to the ip address of the server hosting the website.
3.	DNS: the DNS record www is in www.foobar.com: the www record for foobar.com is configured to point to the ip address of the server hosting the website.
4.	The role of the web server: This is NGINX, which will receive requests from the user's web browser and deliver the website's web pages.
5.	The role of the application server: This will execute the codebase for the website's web application.
6.	The role of the database: This is Mysql, which will store the website's data.
7.	The server used to communicate with the computer of the user requesting the website is the HTTP protocol, which communicates with the user's computer requesting the website. The web server will receive the user's request via HTTP, process it and respond with the appropriate web pages 




ISSUES WITH THE INFRASTRUCTURE
1.	SPOF: This particular web infrastructure relies on a single server, it is a **Single Point Of Failure** (SPOF). If the server goes down, the website will become unavailable , and users will not be able to connect or access it.
2.	Downtime OR maintenance period: It’s just like deploying new code web server needs to be restarted, during maintenance or update the server needs to be restarted, causing downtime and disrupting access to the website.
3.	Cannot scale if too much incoming traffic: This literally means; whenever the website receives too much traffic, the infrastructure will be unable to handle it, resulting in crashes or slow loading time. Since this infrastructure only has a single server, the scaling options are limited.
*/
