# malware bazaar downloader
![malware bazaar dowloader](mb-download.png)

quick and dirty ansible playbook to download and extract recent malware samples from abuse.ch's malware bazaar
# --WARNING--
this script will download and extract actual malware samples. you have been warned
## usage
tested on ubuntu 24.04
- install ansible
- clone repo
- update download_malware.yml with your abuse.ch API key
- run
``ansible-playbook download_malware.yaml`` from mb-download directory
## note
by default the playbook downloads all samples from the last 24 hours

