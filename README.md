# Summarization-Project

## Goal

> The technique of compressing a piece of text into a shorter version in order to minimize the size of the original text while maintaining vital informative aspects and content significance is known as summarization.
Because text summarizing is a time-consuming and arduous activity, automating it is becoming increasingly popular and acts as a powerful motivation for researchers.
In this repository, we summarized automatically a text from a publicly available text summarizing news item dataset that was collected for Hermann et al (2015). 

## Models used

> In this study we used the The T5 model which was presented in 'Exploring the Limits of Transfer Learning with a Unified Text-to-Text Transformer' by Colin Raffel, Noam Shazeer, Adam Roberts, Katherine Lee, Sharan Narang, Michael Matena, Yanqi Zhou, Wei Li, Peter J. Liu.
T5 is an encoder-decoder model pre-trained on a multi-task mixture of unsupervised and supervised tasks and for which each task is converted into a text-to-text format. T5 works well on a variety of tasks out-of-the-box by prepending a different prefix to the input corresponding to each task, e.g., for translation: and summarization.

## Libraries

> For this study, we used the python language and all the libraries, are mentioned in the ipynb script.

## Dataset 

DatasetDict({
    train: Dataset({
        features: ['document', 'summary'],
        num_rows: 50000
    })
    test: Dataset({
        features: ['document', 'summary'],
        num_rows: 5000
    })
    val: Dataset({
        features: ['document', 'summary'],
        num_rows: 5000
    })
})

