
https://play.picoctf.org/practice/challenge/371?page=2

Description
Can you make sense of this file? Download the file here.
enc_flag

Hints

Multiple decoding is always good.

CLI

kappa@kappa-Aspire-Z5600:~/Desktop/repetitions$ ls -la
total 16
drwxrwxr-x 2 kappa kappa 4096 Dec 27 16:22 .
drwxr-xr-x 7 kappa kappa 4096 Dec 27 16:18 ..
-rw-rw-r-- 1 kappa kappa  349 Dec 27 16:17 enc_flag
-rw-rw-r-- 1 kappa kappa  185 Dec 27 16:22 repetitions.md
kappa@kappa-Aspire-Z5600:~/Desktop/repetitions$ cat enc_flag
VmpGU1EyRXlUWGxTYmxKVVYwZFNWbGxyV21GV1JteDBUbFpPYWxKdFVsaFpWVlUxWVZaS1ZWWnVh
RmRXZWtab1dWWmtSMk5yTlZWWApiVVpUVm10d1VWZFdVa2RpYlZaWFZtNVdVZ3BpU0VKeldWUkNk
MlZXVlhoWGJYQk9VbFJXU0ZkcVRuTldaM0JZVWpGS2VWWkdaSGRXCk1sWnpWV3hhVm1KRk5XOVVW
VkpEVGxaYVdFMVhSbFZrTTBKeldWaHdRMDB4V2tWU2JFNVdDbUpXV2tkVU1WcFhWVzFHZEdWRlZs
aGkKYlRrelZERldUMkpzUWxWTlJYTkxDZz09Cg==

kappa@kappa-Aspire-Z5600:~/Desktop/repetitions$ cat enc_flag | base64 -d
VjFSQ2EyTXlSblJUV0dSVllrWmFWRmx0TlZOalJtUlhZVVU1YVZKVVZuaFdWekZoWVZkR2NrNVVX
bUZTVmtwUVdWUkdibVZXVm5WUgpiSEJzWVRCd2VWVXhXbXBOUlRWSFdqTnNWZ3BYUjFKeVZGZHdW
MlZzVWxaVmJFNW9UVVJDTlZaWE1XRlVkM0JzWVhwQ00xWkVSbE5WCmJWWkdUMVpXVW1GdGVFVlhi
bTkzVDFWT2JsQlVNRXNLCg==

-SNIP-

kappa@kappa-Aspire-Z5600:~/Desktop/repetitions$ cat enc_flag | base64 -d | base64 -d | base64 -d | base64 -d | base64 -d | base64 -d
picoCTF{base64_n3st3d_dic0d!n8_d0wnl04d3d_73494190}
kappa@kappa-Aspire-Z5600:~/Desktop/repetitions$ 

The name of the challenge is repetition so I kept adding more " | base64 -d " until I found something human readable. In my case it 6 attempts.


