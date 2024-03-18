---
title: "SynCluster: Reaction Type Clustering and Recommendation Framework for Synthesis Planning"

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here 
# and it will be replaced with their full name and linked to their profile.
authors:
- Tiantao Liu
- admin
- Yuansheng Huang
- Yue Wan
- Jian Wu
- Chang-Yu Hsieh
- Tingjun Hou
- Yu Kang

# Author notes (optional)
author_notes:
- "Equal contribution"
- "Equal contribution"

date: "2023-11-17T00:00:00Z"
doi: "https://doi.org/10.1021/jacsau.3c00607"

# Schedule page publish date (NOT publication's date).
publishDate: "2023-11-17T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["2"]

# Publication name and optional abbreviated publication name.
publication: JACS Au
publication_short: JACS Au

abstract: AI-assisted synthesis planning has emerged as a valuable tool in accelerating synthetic chemistry for the discovery of new drugs and materials. The template-free approach, which showcases superior generalization capabilities, is seen as the mainstream direction in this field. However, it remains unclear whether such an end-to-end approach can achieve problem-solving performance on par with experienced chemists without fully revealing insights into the chemical mechanisms involved. Moreover, there is a lack of unified and chemically inspired frameworks for improving multitask reaction predictions in this area. In this study, we have addressed these challenges by investigating the impact of fine-grained reaction-type labels on multiple downstream tasks and propose a novel framework named SynCluster. This framework incorporates unsupervised clustering cues into the baseline models and identifies plausible chemical subspaces which is compatible with multitask extensions and can serve as model-independent indicators to effectively enhance the performance of multiple downstream tasks. In retrosynthesis prediction, SynCluster achieves significant improvements of 4.1 and 11.0% in top-1 and top-10 prediction accuracy, respectively, compared to the baseline Molecular Transformer, and achieves a notable enhancement of 13.9% in top-10 accuracy when combined with Retroformer. By incorporating simplified molecular-input line-entry system augmentation, our framework achieves higher top-10 accuracy compared to state-of-the-art sequence-based retrosynthesis models and improves over the baseline on the diversity and validity of reactants. SynCluster also achieves 94.9% top-10 accuracy in forward synthesis prediction and 51.5% top-10 Maxfrag accuracy in reagent prediction. Overall, SynCluster provides a fresh perspective with chemical interpretability and reinforcement of domain knowledge in the synthesis design. It offers a promising solution for improving the accuracy and efficiency of AI-assisted synthesis planning and bridges the gap between template-free approaches and the problem-solving abilities of experienced chemists.

# Summary. An optional shortened abstract.
summary: Deep Learning-based Sythesis Planning.

tags: ['drug discovery']

# Display this page in the Featured widget?
featured: false

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: 'https://pubs.acs.org/doi/full/10.1021/jacsau.3c00607'
url_code: 'https://pubs.acs.org/doi/full/10.1021/jacsau.3c00607'
url_dataset: 'https://pubs.acs.org/doi/full/10.1021/jacsau.3c00607'
url_poster: ''
url_project: ''
url_slides: ''
url_source: ''
url_video: ''

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
image:
  # caption: 'Image credit: [**Unsplash**](https://unsplash.com/photos/pLCdAaMFLTE)'
  focal_point: ""
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects:
- Drug Discovery

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
# slides: example
---

<!-- {{% callout note %}}
Click the *Cite* button above to demo the feature to enable visitors to import publication metadata into their reference management software.
{{% /callout %}}

{{% callout note %}}
Create your slides in Markdown - click the *Slides* button to check out the example.
{{% /callout %}}

Supplementary notes can be added here, including [code, math, and images](https://wowchemy.com/docs/writing-markdown-latex/). -->
