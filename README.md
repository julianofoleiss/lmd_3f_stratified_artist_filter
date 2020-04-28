# Stratified 3-fold artist-filtered cross-validation split for the LMD Dataset

This repository contains a 3-fold cross-validation split of the LMD Dataset. It contains a subset of 1300 songs from the 3227 in the original dataset. This split was created by hand by Yandre Costa and passed on to me for my PhD studies. It has been used in [this](http://www.inf.ufpr.br/lesoliveira/download/ASOC2017.pdf) paper and [this](https://www.researchgate.net/profile/Loris_Nanni/publication/283038767_Combining_visual_and_acoustic_features_for_music_genre_classification/links/59e52e060f7e9b0e1aa8897b/Combining-visual-and-acoustic-features-for-music-genre-classification.pdf) paper. It complies to the following rules:

* Applies an artist filter: making sure that, for a given fold, no songs from the same artist are on the training and the test sets at the sime time.


## f*_train.txt files

These files contain the lists of the files that should be used to train the predictive models. The format is the following:

> song_file\\tgenre\\n

## f*_test.txt files

These files contain the lists of files that should be used to test the predictive models. The format is the following:

> song_file\\n

## f*_evaluate.txt files

These files contain the exact same list of files of the correspondent test file, except that they also contain the ground-truth:

> song_file\\tgenre\\n

If you use this split, please cite the following paper:

> @article{FOLEIS2020106127,
> title = "Texture selection for automatic music genre classification",
> journal = "Applied Soft Computing",
> volume = "89",
> pages = "106127",
> year = "2020",
> issn = "1568-4946",
> doi = "https://doi.org/10.1016/j.asoc.2020.106127",
> url = "http://www.sciencedirect.com/science/article/pii/S1568494620300673",
> author = "Juliano Henrique Foleis and Tiago Fernandes Tavares",
> keywords = "Music genre classification, Sound texture selection, Music classification, Signal processing, Music information retrieval",
> }

Thanks to Yandre Costa for supplying me with this split.

Cheers!

Juliano

Lecturer @ Universidade Tecnologica Federal do Parana (Campo Mourao, PR, Brazil) 

PhD Candidate @ UNICAMP (Campinas, SP, Brazil)

julianofoleiss *at* utfpr *dot* edu *dot* br


