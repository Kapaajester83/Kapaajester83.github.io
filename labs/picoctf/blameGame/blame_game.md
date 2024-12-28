
https://play.picoctf.org/practice/challenge/405?page=2

Description
Someone's commits seems to be preventing the program from working. Who is it? You can download the challenge files here:

    challenge.zip

Hints

In collaborative projects, many users can make many changes. How can you see the changes within one file?

Read the chapter on Git from the picoPrimer here.
https://primer.picoctf.org/#_git_version_control

You can use python3 <file>.py to try running the code, though you won't need to for this challenge.

CLI

kappa@kappa-Aspire-Z5600:~/Desktop/blameGame/drop-in$ git status
On branch master
nothing to commit, working tree clean
kappa@kappa-Aspire-Z5600:~/Desktop/blameGame/drop-in$ git log
commit 83afd3ebd7899251a19d290df92fd1bfc9998adb (HEAD -> master)
Author: picoCTF <ops@picoctf.com>
Date:   Tue Mar 12 00:07:03 2024 +0000

    important business work

commit 760de15c177831fee8b2965e57d1461423ad5ed0
Author: picoCTF <ops@picoctf.com>
Date:   Tue Mar 12 00:07:03 2024 +0000

    important business work


kappa@kappa-Aspire-Z5600:~/Desktop/blameGame/drop-in$ git log message.py 
commit 0351e0474493168ca76441c24630c17554fd09ca
Author: picoCTF{@sk_th3_1nt3rn_d2d29f22} <ops@picoctf.com>
Date:   Tue Mar 12 00:07:01 2024 +0000

    optimize file size of prod code

commit c9e851509190f5887e91339ee18087e3e77ebfda
Author: picoCTF <ops@picoctf.com>
Date:   Tue Mar 12 00:07:01 2024 +0000

    create top secret project
kappa@kappa-Aspire-Z5600:~/Desktop/blameGame/drop-in$

picoCTF{@sk_th3_1nt3rn_d2d29f22}
