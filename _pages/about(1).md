---
permalink: /
title: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

Hello! I am currently a master’s student at Tongji University. This is my personal homepage, where I will share some of my research projects and interesting side projects I’ve undertaken. I warmly invite you to reach out and engage in discussions with me!

Research Interests
======
My recent research focuses primarily on open-set object detection, encompassing both 2D OVD(Open-Vocabulary Object Detection) and 3D OVD. In the 2D domain, my collaborators and I utilized a diffusion model to generate sample images for novel categories. We proposed a keypoint localization module based on cross-attention maps to obtain bounding box labels for these sample images, subsequently training a set of prototypes using these box labels. In the 3D domain, we developed an open-set instance segmentation model based on multi-view sampling and distilled an MLP layer to map 3D features into CLIP’s shared embedding space. This enables direct instance classification by measuring the similarity between 3D features and textual features.

Moving forward, I plan to delve deeper into the field of multimodal content understanding.

Current Research
======
<div style="display: flex; align-items: flex-start; margin-bottom: 20px;">
   <div style="flex: 0 0 45%; margin-right: 20px;">
       <div class="image-hover-container">
           <!-- <img src="../images/MOSS_Homepage.png" style="width: 100%; height: auto;"/> -->
          <a href="https://youtu.be/bWvvBuXxSN4?feature=shared" target="_blank">
              <img src="../images/MOSS_Homepage.png" alt="MOSS Homepage" style="width: 100%; height: auto;"/>
          </a>
       </div>
   </div>
   <div style="flex: 0 0 50%;">
       <h3 style="margin-top: 0;"><img src="..\images\favicon-192x192.png" style="height: 1.5em; width: 1.5em; vertical-align: -0.3em; margin-right: 2px;">MOSS: Mask-Oriented Open-Set for 3D Scene Segmentation using Superpoint</h3>
       <p><em>Preparing for NIPS 2025</em></p>
       <p>
           <a href="../files/MOSS_v3.pdf">[PPT]</a>
           <a href="https://youtu.be/lukFo59tY5o">[Video]</a>
       </p>
       <p>
           The voiceover in the videos was created using ByteDance's Model <a href="https://www.doubao.com/">Doubao</a> that cloned my voice!
       </p>
   </div>
</div>

Site-wide configuration
------
The main configuration file for the site is in the base directory in [_config.yml](https://github.com/academicpages/academicpages.github.io/blob/master/_config.yml), which defines the content in the sidebars and other site-wide features. You will need to replace the default variables with ones about yourself and your site's github repository. The configuration file for the top menu is in [_data/navigation.yml](https://github.com/academicpages/academicpages.github.io/blob/master/_data/navigation.yml). For example, if you don't have a portfolio or blog posts, you can remove those items from that navigation.yml file to remove them from the header. 

Create content & metadata
------
For site content, there is one markdown file for each type of content, which are stored in directories like _publications, _talks, _posts, _teaching, or _pages. For example, each talk is a markdown file in the [_talks directory](https://github.com/academicpages/academicpages.github.io/tree/master/_talks). At the top of each markdown file is structured data in YAML about the talk, which the theme will parse to do lots of cool stuff. The same structured data about a talk is used to generate the list of talks on the [Talks page](https://academicpages.github.io/talks), each [individual page](https://academicpages.github.io/talks/2012-03-01-talk-1) for specific talks, the talks section for the [CV page](https://academicpages.github.io/cv), and the [map of places you've given a talk](https://academicpages.github.io/talkmap.html) (if you run this [python file](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.py) or [Jupyter notebook](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.ipynb), which creates the HTML for the map based on the contents of the _talks directory).

**Markdown generator**

The repository includes [a set of Jupyter notebooks](https://github.com/academicpages/academicpages.github.io/tree/master/markdown_generator
) that converts a CSV containing structured data about talks or presentations into individual markdown files that will be properly formatted for the Academic Pages template. The sample CSVs in that directory are the ones I used to create my own personal website at stuartgeiger.com. My usual workflow is that I keep a spreadsheet of my publications and talks, then run the code in these notebooks to generate the markdown files, then commit and push them to the GitHub repository.

How to edit your site's GitHub repository
------
Many people use a git client to create files on their local computer and then push them to GitHub's servers. If you are not familiar with git, you can directly edit these configuration and markdown files directly in the github.com interface. Navigate to a file (like [this one](https://github.com/academicpages/academicpages.github.io/blob/master/_talks/2012-03-01-talk-1.md) and click the pencil icon in the top right of the content preview (to the right of the "Raw | Blame | History" buttons). You can delete a file by clicking the trashcan icon to the right of the pencil icon. You can also create new files or upload files by navigating to a directory and clicking the "Create new file" or "Upload files" buttons. 

Example: editing a markdown file for a talk
![Editing a markdown file for a talk](/images/editing-talk.png)

For more info
------
More info about configuring Academic Pages can be found in [the guide](https://academicpages.github.io/markdown/), the [growing wiki](https://github.com/academicpages/academicpages.github.io/wiki), and you can always [ask a question on GitHub](https://github.com/academicpages/academicpages.github.io/discussions). The [guides for the Minimal Mistakes theme](https://mmistakes.github.io/minimal-mistakes/docs/configuration/) (which this theme was forked from) might also be helpful.
