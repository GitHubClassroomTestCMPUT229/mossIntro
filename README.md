# mossIntro

### Setup
Register with Moss to gain access to submission script  
Registration:  email moss@moss.stanford.edu  
Email body:
registeruser
mail username@domain         | replace username & domain with actual values

Queries: email moss-request@cs.stanford.edu  
moss file should not be made accessible per readme 
Uses Perl.  Installed for my account -> default in configuration?  

### Interface  
Can specify language with -l  
Can specify directories of files using -d  
Can specify base code files with -b        * Must take path to file  
Can specify granularity with -m         * Sets threshold for reporting similar files  
Can specify comment string with -c        * Use this to identify if many queries sent  

Submit all of the ML programs in directories asn1.96/\* and asn1.97/\*, where asn1.97/instructor/example.ml and asn1.96/instructor/example.ml contain the base files.  
moss -l ml -b asn1.97/instructor/example.ml -b asn1.96/instructor/example.ml -d asn1.97/\*/\*.ml asn1.96/\*/\*.ml

Submit all MIPS programs:  
moss -l mips -b \<assignment>/instructor/\<file>.s -d \<assignment>/\*/\*.s  

Run moss on simple files:  
moss -l mips ./simple/*.s  

Run moss on instructorTest:  
moss -l mips -b ./instructorTest/instructor/example.s -d instructorTest/\*/\*.s  
