# coursework_protbert

The adaptive immune system helps us to resist the spread and eliminate potentially dangerous pathogens from an organism. This specific activity to pathogens is achieved through immune receptors such as B cell receptors (BCR) and their secreted version antibodies and T cell receptors (TCR). The sum of B cell and T cell receptors is the immune repertoire. The immune repertoire is the language of the immune system and its study would reveal information about antigen specificity, immune history, immune status, and therapeutics. CDR3 is the most variable part of TCR_beta and makes the most significant contribution to the binding to the antigen. There are many Machine Learning and Deep Learning approaches for immune repertoire analysis. But the studies with attention-based model implementations lack.  We take amino acid sequences of CDR3 fragments from TCR_beta and use them as text for a state-of-the-art NLP model for the classification task. We choose ProtBert to obtain embeddings for a further downstream task to classify immune status. Using the BERT model did not yield significant results compared to the simpler model. Such a contradictory result can be explained by the fact that the attention mechanism could not catch high-level dependencies in sequences, and it is enough to use differences at the n-gram level to get a relatively good result.
