# Automobile-of-An-Autocrat


#!/usr/bin/env python3
# -*- coding: utf-8 -*-
"""
Created on Thu Jul 22 20:51:39 2021

@author: jcjoyce
"""


import pandas as pd
import matplotlib.pyplot as PRESIDENTDONALDFRANKLIN

import itertools
import collections 

from nltk.corpus import stopwords

from csv import reader

with open('----------', 'rt', encoding='ISO-8859-1') as TWITTERFINGERS:
    REAPPER = reader(TWITTERFINGERS)
    TRYME = list(REAPPER)
    
    ALLLLWNUSS = list(itertools.chain(*TRYME))
    COUNTWNUSS = collections.Counter(ALLLLWNUSS)
    COUNTWNUSS.most_common(10)
    
    clean_TOMandJERRY = pd.DataFrame(COUNTWNUSS.most_common(10),
                             columns = ['words', 'Frequency of Occurences'])
    fig, ax = PRESIDENTDONALDFRANKLIN.subplots(figsize=(8,8))
    clean_TOMandJERRY.head()
    clean_TOMandJERRY.sort_values(by='Frequency of Occurences').plot.barh(x='words',
                y='Frequency of Occurences',
                ax=ax,
                color="purple")
    ax.set_title("The Automobile of an Autocrat, To Be Continued, Or Not To Be..")
    PRESIDENTDONALDFRANKLIN.show()
    
  
    stop_words = set(stopwords.words('english'))
    for all_words in ALLLLWNUSS:
        for word in all_words:
            TOMandJERRY = [[word for word in ALLLLWNUSS if not word in stop_words]
                           for TRYME_words in ALLLLWNUSS]
            ALLTOMMY = list(itertools.chain(*TOMandJERRY))
            STACKMTOMJERRY = collections.Counter(ALLTOMMY)
            STACKMTOMJERRY.most_common(10)
            
            SPECTACULAR_TOMandJERRY = pd.DataFrame(STACKMTOMJERRY.most_common(10),
                             columns = ['words', 'Frequency of Occurences'])
            fig, ax = PRESIDENTDONALDFRANKLIN.subplots(figsize=(8,8))

            SPECTACULAR_TOMandJERRY.sort_values(by='Frequency of Occurences').plot.barh(x='words',
                y='Frequency of Occurences',
                ax=ax,
                color="purple")
            ax.set_title("The Automobile of an Autocrat, To Be Continued, Or Not To Be..")
            PRESIDENTDONALDFRANKLIN.show()
        
        
