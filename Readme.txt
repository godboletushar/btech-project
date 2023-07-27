Contents:
Datasets:
	test.csv	Metaphor Novelty Dataset test dataset
	train.csv	Metaphor Novelty Dataset training dataset
	3244ANPs.txt	VSO  (Visual Sentiment Ontology) dataset
	AN-phrase-annotations.csv	ANP dataset by Guiterrez et al.
	Sonnets.txt	Shakespeare's Sonnets
Final outputs:
	Output_all.csv		All word pairs with all adjectives
	Output_limited.csv	Only noun pairs with common adjectives
	Sonnet_relations.csv	Link predictions for each noun pair
	Link_predictions.xlsx	Calculations for link predictions
* Link_predictions.xlsx contains calculations for link predictions as used in the project report. The Sonnet_relations.csv is the output of another execution of the notebook and may not match the link predictions in Link_predictions.xlsx.
--------------------------
Notebooks

Prepare.ipynb
	Input files:
		train.csv
		test.csv
		3244ANPs.txt
		AN-phrase-annotations.csv
		Sonnets.txt
	Output files:
		Output_all.csv		All word pairs with common adjectives for noun pairs
		Output_limited.csv	Only noun pairs with common adjectives
		Sonnet_pairs.csv	Sonnet lines and their nouns
		triples.txt		All triples formed from the noun pairs and their common adjectives


Predict.ipynb
	Input files:
		triples.txt OR (triples_test.txt AND triples_train.txt)
		Sonnet_pairs.csv
	Output_file:
		Sonnet_relations.csv	Link predictions for each noun pair
		

-------------------
Documents

Final presentation:
Final_project_ppt_111903115.pptx

Final project report:
YVH_04.pdf

Readme.txt
-----------------------------------
Execution using Google Colab


1. First, the Prepare.ipynb notebook should be executed.
2. The output files should be downloaded.
3. In the Predict.ipynb notebook, at first, only the first cell should be run (installing Ampligraph). Once that is done, the runtime should be restarted before running the entire notebook.