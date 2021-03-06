# WORLD - a high-quality speech analysis, manipulation and synthesis system

WORLD is free software for high-quality speech analysis, manipulation and synthesis.
It can estimate Fundamental frequency (F0), aperiodicity and spectral envelope and also generate the speech like input speech with only estimated parameters.

This source code is released under the modified-BSD license.
There is no patent in all algorithms in WORLD.

## Functions for aperiodicity codec were added (2017/03/22)
You can code/decode the aperiodicity. The compression ratio is 1/205 in full-band speech (48 kHz).
In cases where you use the full-band speech, there is no deterioration.
There are examples in examples/codec_test directory.

## Parameter I/O functions were added (2017/03/12)
New files were added in tools directory.
There are examples in examples/parameter_io directory.

## Important notice (2017/01/02)
You can control the fft_size in CheapTrick().
According to this change, arguments in InitializeCheapTrickOption() have changed. Please see test.cpp.

## References
When you cite the latest version of WORLD in your paper, please use the sentence "WORLD \[1\] (D4C edition [2])" and cite the following papers.  
[1] M. Morise, F. Yokomori, and K. Ozawa: WORLD: a vocoder-based high-quality speech synthesis system for real-time applications, IEICE transactions on information and systems, vol. E99-D, no. 7, pp. 1877-1884, 2016.  
[2] M. Morise: D4C, a band-aperiodicity estimator for high-quality speech synthesis, Speech Communication, vol. 84, pp. 57-65, Nov. 2016. http://www.sciencedirect.com/science/article/pii/S0167639316300413  

In CheapTrick, you can refer the following references.  
[3] M. Morise: CheapTrick, a spectral envelope estimator for high-quality speech synthesis, Speech Communication, vol. 67, pp. 1-7, March 2015. http://www.sciencedirect.com/science/article/pii/S0167639314000697  
[4] M. Morise: Error evaluation of an F0-adaptive spectral envelope estimator in robustness against the additive noise and F0 error, IEICE transactions on information and systems, vol. E98-D, no. 7, pp. 1405-1408, July 2015.  

In DIO, you can refer the following reference.  
[5] M. Morise, H. Kawahara and H. Katayose: Fast and reliable F0 estimation method based on the period extraction of vocal fold vibration of singing voice and speech, AES 35th International Conference, CD-ROM Proceeding, Feb. 2009.

In Harvest, I submitted a paper to INTERSPEECH 2017.  
[6] M. Morise: Harvest: A high-performance fundamental frequency estimator from speech signals, in Proc. INTERSPEECH 2017 (submitted).

## Introduction of WORLD family

I introduce useful software in WORLD. If you want to introduce your project in WORLD, please contact me.

PyWorldVocoder (https://github.com/JeremyCCHsu/Python-Wrapper-for-World-Vocoder) is a Python wrapper for World Vocoder.

Note: To avoid making the project complicated, I decided not to merge it to my repository and introduce your project here. The other reason is that I can't support some computer languages.
