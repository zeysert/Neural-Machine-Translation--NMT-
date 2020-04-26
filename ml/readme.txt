Neural machine translation (NMT) is an approach to machine translation that uses an artificial neural network to predict the likelihood of a sequence of words, typically modeling entire sentences in a single integrated model.

NMT departs from phrase-based statistical approaches that use separately engineered subcomponents.Neural machine translation (NMT) is not a drastic step beyond what has been traditionally done in statistical machine translation (SMT). Its main departure is the use of vector representations ("embeddings", "continuous space representations") for words and internal states. The structure of the models is simpler than phrase-based models. There is no separate language model, translation model, and reordering model, but just a single sequence model that predicts one word at a time. However, this sequence prediction is conditioned on the entire source sentence and the entire already produced target sequence. NMT models use deep learning and representation learning.

The word sequence modeling was at first typically done using a recurrent neural network (RNN). A bidirectional recurrent neural network, known as an encoder, is used by the neural network to encode a source sentence for a second RNN, known as a decoder, that is used to predict words in the target language.Recurrent neural networks face difficulties in encoding long inputs into a single vector. This can be compensated by an attention mechanism which allows the decoder to focus on different parts of the input while generating each word of the output. There are further Coverage Models addressing the issues in such attention mechanisms, such as ignoring of past alignment information leading to over-translation and under-translation.

Convolutional Neural Networks (Convnets) are in principle somewhat better for long continuous sequences, but were initially not used due to several weaknesses. These were successfully compensated for in 2017 by using "attention mechanisms".

A attention-based model, the transformer architecture remains the dominant architecture for several language pairs.





Deep learning applications appeared first in speech recognition in the 1990s. The first scientific paper on using neural networks in machine translation appeared in 2014, followed by a lot of advances in the following few years. (Large-vocabulary NMT, application to Image captioning, Subword-NMT, Multilingual NMT, Multi-Source NMT, Character-dec NMT, Zero-Resource NMT, Google, Fully Character-NMT, Zero-Shot NMT in 2017) In 2015 there was the first appearance of a NMT system in a public machine translation competition (OpenMT'15). WMT'15 also for the first time had a NMT contender; the following year it already had 90% of NMT systems among its winners.