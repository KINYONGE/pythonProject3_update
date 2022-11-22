# pythonProject3_update
Third project for the Engeto Online Python Academy.

Project description
This script is used to retrieve data from the official web pages of the elections to the Chamber of Deputies of the Parliament of the Czech Republic that took place on 20 and 21 October 2017.

Installation of the libraries
The libraries used in this script are listed in the requirements.txt file. For the installation, I recommend to use a virtual environment and to install the python libraries directly from your working environment. For my project, I installed the libraries with my Pycharm work environment. It is comfortable and faster.

pip3 --version
pip3 install -r requirements.txt
Starting the project
To run the script correctly, you need to start the project_3.py file with two mandatory arguments.

python project_3.py <base file reference> <tracking file>

The data is then downloaded from the specified link and saved to a file with a .csv extension.

Example of a project
Voting results for the district of Hradec Králové:

1. argument: https://volby.cz/pls/ps2017nss/ps32?xjazyk=CZ&xkraj=8&xnumnuts=5201
2. argument: results_Hradec_Kralove
  
Execution of the program :

python scraper-election.py "https://volby.cz/pls/ps2017nss/ps32?xjazyk=CZ&xkraj=8&xnumnuts=5201" "vysledky_Hradec_Kralove"

Program flow:

Download data from https://volby.cz/pls/ps2017nss/ps32?xjazyk=CZ&xkraj=8&xnumnuts=5201
Export to the file results_Hradec_Kralove.csv
Completed.
Partial output :

code;location;registered;envelopes;valid;...
569828;Babice;165;109;108;7;1;0;4;0;7;19;3;0;0;1;0;6;0;9;36;0;0;2;1;0;0;12;0
569836;Barchov;227;141;140;21;0;0;9;0;5;16;2;0;2;0;0;19;1;4;46;1;0;3;2;1;1;6;1
...
