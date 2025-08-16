# URL Discovery:
  ### gau - getallurls:
    https://github.com/lc/gau  -> getallurls (gau) fetches known URLs from AlienVault's Open Threat Exchange, the Wayback Machine, Common Crawl, and URLScan for any given domain. Inspired by Tomnomnom's waybackurls.
  
  ### httpx:
    https://github.com/projectdiscovery/httpx  -> httpx is a fast and multi-purpose HTTP toolkit that allows running multiple probes using the retryablehttp library.

### example: 
    cat list.txt | httpx -silent | gau  -> enumerate subdomains from the list -> which has active webservers -> which URL are active in it subdomain
    subfinder -d example.com -silent | httpx -silent | gau   -> enumerate subdomains -> which has active webservers -> which URL are active in it subdomain
  
