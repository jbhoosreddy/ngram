ngram
=====

A software which creates n-Gram (1-5) Maximum Likelihood Probabilistic Language Model with Laplace Add-1 smoothing and stores it in hash-able dictionary form

class nGram
 |  A program which creates n-Gram (1-5) Maximum Likelihood Probabilistic Language Model with Laplace Add-1 smoothing and stores it in hash-able dictionary form.
 |  
 |  Usage:
 |  >>> ng = nGram(True, True, True)
 |  >>> print ng.sentenceprobability('hold your horses', 'bi', 'log')
 |  >>> -18.655540764
 |  
 |  Methods defined here:
 |  
 |  __init__(self, uni=False, bi=False, tri=False, quadri=False, penti=False)
 |      Constructor method which loads the corpus from file and creates ngrams based on imput parameters.
 |  
 |  createBigram(self, words)
 |      Method to create Bigram Model for words loaded from corpus.
 |  
 |  createPentigram(self, words)
 |      Method to create Pentigram Model for words loaded from corpus.
 |  
 |  createQuadrigram(self, words)
 |      Method to create Quadrigram Model for words loaded from corpus.
 |  
 |  createTrigram(self, words)
 |      Method to create Trigram Model for words loaded from corpus.
 |  
 |  createUnigram(self, words)
 |      Method to create Unigram Model for words loaded from corpus.
 |  
 |  loadCorpus(self)
 |      Method to load external file which contains raw corpus.
 |  
 |  probability(self, word, words='', gram='uni')
 |      Method to calculate the Maximum Likelihood Probability of n-Grams on the basis of various parameters.
 |  
 |  sentenceprobability(self, sent, gram='uni', form='antilog')
 |      Method to calculate cumulative n-gram Maximum Likelihood Probability of a phrase or sentence.
