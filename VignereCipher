# -*- coding: utf-8 -*-
"""
Created on Mon Feb  5 10:25:18 2024

@author: Caleb Backer-Corthell
"""

import string
get_num = dict()
for index, letter in enumerate(string.ascii_lowercase):
   get_num[letter] = (index + 1) % 26
   
get_let = dict()
for index, letter in enumerate(string.ascii_lowercase):
    get_let[(index +1)%26] = letter
    
    def vin_encrypt(entry,key):
        opt= ""
        for x in range (len(entry)):
            #get number of entry[x]
            #get number of key[x%(len(entry))]
            #add numbers
            #covert back to letter
            #print ("x = ", x)
            #print (g_num (entry[x]))
            cng = g_num(entry[x]) + g_num(key[(x%len(key))%(len(entry))])
            cng = cng % 26
            #print(cng)
            #print(g_let(cng))
            opt = opt + g_let(cng)
            #print (opt)
        
        return opt
            
                                              
                        

    def g_num(entry):
        return get_num[entry]

    def g_let(entry):
        return get_let[entry]
