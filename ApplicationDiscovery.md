# URL Discovery:
  ### gau - getallurls:
    https://github.com/lc/gau  -> getallurls (gau) fetches known URLs from AlienVault's Open Threat Exchange, the Wayback Machine, Common Crawl, and URLScan for any given domain. Inspired by Tomnomnom's waybackurls.
  
  ### httpx:
    https://github.com/projectdiscovery/httpx  -> httpx is a fast and multi-purpose HTTP toolkit that allows running multiple probes using the retryablehttp library.

#### example: 
    cat list.txt | httpx -silent | gau  -> enumerate subdomains from the list -> which has active webservers -> which URL are active in it subdomain
    subfinder -d example.com -silent | httpx -silent | gau   -> enumerate subdomains -> which has active webservers -> which URL are active in it subdomain
  
# Parameter Discovery:
  ### ParamSpider:
    https://github.com/devanshbatham/ParamSpider   -> Mining URLs from dark corners of Web Archives for bug hunting/fuzzing/further probing 
    paramspider -d example.com -> Discover URLs for a single domain with its parameters
  
  ### Kxss:
    https://github.com/tomnomnom/hacks/tree/master/kxss   -> check if each parameter can reflect the payload 
  
  #### example: 
      paramspider -d example.com | kxss    -> check if each parameter found by paramspider can be reflected by the endpoint, helping to enumerate xss reflected 

  ### Hacks:
    https://github.com/tomnomnom/hacks
    
  ### Parth:
    https://github.com/s0md3v/Parth
    
  ### GF:
    https://github.com/tomnomnom/gf
    
# Content Discovery:
  ### AQUATONE:
    https://github.com/michenriksen/aquatone
    subfinder -d example.com -silent | ./aquatone  -> it will take a screenshot of each subdomain and save to a directory, it will make a html report with the informations obtained 

  ### SecretFinder:
     https://github.com/m4ll0k/SecretFinder   -> A python script for find sensitive data (apikeys, accesstoken,jwt,..) and search anything on javascript files
