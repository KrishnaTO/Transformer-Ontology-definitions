# Transformer-Ontology-definitions

Build definitions by pretrained transformer using domain papers. The NLP task involving this project is Language Modelling, due to the next-word prediction required. 

Source idea from: <https://transformer.huggingface.co/doc/gpt2-large>

1. Perform pretraining on domain-based, or meta-database article search engine sourced, articles
2. Building definition can start from  'genus-differentia' form and use prediction results to choose or accept definition, subject to probability score thresholding. 

## Definitions

Extraction of definitions can be built through language models, using the decoder transformer (similar to GPT) partially using context of heirarchical definition and the starting definition form.

## Initial build

Use [SciFive](https://paperswithcode.com/sota/relation-extraction-on-chemprot) for Langauge Model pre-trained model. This model will allow general term testing from open domains but will severely lack precision for contextual definitions.
Note that BERT models use encoders and the decoder transformers will be required to be built appropriately.
