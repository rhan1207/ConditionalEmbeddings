# ConditionalEmbeddings
Estimate conditional word embedding distributions with Bayes-by-Backprop



Step 1: Data Processing
        a) run create_dictionary.py to create a dictionary by frequency rank (vocab.npy) and a dictionary by counts (vocab_f.npy).
	b) run down_sample.py to select only top K vocabulary and down-sample raw text corpus according to Mikolov et al, 2013. This step produces the final vocabulary: vocab_freq.npy and file text corpus: *_freq.txt

Step 2:
        Run main.py to estimate the model. Conditional Bayes-by-Backprop model implemenation is in the BBP.py file. This step will save the best model object for downstream analysis
	
	
EMNLP 2018 Publication: http://aclweb.org/anthology/D18-1527
