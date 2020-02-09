## What olger does

Olger Nmap D3.js data visualizer and ansible playbook smart generation.

Local python webserver in localhost for graph visualization with D3.js .

Uses www.cvdetails.com to identify Cyber Security Vulnerabilities .

Sends data to elastichsearch and visualizes data in kibana .

Ansible inventory generation, group inventory per software type

Graphviz export, export pdf and .dot files

Shodan api - Cooming soon

## How to plot a network graph

Execute command:

cd olger

chmod +x olger.sh (Just first time)

./olger.sh 192.168.0.1-255 name-mission


Outputs:

  - cvedetails.cve , a csv format with vulneravilities in the network
  - web/graphs/data.json, a compatible D3.js json graph data format
  - reports/reportNameMission.txt, a plaint text data report in txt format
  - web server in port 8000, serving D3.js interactive graph
  - elastsearch with tls support push
  
## How to dump a workless security report

Execute command:

cd olger

chmod +x genreport.sh (Just first time)

./genreport.sh ./web/graphs/data.json name-mission

Outputs:

  -reports/nameMission/namemission.pdf
  -reports/nameMission/namemission.dot

## How it looks

Explore the network with browser view and D3.js Graph

![image olger graph d3 js](olger.png)


Make a plain text report with cvdetails connection

![image olger report vulnerabilities CVE](report.png)


Send data to elastic search and import our Dashboard in KIBANA

![image olger relastic search and kibana](kibana.png)
