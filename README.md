# BDA Final Project (PBL)

## Files:
1. `requirements.txt`
2. `rename_images.py` (utility): sequentially rename each image in `outfits/`
3. `outfits/`: provided clothing pieces (renamed)
4. `generate_embeddings.py`: generates CLIP embeddings of the images in `outfits/`, dimension: 512
5. `outfit_embeddings.npy`: embedding results of outfits in numpy array
6. `catalog_index.json`: mapping of filename in `outfits\` to index in `outfit_embeddings.npy` for fast retrieval
7. `generate_outfit_descriptions.py`: Generate textual descriptions for each outfits in `outfits/`, using LLaVA as backbone VLM model. _use this file for local run_
8. `BDA_Final_Project_generate_outfit_descriptions.ipynb`: Basically `generate_outfit_descriptions.py` converted to python notebook to run in Colab for acceleration with T4 GPU (free tier)
9. `outfit_descriptions.json`: Textual descriptions of each outfits that LLaVa generated.