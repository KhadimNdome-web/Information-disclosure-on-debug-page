# Information-disclosure-on-debug-page
I opened the website `(https://0ad8008b048b474cd15aef9200b800e0.web-security-academy.net)`, logged into my Windows Console and intalled Feroxbuster, which is particularly usedul in finding more files or directories by appending possible file names or directories at the end of the given url, facilitating and accelerating the finding of files that can lead to vulnerabilities.

I also downloaded a wordlist of all possible file names and directories that can be appended to the website URL, and that can consequently be searched thorugh Feroxbuster,then saved it as a text-file and named it `common.txt`

I ran Linux from my Command line and typed in the code `./feroxbuster -u https://0ad8008b048b474cd15aef9200b800e0.web-security-academy.net -w Desktop/common.txt`.

The command Line procedeed to list me all possible file names and directories given the chosen wordlist from `common-txt`. 

After analazing the file names, i decided to open the file `https://0ad8008b048b474cd15aef9200b800e0.web-security-academy.net/cgi-bin` which led to a file named `phpinfo.php`, and subsequently opening a Tab with sensitive and detailed information about the PHP environment that the server is using, thus representing a security risk.

