# RankProt
Relative ranking method to predict protein thermostability from protein .pdb structures

The rankprot tool runs best in Linux due to the requirement of the third party software VADAR which runs with f77 compiler.

1. Need to install f77 compiler.
2. install python 3.4.1 and install it giving the path to rankprot folder. 
3. install promotif by typing sh makefilelinux3
4. install vadar by ./Install. It will ask for path so give 
1) /usr/local/bin -> /home/your directory/Desktop/bin
2) /usr/local/lib -> /home/your directory/Desktop/lib

5. Open the rankprot folder.
6. Change the path of vadar and promotif in rankprot.bash.
7. Other files that are required for the software to run are protein.py, parsing_vadar.py and parsing_promotif.py, rank_parser.py have been provided.
8. There are pdb format files in this folder, 1i6w.pdb as an example case.
9. Now in terminal, go to the rankprot folder and type.
./rankprot.bash 1i6w.pdb 1i6w.pdb.

10. On asking for option press 1. 
11. This should calculate and make 1.txt and 2.txt and multiply it with eigen.txt and give ranks in rank.txt.
