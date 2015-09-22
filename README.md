# shell-commands


#### Find  

**Recursivly change files extension**  
Rename recursively all files in the current directory changing the extension from ext1 to ext2.  
`find . -name "*.ext1" -exec rename -v 's/\.ext1$/.ext2/' '{}' \;`
