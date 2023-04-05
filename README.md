# 
// Shorthash function must be contingent on first root block in root chain having nonce unspecified [], otherwise error
// Shorthash function also contingent on previous hash (aka parent hash) also unspecified [], otherwise error
// You can hash pre-existing payload in original block which payload and other data do not change later. 
// Root blocks for forks are ideal use for ommer blocks.  
// Fork block is formed second after root block, because fork block needs shorthash from root block. 
// Necessary but not sufficient element of fork block is an authorized or special hash field defined as = shorthash from root block. 
// Fork block becomes the previous block for root block, previous block was left unspecified see line 3 above
// Root block can then be completed as first block on forked chain.   
