<h1 align="center">
 𝓟𝓨𝓞𝓢𝓘𝓝𝓣 
 </h1>

<p align="center">
<img src="https://img.shields.io/badge/license-GPL-blue">
 <img src="https://camo.githubusercontent.com/8a6b52f917c9d3391417f3a2b2727b918b425564e54609efe81c58fef6b084e2/68747470733a2f2f696d672e736869656c64732e696f2f62616467652f706c6174666f726d2d57696e646f77732532302537432532304c696e75782d79656c6c6f77">
 <img src="https://img.shields.io/badge/Python-3-brightgreen.svg?style=plastic">
</p>

 <img src ="https://github.com/d8rkmind/datacontainer/blob/main/data/gif/Pyosint.gif" width=2160px>

<p><b>Subdomain</b> enumeration,Web scraping and finding usernames automation script written in python
<br></p>
<h2>Installation</h2>

```markdown
cd PyOsint
pip3 install -r requirements.txt
```
<b>Usage :</b>

```
python3 Pyosint.py [OPTIONS]
```
## Brief info: 

The main functionality of this program has been divided to 3 parts
 <br>
 * Find - Module to search For usenames form a list of <b><i>326</i></b> websites
 * Scrap - To Scrap a website to extract all links form a given website and store it in a file
 * Enum - To automate the search of subdomains of a given domain from diffrent services
 
 In Scrap module results are automatically stored in <i> output/web </i> folder wit he ip-address of the website as the filename <br><br>
 The services used are<i> <b> Virus Total,PassiveDns,CrtSearch,ThreatCrowd</i> </b> <br>
<b> Enum </b> module an Api key of <b>Virus total</b> that you can get from going <a href="https://www.virustotal.com/gui/sign-in"> Here </a><br>

<img src = "https://github.com/d8rkmind/datacontainer/blob/main/data/pictures/mceclip0.png" width=1080p>
<img src = "https://github.com/d8rkmind/datacontainer/blob/main/data/pictures/Untitled.png" width=1080p>

<b>Paste</b> the key inside the curly bracket inside api.json file:

<img src ="https://raw.githubusercontent.com/d8rkmind/datacontainer/main/data/pictures/Screenshot%20at%202021-09-16%2016-07-42.png" width=1080p>

<i> * if this step is not done Virus total may block your request</i>



<h2>Command Line Utilization Information.</h2>
The following are the sub-commands that work this program<br>

Arguments |Shot<br>form |Long<br>form| Functionality
----------|-- | ----|---------
 Name| -n| --name| To specify the domain name or username to use 
 Module| -m| --module| To specify which module to use
 Output | -o| --output| To specify outputfile name
 Thread | -t| --threads | To specify the number of threads to use<br> <i> [ Not applicable to web crawling ] </i> 
 Limit| -l | --limit| to specify the maxium value of web urls to crawl<br><i> [ Applicable only to web crawling ] </i>
 Verbose| -v| --verbose| To enable verbose mode <br><i>[ Applicable only to Enumeration ]</i>
 Ports| -p| --ports| To specify the ports to scan<br><i> [ Applicable only to Enumeration ]</ii>
 Help | -h| --help| To Show the help options
 <br>
 
 #### Example :
 
 ###### Linux commands:
 ``` 
 python3 pyosint.py -m find -n exampleuser               <-- Username-huntdown
 
 python3 pyosint.py -m scrap -n http://scanme.nmap.org   <-- Scrapping using bot
 
 python3 pyosint.py -m enum -n google.com                <-- Subdomain enum  
 ```
  
 <br>
 The project is still in development and will be added with additional functionality.<br>Happy to hear suggestions for improvement.
 
<br>Special Thanks to <a href="https://github.com/technoreck"> 𝓣𝓮𝓬𝓱𝓷𝓸𝓻𝓮𝓬𝓴</a> and <a href ="https://github.com/Shunux-Stuxnet">𝓢𝓱𝓾𝓷𝓾𝔁 - 𝓢𝓽𝓾𝔁𝓷𝓮𝓽</a> For working on this project 


<h2>License :</h2>
Pyosint is licensed under the GNU GPL license. take a look at the <a href="https://github.com/d8rkmind/PyOsint/blob/main/LICENSE">LICENSE</a> for more information


<h2>Update informations</h2>

<h3> Update on 18-8-21:</h3>
Rewritten the code completely ,Improved interface

<h3> Update on 20-8-21:</h3> 
Subdomain enumeration module (enum) has been added

<h3> Update on 23-8-21:</h3>
<p>
Find module code that has been optimised. The number of sites to automate has grown from 14 to 147, and  connection error has been resolved.</p>

<h3> Update on 16-09-21:</h3>

* Porgram has been re-written to work with arguments 
* Find module has been added threading Functionality
* Output functionality has been added to every module 
* More Error handiling has been added
* Number of sites has been increased from 147 to 326
* Cross platform portable 
* Reduced unused and unwanted codes codes 
* Removed console mode 
