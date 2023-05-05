Download Link: https://assignmentchef.com/product/solved-cse5334-assignment-3-prominentstreak
<br>
<h2></h2>

You code should accomplish the following tasks:

<ul>

 <li><strong>Read</strong> the text file 1991-2004-nba.dat. In this file, each line is the boxscore of an NBA player in an NBA game. The records are already sorted by players and then by dates, i.e., all the boxscores of a player are in consecutive rows, in chronological order.</li>

</ul>

You only need to use the first column (player ID) and the last column (number of points by the player in a game) of this file.

We provide a skeleton file “P3_skeleton.py” to you. It already has the code for reading from the data file.

<ul>

 <li><strong>Compute</strong> the prominent streaks in this dataset. For each player, the sequence has all the points the player made in his games. There are multiple sequences, one for each player. Each prominent streak is a subsequence of a player’s sequence. It must not be dominated by any other streak in any player’s sequence.</li>

</ul>

For the concepts and algorithms of prominent streaks, refer to our lecture vidoes, slides, as well as the following two papers.

Xiao Jiang, Chengkai Li, Ping Luo, Min Wang, and Yong Yu. Prominent Streak Discovery in Sequence Data. In Proceedings of the 17th ACM SIGKDD International Conference on Knowledge Discovery and Data Mining (KDD), pages 1280-1288, San Diego, California, USA, August 2011.

<a href="http://ranger.uta.edu/~cli/pubs/2011/streak-kdd11-jllwy-jun11.pdf">(</a><u><a href="http://ranger.uta.edu/~cli/pubs/2011/streak-kdd11-jllwy-jun11.pdf">http://ran</a></u><a href="http://ranger.uta.edu/~cli/pubs/2011/streak-kdd11-jllwy-jun11.pdf">g</a><u><a href="http://ranger.uta.edu/~cli/pubs/2011/streak-kdd11-jllwy-jun11.pdf">er.uta.edu/~cli/pubs/2011/streak-kdd11-</a></u><a href="http://ranger.uta.edu/~cli/pubs/2011/streak-kdd11-jllwy-jun11.pdf">j</a><u><a href="http://ranger.uta.edu/~cli/pubs/2011/streak-kdd11-jllwy-jun11.pdf">llw</a></u><a href="http://ranger.uta.edu/~cli/pubs/2011/streak-kdd11-jllwy-jun11.pdf">y</a><u><a href="http://ranger.uta.edu/~cli/pubs/2011/streak-kdd11-jllwy-jun11.pdf">-jun11.pdf </a></u><a href="http://ranger.uta.edu/~cli/pubs/2011/streak-kdd11-jllwy-jun11.pdf">(</a><u><a href="http://ranger.uta.edu/~cli/pubs/2011/streak-kdd11-jllwy-jun11.pdf">http://ran</a></u><a href="http://ranger.uta.edu/~cli/pubs/2011/streak-kdd11-jllwy-jun11.pdf">g</a><u><a href="http://ranger.uta.edu/~cli/pubs/2011/streak-kdd11-jllwy-jun11.pdf">er.uta.edu/~cli/pubs/2011/streakkdd11-</a></u><a href="http://ranger.uta.edu/~cli/pubs/2011/streak-kdd11-jllwy-jun11.pdf">j</a><u><a href="http://ranger.uta.edu/~cli/pubs/2011/streak-kdd11-jllwy-jun11.pdf">llw</a></u><a href="http://ranger.uta.edu/~cli/pubs/2011/streak-kdd11-jllwy-jun11.pdf">y</a><u><a href="http://ranger.uta.edu/~cli/pubs/2011/streak-kdd11-jllwy-jun11.pdf">-jun11.pdf)</a></u><a href="http://ranger.uta.edu/~cli/pubs/2011/streak-kdd11-jllwy-jun11.pdf">)</a>

Gensheng Zhang, Xiao Jiang, Ping Luo, Min Wang, and Chengkai Li. Discovering General Prominent Streaks in Sequence Data. In ACM Transactions on Knowledge Discovery from Data (TKDD), 8(2): 9:1-9:37, June 2014. <a href="http://ranger.uta.edu/~cli/pubs/2014/streak-tkdd-jllwy-sept13.pdf">(</a><u><a href="http://ranger.uta.edu/~cli/pubs/2014/streak-tkdd-jllwy-sept13.pdf">http://ran</a></u><a href="http://ranger.uta.edu/~cli/pubs/2014/streak-tkdd-jllwy-sept13.pdf">g</a><u><a href="http://ranger.uta.edu/~cli/pubs/2014/streak-tkdd-jllwy-sept13.pdf">er.uta.edu/~cli/pubs/2014/streak-tkdd-</a></u><a href="http://ranger.uta.edu/~cli/pubs/2014/streak-tkdd-jllwy-sept13.pdf">j</a><u><a href="http://ranger.uta.edu/~cli/pubs/2014/streak-tkdd-jllwy-sept13.pdf">llw</a></u><a href="http://ranger.uta.edu/~cli/pubs/2014/streak-tkdd-jllwy-sept13.pdf">y</a><u><a href="http://ranger.uta.edu/~cli/pubs/2014/streak-tkdd-jllwy-sept13.pdf">-sept13.pdf </a></u><a href="http://ranger.uta.edu/~cli/pubs/2014/streak-tkdd-jllwy-sept13.pdf">(</a><u><a href="http://ranger.uta.edu/~cli/pubs/2014/streak-tkdd-jllwy-sept13.pdf">http://ran</a></u><a href="http://ranger.uta.edu/~cli/pubs/2014/streak-tkdd-jllwy-sept13.pdf">g</a><u><a href="http://ranger.uta.edu/~cli/pubs/2014/streak-tkdd-jllwy-sept13.pdf">er.uta.edu/~cli/pubs/2014/streaktkdd-</a></u><a href="http://ranger.uta.edu/~cli/pubs/2014/streak-tkdd-jllwy-sept13.pdf">j</a><u><a href="http://ranger.uta.edu/~cli/pubs/2014/streak-tkdd-jllwy-sept13.pdf">llw</a></u><a href="http://ranger.uta.edu/~cli/pubs/2014/streak-tkdd-jllwy-sept13.pdf">y</a><u><a href="http://ranger.uta.edu/~cli/pubs/2014/streak-tkdd-jllwy-sept13.pdf">-sept13.pdf)</a></u><a href="http://ranger.uta.edu/~cli/pubs/2014/streak-tkdd-jllwy-sept13.pdf">)</a>

<h2>2. Expected Output</h2>

Your code should return the following results. Each prominent streak should be displayed in the format of (player ID, beginning index of the streak, length of the streak, minimum value in the streak). The beginning index provides the position of the left end of the streak. In a player’s seequence, the index of the first element is 0.

Note that the prominent streaks in the output can be in any order, depending on the particular way an implementation finds the prominent streaks.

In a typical run, our solution code finishes computing prominent streaks in less than half a second on our computer. (Reading the data file itself takes 20-30 seconds.) When we test your code on the same computer, your code is expected to achieve the same efficiency, in order to be considered efficiently implemented. Note that an implementation of the brute-force baseline method took several mminutes to finish.

In [ ]: Reading the data file takes  22.284526109695435  seconds.

Computing prominent streaks takes  0.49631690979003906  seconds.

[(‘BRYANKO01’, 457, 4, 42), (‘BRYANKO01’, 457, 9, 40), (‘BRYANKO01’, 453 , 13, 35), (‘BRYANKO01’, 453, 14, 32), (‘BRYANKO01’, 453, 16, 30), (‘IVE RSAL01’, 305, 27, 26), (‘IVERSAL01’, 554, 2, 51), (‘IVERSAL01’, 550, 45,

21), (‘IVERSAL01’, 550, 57, 20), (‘JACKSJI01’, 0, 1185, 0), (‘JAMISAN0 1’, 107, 2, 51), (‘JORDAMI01’, 196, 17, 27), (‘MALONKA01’, 176, 159, 14

), (‘MALONKA01’, 72, 263, 13), (‘MALONKA01’, 72, 357, 12), (‘MALONKA01’,  482, 96, 17), (‘MALONKA01’, 459, 119, 16), (‘MALONKA01’, 430, 149, 15),  (‘MALONKA01’, 72, 527, 11), (‘MALONKA01’, 24, 575, 10), (‘MALONKA01’, 2 4, 758, 7), (‘MALONKA01’, 0, 866, 2), (‘MCGRATR01’, 380, 34, 24), (‘ONEA SH01’, 373, 74, 19), (‘ONEASH01’, 353, 94, 18), (‘ONEASH01’, 0, 858, 6),  (‘ROBINDA01’, 229, 1, 71), (‘STOCKJO01’, 0, 932, 1)]