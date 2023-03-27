---
title: "A Robust Shape-Aware Rib Fracture Detection and Segmentation Framework with Contrastive Learning"

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here 
# and it will be replaced with their full name and linked to their profile.
authors:
- admin
- Liming Xu
- Danny Z. Chen
- Honghao Gao
- Jian Wu

# Author notes (optional)
# author_notes:
# - "Equal contribution"
# - "Equal contribution"

date: "2023-03-25T00:00:00Z"
doi: ""

# Schedule page publish date (NOT publication's date).
publishDate: "2023-03-25T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["2"]

# Publication name and optional abbreviated publication name.
publication: IEEE Transactions on Multimedia
publication_short: IEEE TMM

abstract: The rib fracture is a common type of thoracic skeletal trauma, and its inspections using computed tomography (CT) scans are critical for clinical evaluation and treatment planning. However, it is often challenging for radiologists to quickly and accurately detect rib fractures due to tiny objects and blurriness in large 3D CT images.  Previous diagnoses for automatic rib fracture mostly relied on deep learning (DL)-based object detection, which highly depends on label quality and quantity. Moreover, general object detection methods did not take into consideration the typically elongated and oblique shapes of ribs in 3D volumes. To address these issues, we propose a shape-aware method based on DL called SA-FracNet for rib fracture detection and segmentation. First, we design a pixel-level pretext task founded on contrastive learning on massive unlabeled CT images. Second, we train the fine-tuned rib fracture detection model based on the pre-trained weights. Third, we develop a fracture shape-aware multi-task segmentation network to delineate the fracture based on the detection result. Experiments demonstrate that our proposed SA-FracNet achieves state-of-the-art rib fracture detection and segmentation performance on the public RibFrac dataset, with a detection sensitivity of 0.926 and segmentation Dice of 0.754. Test on a private dataset also validates the robustness and generalization of our SA-FracNet.

# Summary. An optional shortened abstract.
summary: Deep learning model for rib fracture diagnose (detection and segmentation.

tags: ['medical imaging']

# Display this page in the Featured widget?
featured: true

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: ''
url_code: ''
url_dataset: ''
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
- Medical Image Analysis

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
