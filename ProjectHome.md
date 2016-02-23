### fx-http-traffic-generator  v.01 ###

fx-http-traffic-generator was created to respond to the need of those who want to generate a good amount of http traffic.
Depending on the need, different things can be performed with the traffic generated. The idea was born when testing Intrusion Detection System and their resistance to HTTP attacks.
Part of the code I am using was inspired by http://www.javapractices.com/topic/TopicAction.do?Id=147


The main focus of the project are:
  1. Generate HTTP traffic
  1. Test IDS
  1. Take advantage of urlBlacklist
  1. Test Web Application against well known spam databases
  1. Obfuscate URL while passing traffic to leverage a higher test lever of web application and IDS boxes.


---

#### Running the project ####
The project accepts three parameters:


  * `aArgs[0]:` this is the file containing all the domains  and or Urls

  * `aArgs[1]:` (header | content) specifies whether to extract pages hearder or their content

  * `aArgs[2]:` afile - a file name on which all extracted headers/content will be saved.

To run the project, go to the command line (linux, windows, any java enabled OS)


` java -jar WebPageFetcher <aArgs[0]> [header|content] <aArgs[2]> `


---

To do
  * user parallelism to extract more that one header/content at once
  * extract domain/url header at a certain speed
  * obfuscate header request
  * apply more than one obfuscation technique at the same time.
  * accept folder of files i.e. a folder can be passed into parameters instead of passing individual file.


Brought to you by Jules F. Pagna Disso  -- jferdinand-at-gmail-dot-com
You can aslo check my Website at http://www.thescholars.info/