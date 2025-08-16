#### securitytrails 
    https://securitytrails.com/

#### Open Source tools:
    host <example.com> -> it presents the ip address of the website that you are looking for
    host <subdomain.example.com> -> it presents the ip address of the subdomain that you are looking for

  #### Sublist3r:
    https://github.com/aboul3la/Sublist3r
    python3 sublist3r.py -d example.com  -> To enumerate subdomains of specific domain
    python3 sublist3r.py -e google,yahoo,virustotal -d example.com  -> To enumerate subdomains and use specific engines such Google, Yahoo and Virustotal engines
    python sublist3r.py -b -d example.com  -> To enumerate subdomains and enable the bruteforce module

  #### subfinder:
    https://github.com/projectdiscovery/subfinder
    ./subfinder -d example.com  -> To enumerate passively the subdomains of a specific domain
    It is possible to increase the passive research by adding your API Keys to the /subfinder/config.yaml file
    https://chaos.projectdiscovery.io/ -> bug bounty database which you can search for specific domains 
    
  #### Subbrute:
    https://github.com/TheRook/subbrute
    python3 subbrute.py example.com  -> To enumerate subdomains of a specific domain
    python3 subbrute.py -t list.txt  -> To enumerate multiple subdomains from a list of domains
    python3 subbrute.py 
    
  #### crt.sh:
    https://crt.sh  
    https://crt.sh/?q=example.com  -> To search for all the certificates example.com had/has, it helps identify subdomains passively
    
  #### CTFR:
    https://github.com/UnaPibaGeek/ctfr
    python3 ctfr.py -d example.com  -> Generate a list of all the subdomains that had a valid certificate from the website that you are looking at
  
  

    
