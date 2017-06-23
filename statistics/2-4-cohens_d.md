import math
import numpy as np

import thinkstats2
import nsfg

def ReadBirthOrd():
    preg = nsfg.ReadFemPreg()
    live = preg[preg.outcome == 1]
    firsts, others = live[live.birthord == 1], live[live.birthord != 1]
    return firsts, others

def CohenEffectSize(group1, group2):
    diff = group1.mean() - group2.mean()
    
    var1, var2 = group1.var(), group2.var()
    n1, n2 = len(group1), len(group2)
    
    pooled_var = (n1 * var1 + n2 * var2) / (n1 + n2)
    d = diff / math.sqrt(pooled_var)
    return d

g1, g2 = ReadBirthOrd()
print(CohenEffectSize(g1['totalwgt_lb'], g2['totalwgt_lb']))
