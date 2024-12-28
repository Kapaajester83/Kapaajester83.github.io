
https://play.picoctf.org/practice/challenge/320?page=2

Description
Unzip this archive and find the file named 'uber-secret.txt'

    Download zip file

CLI

kappa@kappa-Aspire-Z5600:~/Desktop/firstFind/files$ ls
13771.txt.utf-8  acceptable_books  satisfactory_books
14789.txt.utf-8  adequate_books
 
kappa@kappa-Aspire-Z5600:~/Desktop/firstFind/files$ find ./ -name 'uber-secret.txt'
./adequate_books/more_books/.secret/deeper_secrets/deepest_secrets/uber-secret.txt

kappa@kappa-Aspire-Z5600:~/Desktop/firstFind/files$ cat ./adequate_books/more_books/.secret/deeper_secrets/deepest_secrets/uber-secret.txt
picoCTF{f1nd_15_f457_ab443fd1}
kappa@kappa-Aspire-Z5600:~/Desktop/firstFind/files$
