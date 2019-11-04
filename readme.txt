This program can be used to run input text files of medium size. I included two input text files for testing purpose:
- 10000_sample.txt
(contains 10,000 first json strings copied from the given dblp_papers_v11.txt of 12 GB)
- self_sample.txt
(contains 75 self-created json strings to make sure they refer to each other up to tier 2)





## The output of the program: 
   The program will print the result to an output.txt file. Here is an example of the result:

Keyword: computer
n = 2
100027507: Number of times cited 3; Title contains keyword: null
100023113: Number of times cited 1; Title contains keyword: null
100001334: Number of times cited 1; Title contains keyword: yes
100034732: Number of times cited 1; Title contains keyword: null
100019058: Number of times cited 1; Title contains keyword: null
1000153461: Number of times cited 0; Title contains keyword: yes
1000290224: Number of times cited 0; Title contains keyword: yes

- All tier papers ID are listed in the result. 
- Papers that were cited the MOST are the most important and are place at the top.
- The end of the file lists tier0 papers (papers whose title contains the keyword but were not cited by other tier papers).
- "Number of times cited 0; Title contains keyword: yes" usually means tier0 papers as just mentioned above.
- "Title contains keyword: null" means that paper's title does NOT contain the keyword.





## How to run the program:
- In Command Line, cd to the target folder of the maven project (maven-demo/target)
- Use the command "java -jar maven-demo-0.0.1-SNAPSHOT.jar " to run the program
- After running the command above, the program will prompt user to enter the value of n, keyword, and the file name to test.
- The 2 input files (10000_sample.txt and self_sample.txt) can be used for testing purpose.
- The program will print the result to the output.txt file. The output can be compared with the result output files put in the "test_output" folder.
