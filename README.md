# Create Own GPT Model
Construct and train a minified GPT implementation. GPT refers to the "Generative Pre-trained Transformers" from OpenAI, originally described in "Improving language understanding with unsupervised learning". This specific GPT implementation is heavily inspired by the minGPT implementation provided by Andrej Karpathy.

There are three important PyTorch modules here:

MultiHeadSelfAttention: a self-attention implementation which will be provided for you;
Block: a transformer block which is repeated n_layer times in a GPT model;
GPT: the full GPT model itself, including intial embeddings, the GPT blocks, and the token decoding logic.
The GPT module uses the Block module, which in turn uses the MultiHeadSelfAttention module.

    ┌────────────────────────┐     
    │          GPT           │     
    └────────────────────────┘     
                ▲                  
    ┌───────────┴────────────┐     
    │         Block          │     
    └────────────────────────┘     
                ▲                  
    ┌───────────┴────────────┐     
    │ MultiHeadSelfAttention │     
    └────────────────────────┘     

## Key Steps:
* Complete the implementataion of the Block Class
* Complete GPT model implementation of _init_ and forward
* Complete the generate method
* Train the model
