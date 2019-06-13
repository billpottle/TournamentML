# TournamentML
A machine learning model and associated spreadsheet that automatically groups competitors into divisions and prints brackets. 

"Life isn't fair", so martial arts students should train to defeat opponents who are bigger and stronger. However, sports should be fair, so most martial arts tournaments are organized into divisions of similar athletes. 

Large and official tournaments such as the Olympics, national championships, etc set the divisions ahead of time, and athletes will generally cut weight or have to qualify through previous victories, point rankings, etc. 

Local tournaments can use those "regular" divisions, but this often results in a degraded customer experience (for instance, cutting to a lower weight division but no one is there so divisions are combined anyway, 9-10 year olds being grouped together even though their weights are far apart, when the 10 year old could have had a much better division with the 11 year olds, many demo matches or athletes without matches, etc). 

This project uses the K means nearest neighbor in Google Colab to cluster athletes into divisions. The excel sheet also includes related functionality to create division names, and division score sheets (ie, for forms or weapons) as well as single or double elimination brackets. 

When run on data from several previous tournaments, about 90% of the resultant divisions are good, and the other 10% should be adjusted manually before printing brackets. Manual adjustment will likely be much faster than parameter tweaking. 

***
## INSTRUCTIONS

Follow the detailed instructions in the excel file and click on the buttons to launch various blocks of code. 
*** 
## PARAMETERS
You will probably get decent results with the default parameters, but they can be adjusted as needed. When you vary a parameter within a group, it will cause more weight among the group. For instance, the default parameters for skills have Beg(0), Int(5), Adv(10) and Black(20). Since the black belt division has the greatest gap in skill of any division, we want to make sure that is is very unlikely black belts will be paired with other belts. Adjusting the parameters up will also cause other parameters to be given less weight. For instance, if you set the Weight Multiplier at 100, then you will get divisions of very similar weights, even if it has to match males with females or people of vary different ages together. 

