# Fuzzing

  ### Wfuzz:
    https://github.com/xmendez/wfuzz  -> Web application fuzzer
    wfuzz -c -z range,1-100 http://example.com/users.php\?id\=FUZZ  -> -c makes the output colorful -z let you choose between make the scan based on file or RANGE
    wfuzz -c -z file,list.txt http://example.com/FUZZ  -> -c makes the output colorful -z let you choose between make the scan based on FILE or range
    wfuzz -t 10 -c -z file,list.txt --hc 404 http://example.com/FUZZ  -> -t 10 choose 10 threads --hc will hide each one page that present a 404 error 
    wfuzz -t 10 -c -z file,list.txt --sc 200 http://example.com/FUZZ  -> --sc will present only pages with status code 200
  
  ### Ffuf:
    https://github.com/ffuf/ffuf  -> Fast web fuzzer written in Go
    
     
