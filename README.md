# gnltests

A basic script to test the mandatory part of GNL.

To run it :

- git clone the repo in your GNL folder
- cd to the repo
- Check that the ".h" included in the main match the name of your ".h" file 
- run ./mytest.sh $1 $2 $3
- $1 must be replaced by the BUFFER_SIZE of your choice
- $2 must be replaced by the number of the test files of your choice (here from 1-7)
- $3 can be replaced by any command of your choice, i use to replace it by "valgrind" or "time"

This test will call your GNL until EOF is encountered (in fact while GNL returns something).
The output of your GNL will be written in a diff.txt and a diff is execute to let you know of any differencies between original file and your output.

You can modify/add test files at your taste (i didn't think of much cases ;) ). For the script to still run, you must respect the following nomenclature naming your files : test(number).txt

This script doesn't guarantee the success of your project in any way. It was solely written to help me test during the elaboration of my GNL

Feel free to use during evaluations/elaboration of your code but keep in mind that it is really basic an that an error running it is in no way a good reason to mark a project 0/ consider your project as false.
