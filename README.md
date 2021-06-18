# Block-based-algo-using-cryptography

PRE- block -preparation:    

1.Create 10(any) numbers of stego message.  
2. One of them will be encrypted with our own encryptor. Or, multiple of them, in that case, only one will carry the correct message. Other messages will be only used as decoy(illusion).  
3. Make a private key (or any suitable function for detecting the correct stego block)  

Block works:    
1. Each block will be consisting of a visually similar message (stego message/ or null message), a public key and a private key. Public key will be their individual identity, so that we can identify them. Private key will be used to unlock the right one.  
Block = message+ public key+ private key  
2. We will create 10 (any numbers) of block, or N numbers of extra block just to make it complicated.  
3. Then we will encrypt the blocks with any suitable encryption system.  
4. Then we will randomize the blocks  &  join the blocks (zip or any good technique)  

Decrypt:  
1. With the help of public key we will identify the correct one (as they will be randomized, we have to identify them somehow) then use private key to open the secret message.
