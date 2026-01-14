# malware bazaar downloader
![malware bazaar dowloader](images/mb-download.png)

quick and dirty ansible playbook to download and extract recent malware samples from abuse.ch's malware bazaar

https://abuse.ch

https://bazaar.abuse.ch

# --WARNING--
HERE BE DRAGONS - this script will download and extract actual malware samples. use in a segmented lab at your own peril. you have been warned!
## usage
tested on ubuntu 24.04 and ansibe v2.16.3
- install ansible
``` sudo apt-get install ansible```
- clone this repo
``` git clone https://github.com/jreverri/mb-download.git ```
- update download_malware.yml with your abuse.ch API key obtained from https://bazaar.abuse.ch/api/
- run
```ansible-playbook download_malware.yaml``` from mb-download directory
- the script will create a directory called ```malware_samples_ansible``` then download and extract the samples
## note
by default the playbook downloads all samples from the last 24 hours

## please adhear to abuse.ch's ToS

--
Terms of Services (ToS)

By using the website of MalwareBazaar or any of it's services / datasets, you agree that:

All datasets offered by MalwareBazaar can be used for both, commercial and non-commercial purpose for free without any limitations (CC0)

Any data offered by MalwareBazaar is served as it is on best effort with no warranty

MalwareBazaar can not be held liable for any false positives or damage caused by the use of the website or the datasets provided

Any submission to MalwareBazaar will be treated and shared under TLP:CLEAR and under Creative Commons No Rights Reserved (CC0)

It is forbidden to use MalwareBazaar to distribute malware and/or infect any devices for malicious purpose
