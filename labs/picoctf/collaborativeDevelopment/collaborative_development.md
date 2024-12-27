

https://play.picoctf.org/practice/challenge/410?page=2

Description

My team has been working very hard on new features for our flag printing program! I wonder how they'll work together? You can download the challenge files here:

    challenge.zip

Hints

git branch -a will let you see available branches

How can file 'diffs' be brought to the main branch? Don't forget to git config!

CLI

print("w0rk_e4b79efb}")

print("picoCTF{t3@mw0rk_", end='')

print("m@k3s_th3_dr3@m_", end='')

print("w0rk_e4b79efb}")

picoCTF{t3@mw0rk_m@k3s_th3_dr3@m_w0rk_e4b79efb}

kappa@kappa-Aspire-Z5600:~/Desktop/collaborativeDevelopment/drop-in$ ls
flag.py
kappa@kappa-Aspire-Z5600:~/Desktop/collaborativeDevelopment/drop-in$ cat flag.py
print("Printing the flag...")

print("w0rk_e4b79efb}")
kappa@kappa-Aspire-Z5600:~/Desktop/collaborativeDevelopment/drop-in$ git branch
  feature/part-1
  feature/part-2
* feature/part-3
  main
kappa@kappa-Aspire-Z5600:~/Desktop/collaborativeDevelopment/drop-in$ git checkout feature/part-1
Switched to branch 'feature/part-1'
kappa@kappa-Aspire-Z5600:~/Desktop/collaborativeDevelopment/drop-in$ cat flag.py
print("Printing the flag...")
kappa@kappa-Aspire-Z5600:~/Desktop/collaborativeDevelopment/drop-in$ git checkout feature/part-2op-in$ git checkout feature/part-2
Switched to branch 'feature/part-2'
kappa@kappa-Aspire-Z5600:~/Desktop/collaborativeDevelopment/drop-in$ cat flag.py
print("Printing the flag...")

kappa@kappa-Aspire-Z5600:~/Desktop/collaborativeDevelopment/drop-in$ git checkout feature/part-3p-in$ git checkout feature/part-3
Switched to branch 'feature/part-3'
kappa@kappa-Aspire-Z5600:~/Desktop/collaborativeDevelopment/drop-in$ cat flag.py 
print("Printing the flag...")

print("w0rk_e4b79efb}")
kappa@kappa-Aspire-Z5600:~/Desktop/collaborativeDevelopment/drop-in$ 








