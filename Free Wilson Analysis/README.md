## Free Wilson Analysis : Promising substituents and their promosing combinations that contribute to or detract from activity

How often have you been in this situation?  You're working on a drug discovery project, you're in mid to late lead optimization, and you're wondering "what have we missed".  "Are there promising combinations of substituents that we didn't synthesize"? Wouldn't it be great if you could look at all the substituent combinations that you didn't make, and identify the combinations that appear promising?
Wow, you ask, what is this snazzy new technique?  Actually, it's not a new technique, it's Free-Wilson analysis, which was originally published in 1964.  The method is pretty simple and can be illustrated through an example like the one in a 1998 review by Hugo Kubinyi.

PAT WALTERS's bolg:

[link](https://practicalcheminformatics.blogspot.com/2018/05/free-wilson-analysis.html)

1. R group decomposition (free_wilson.py rgroup) : r goups file and vector of molecules file
2. Regression (free_wilson.py regression) : Vectors can be used to regress against biological activity values and obtain coefficients the quantify the contributions of particular substituents to biological activity.
3. Enumeration (free_wilson.py enumeration) : Generates all possible combinations of the available substituents. 
