== Post-EMNLP15 submission notes == 
kduh 7/24/2015

Acknowledgments: Prof. Matsumoto, Shindo, Neubig for comments

Typos: 
- Eq. 1: - lambda or + lambda

Clarification needed:
- Sec 3.3. may not be clear about using UAS

---- Comments from Prof. Shindo -----
- If a reviewer knows NN-based dependency parsing and LSTM, I think it is easy for him to understand what you've done in the paper.
- If there is a reason why you use a Web Treebank (not Penn Treebank) as evaluation data, you should describe it. The benchmark test for dependency parsing is usually done on Penn Treebank.
- In experiment, it is better to describe your parser's decoding is based on greedy-search (not beam-search).
- Have you confirmed your re-implementation of baseline parser successfully reproduced Chen and Manning's results?
- You should discuss more about the results in Table 1. In particular, there is no discussion about Web domains results (Answers, Emails, etc.). Since it seems there's no big differences between LSTM and non-LSTM, you need some excuse.

----- Comments from Prof. Neubig -----
It seems pretty nice! It seems like a pretty reasonable paper, and I would probably give it a 4. Knowing that dropout works better than L2 is a nice insight.
But here are grumpy reviewer comments, just in case. Note that I have ideas about some of them, but it's not stated clearly in the paper so there might be comments?

1) Why is the accuracy on WSJ so low? WSJ accuracy for state-of-the-art parsers is 92-93.

2) Why is the feed-forward network better for short term dependencies? This is not stated clearly.

3) There is an improvement in long-term dependencies, but so what? Attachment score is what matters.


