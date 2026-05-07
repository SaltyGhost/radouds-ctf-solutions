```sh
casper@casper-V5-171:~/Desktop/picoctf$ git clone ssh://git@foggy-cliff.picoctf.net:63795/git/challenge.git
Cloning into 'challenge'...
The authenticity of host '[foggy-cliff.picoctf.net]:63795 ([3.15.249.208]:63795)' can't be established.
ED25519 key fingerprint is SHA256:Grm7IvZgdCDbXv3DtQ70/6WKHA2q3XhT+sfva8nLT38.
This host key is known by the following other names/addresses:
    ~/.ssh/known_hosts:19: [hashed name]
Are you sure you want to continue connecting (yes/no/[fingerprint])? yes
Warning: Permanently added '[foggy-cliff.picoctf.net]:63795' (ED25519) to the list of known hosts.
git@foggy-cliff.picoctf.net's password: 
remote: Enumerating objects: 3, done.
remote: Counting objects: 100% (3/3), done.
remote: Compressing objects: 100% (2/2), done.
remote: Total 3 (delta 0), reused 0 (delta 0)
Receiving objects: 100% (3/3), done.
casper@casper-V5-171:~/Desktop/picoctf$ cd challenge/
casper@casper-V5-171:~/Desktop/picoctf/challenge$ echo 123 > flag.txt 
casper@casper-V5-171:~/Desktop/picoctf/challenge$ git config user.name "root"
casper@casper-V5-171:~/Desktop/picoctf/challenge$ git config user.email "root@picoctf"
casper@casper-V5-171:~/Desktop/picoctf/challenge$ git add flag.txt 
casper@casper-V5-171:~/Desktop/picoctf/challenge$ git commit -m "rrrr"
[master 737504b] rrrr
 1 file changed, 1 insertion(+)
 create mode 100644 flag.txt
casper@casper-V5-171:~/Desktop/picoctf/challenge$ git push
git@foggy-cliff.picoctf.net's password: 
Enumerating objects: 4, done.
Counting objects: 100% (4/4), done.
Delta compression using up to 4 threads
Compressing objects: 100% (2/2), done.
Writing objects: 100% (3/3), 261 bytes | 261.00 KiB/s, done.
Total 3 (delta 0), reused 0 (delta 0), pack-reused 0
remote: Author matched and flag.txt found in commit...
remote: Congratulations! You have successfully impersonated the root user
remote: Here's your flag: picoCTF{1mp3rs0n4t4_g17_345y_506743df}
To ssh://foggy-cliff.picoctf.net:63795/git/challenge.git
   1f391cc..737504b  master -> master
casper@casper-V5-171:~/Desktop/picoctf/challenge$
```
