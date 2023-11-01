**TASK**


In my role as a security professional at a healthcare company, part of my responsibility involves maintaining an updated list that specifies which employees are authorized to access restricted content, particularly those handling personal patient records. This authorization is tied to their IP addresses, with an allow list designating which IP addresses are granted access to the restricted subnetwork. Additionally, there's a remove list that specifies which employees need to be removed from this allow list.

My current assignment requires me to develop a Python algorithm that can effectively cross-check the allow list against the remove list. If any of the IP addresses on the remove list match those on the allow list, I need to programmatically remove those corresponding IP addresses from the file that contains the allow list. This process ensures that only authorized personnel retain access to the restricted content, in line with our security protocols.

In order to complete this task i did the following;

1. I accessed a specific file named "allow_list.txt." To do this, I assigned the file name to a string variable called 'import_file.' Subsequently, I utilized a 'with' statement to open this file and store it in a variable named 'file.' This way, I can efficiently work with the contents of the file while operating within the scope of the 'with' statement.

2. I proceeded by employing the .read() method, which will enabled me to transform the contents of the allow list file into a string, making them readable. These converted contents was stored in a variable, which i'll call 'ip_addresses.'

3. To facilitate the removal of individual IP addresses from the allow list, it's essential to have these addresses in a list format. For this purpose, i used the .split() method, which will transform the 'ip_addresses' string into a list format.

4. There was a second list called 'remove_list,' which holds all the IP addresses that must be eliminated from the 'ip_addresses' list. So, i established the loop structure by setting up the header of a 'for' loop that will cycle through the 'remove_list.' I used the variable 'element' as the looping variable.

5. In the body of your iterative statement, i added code that will remove all the IP addresses from the allow list that are also on the remove list. First, i created a conditional that evaluates if the loop variable element is part of the ip_addresses list. Then, within that conditional, i applied the .remove() method to the ip_addresses list and removed the IP addresses identified in the loop variable element.

6. After removing the IP addresses from the ip_address variable, i completed the algorithm by updating the file with the revised list. To do this, i first converted the ip_addresses list back into a string using the .join() method. I applied .join() to the string "\n" in order to separate the elements in the file by placing them on a new line. Then, i used another with statement and the .write() method to write over the file assigned to the import_file variable.

7. Finf the report of this file attached in the directory.
