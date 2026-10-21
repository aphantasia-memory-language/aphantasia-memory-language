
# Words Without Pictures

**A naturalistic analysis of autobiographical memory language in aphantasia

Senior thesis project, Cognitive Science (Computation and Cognition), University of Pennsylvania Author: Esther Appiah · Expected completion: May 2027

> Status: early development. Collection and analysis code will be added here as the project progresses.

## About the project

Aphantasia is the lifelong inability to voluntarily form visual mental images. Lab studies show that people with aphantasia recall fewer sensory details from their past, while their spatial memory stays intact. No study has yet examined how they describe their memories unprompted, in everyday settings.

This project compares personal memory narratives shared publicly on Reddit by users who self-identify as aphantasic with narratives from comparison users posting in the same communities. It tests three predictions about aphantasic narratives:

1. **Sensory reduction: less visual and perceptual language.
2. **Conceptual compensation: more knowledge-based and conceptual language.
3. **Spatial preservation: spatial language comparable to that of typical imagers.

The goal is the first large-scale, naturalistic language profile of memory without imagery, along with an open, reusable R pipeline for studying differences in inner experience through language.

## How the code uses the Reddit API

The collection script is read-only. It does not post, comment, vote, message users, or interact with anyone on Reddit. It:

- Retrieves public posts and comments from r/Aphantasia to identify users who explicitly self-identify as aphantasic.
- Retrieves those users' public posts and comments in other communities, plus posts from comparison users in the same communities, focusing on personal memory narratives (e.g., replies to r/AskReddit threads such as "What's your earliest memory?" and posts in r/nostalgia).
- Runs within Reddit's rate limits, with collection completed by December 2026.
  
## Data handling commitments
- **Non-commercial, academic use only. Data is not sold, shared, or redistributed.
- **No AI model training. Collected content is not used to train or fine-tune language models or other generative AI systems, and is not shared with third-party AI services. Statistical models in this project (including a classifier for an exploratory research question) are fit only on aggregate linguistic measures derived from the text, and any automated text scoring runs locally.
- **Pseudonymization at collection. Usernames are replaced with hashed IDs as data is collected.
- **Respect for deletion. Deleted or removed content is excluded.
- **No verbatim quotes. No posts are quoted in the thesis or any publication; illustrative examples are paraphrased.
- **Secure storage. Data is stored on secure University of Pennsylvania storage and is not committed to this repository.
- **Ethics. The project follows University of Pennsylvania guidance and best practices for research with public social media data, including the Association of Internet Researchers' ethics guidelines, and complies with Reddit's Data API terms.

## Analysis

Analyses are conducted in R using dplyr, tidytext, lme4, and ggplot2. Linguistic measures include the Lancaster Sensorimotor Norms (Lynott et al., 2020), concreteness norms (Brysbaert et al., 2014), and LIWC-22 categories. Hypotheses and analyses will be preregistered on the Open Science Framework before analysis.

## Contact

Esther Appiah · eappiah@sas.upenn.edu
