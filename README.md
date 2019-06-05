# songproject

TO DO:

THINGS TO NOTE: maybe songs are a bad fit for this project because of repetitiveness. 

DATA CLEANING:
- remove non english words
- So so so many typos in these lyrics with wierd words mashed together, get rid of these
-Decide if we need to remove more stop words

MODEL FITTING
- Get a network model to produce any sort of reasonable result
- Get LSA to run (many existing packages, look terrible rn)


POSTER THEME:
- "We build an adjacency matrix of song lyrics"
- "And then build a latent spcae model with VBLPCM
- "It was bad and we didn't learn anything useful"
- "So we used LSA (singular value decomposition basically) to reduce the 
dimension of the space. This helped- kind of learned something.
-- Did it tell us anything about sentiment??? Did pre-post trump get clustered even a little bit?? I have a feeling the answer will be no.   


--- Frame the research question as "did music lyrics change pre / post trump". Do a few different clustering things. Answer::: the clusters based on lyrics did not really learn pre/post they learned like rap vs. not rap kind of. So... maybe lyrics are not a good indicator for the research question we originally set out to study. 


NOTES FROM DEBUGGING THAT WE CAN WRITE ABOUT ON POSTER

- Songs are more repetitive than typical documents because of chorus/refrains. There were some wacky things in our song matrix. Songs that contain the word "low" 100 times. Necessary to get rid of these- they mess up results. Truncate all counts in matrix that are over 20 to 20 or something. 