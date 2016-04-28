# shell-commands


#### Find  

**Recursivly change files extension**  
Rename recursively all files in the current directory changing the extension from ext1 to ext2.

`find . -name "*.ext1" -exec rename -v 's/\.ext1$/.ext2/' '{}' \;`


**Count files in subdirectories**  
Count the number of files inside each directory

`find */ | cut -d/ -f1 | uniq -c`


#### SSH
**Login without password**  

`cat .ssh/id_rsa.pub | ssh b@B 'cat >> .ssh/authorized_keys'`


**Reverse tunnel**

`ssh -Ntg -R <serverport>:localhost:<localport> <serveruser>@<server.domain>`
