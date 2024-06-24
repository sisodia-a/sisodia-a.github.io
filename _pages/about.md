---
permalink: /
title: "About"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I am an Assistant Professor of Marketing at Purdue University. I received my Ph.D. in Quantitative Marketing from Yale University. Prior to my doctoral studies, I worked at Myntra (online fashion retailer), 21st Century Fox (broadcast media) and Tata Consultancy Services (IT). I studied Electrical Engineering at the Indian Institute of Technology, Banaras Hindu University and received my Post Graduate Diploma in Management from the Indian Institute of Management, Ahmedabad.

## Research Papers

<details>
  <summary>
    Generative Interpretable Visual Design: Using Disentanglement for Visual Conjoint Analysis (with Alex Burnap and Vineet Kumar)<br>
    <em>Conditionally Accepted at Journal of Marketing Research</em> <a href="files/GenerativeInterpretableVisualDesign.pdf">[PDF]</a><br>
  </summary>
  <p>
    This article develops a method to automatically discover and quantify human-interpretable visual characteristics directly from product image data. The method is generative, and can create new visual designs spanning the space of visual characteristics. It builds on disentanglement methods in deep learning using variational autoencoders, which aim to discover underlying statistically independent and interpretable visual characteristics of an object. The impossibility theorem in the deep learning literature indicates that supervision with ground truth characteristics would be required to obtain unique disentangled representations. However, these are typically unknown in real world applications, and are in fact exactly the characteristics we want to discover. Extant machine learning methods require ground truth labels for each visual characteristic, resulting in a task requiring human evaluation and judgment to both design and operationalize. In contrast, this method postulates the use of readily available product characteristics (such as brand and price) as proxy supervisory signals to enable disentanglement. This method discovers and quantifies human-interpretable and statistically independent characteristics without any specific domain knowledge on the product category. It is applied to a dataset of watches to automatically discover interpretable visual product characteristics, obtain consumer preferences over visual designs, and generate new ideal point designs targeted to specific consumer segments.
  </p>
</details>

- Winner, 2023 ISMS Doctoral Dissertation Proposal Competition
- Finalist, 2023 ASA Statistics in Marketing Doctoral Research Award

## Works in Progress

<details>
  <summary>
    Market Structure Mapping with Visual Characteristics (with Vineet Kumar and Alex Burnap)<br>
  </summary>
</details>

<details>
  <summary>
    Did *Illegal* Shopping Stymie India's Demonetization? Evidence from an Online Retailer (with K. Sudhir and Nitish Jain)<br>
  </summary>
</details>

A data-driven personal website
======
Like many other Jekyll-based GitHub Pages templates, Academic Pages makes you separate the website's content from its form. The content & metadata of your website are in structured markdown files, while various other files constitute the theme, specifying how to transform that content & metadata into HTML pages. You keep these various markdown (.md), YAML (.yml), HTML, and CSS files in a public GitHub repository. Each time you commit and push an update to the repository, the [GitHub pages](https://pages.github.com/) service creates static HTML pages based on these files, which are hosted on GitHub's servers free of charge.

Many of the features of dynamic content management systems (like Wordpress) can be achieved in this fashion, using a fraction of the computational resources and with far less vulnerability to hacking and DDoSing. You can also modify the theme to your heart's content without touching the content of your site. If you get to a point where you've broken something in Jekyll/HTML/CSS beyond repair, your markdown files describing your talks, publications, etc. are safe. You can rollback the changes or even delete the repository and start over -- just be sure to save the markdown files! Finally, you can also write scripts that process the structured data on the site, such as [this one](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.ipynb) that analyzes metadata in pages about talks to display [a map of every location you've given a talk](https://academicpages.github.io/talkmap.html).

Getting started
======
1. Register a GitHub account if you don't have one and confirm your e-mail (required!)
1. Fork [this repository](https://github.com/academicpages/academicpages.github.io) by clicking the "fork" button in the top right. 
1. Go to the repository's settings (rightmost item in the tabs that start with "Code", should be below "Unwatch"). Rename the repository "[your GitHub username].github.io", which will also be your website's URL.
1. Set site-wide configuration and create content & metadata (see below -- also see [this set of diffs](http://archive.is/3TPas) showing what files were changed to set up [an example site](https://getorg-testacct.github.io) for a user with the username "getorg-testacct")
1. Upload any files (like PDFs, .zip files, etc.) to the files/ directory. They will appear at https://[your GitHub username].github.io/files/example.pdf.  
1. Check status by going to the repository settings, in the "GitHub pages" section

Site-wide configuration
------
The main configuration file for the site is in the base directory in [_config.yml](https://github.com/academicpages/academicpages.github.io/blob/master/_config.yml), which defines the content in the sidebars and other site-wide features. You will need to replace the default variables with ones about yourself and your site's github repository. The configuration file for the top menu is in [_data/navigation.yml](https://github.com/academicpages/academicpages.github.io/blob/master/_data/navigation.yml). For example, if you don't have a portfolio or blog posts, you can remove those items from that navigation.yml file to remove them from the header. 

Create content & metadata
------
For site content, there is one markdown file for each type of content, which are stored in directories like _publications, _talks, _posts, _teaching, or _pages. For example, each talk is a markdown file in the [_talks directory](https://github.com/academicpages/academicpages.github.io/tree/master/_talks). At the top of each markdown file is structured data in YAML about the talk, which the theme will parse to do lots of cool stuff. The same structured data about a talk is used to generate the list of talks on the [Talks page](https://academicpages.github.io/talks), each [individual page](https://academicpages.github.io/talks/2012-03-01-talk-1) for specific talks, the talks section for the [CV page](https://academicpages.github.io/cv), and the [map of places you've given a talk](https://academicpages.github.io/talkmap.html) (if you run this [python file](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.py) or [Jupyter notebook](https://github.com/academicpages/academicpages.github.io/blob/master/talkmap.ipynb), which creates the HTML for the map based on the contents of the _talks directory).

**Markdown generator**

I have also created [a set of Jupyter notebooks](https://github.com/academicpages/academicpages.github.io/tree/master/markdown_generator
) that converts a CSV containing structured data about talks or presentations into individual markdown files that will be properly formatted for the Academic Pages template. The sample CSVs in that directory are the ones I used to create my own personal website at stuartgeiger.com. My usual workflow is that I keep a spreadsheet of my publications and talks, then run the code in these notebooks to generate the markdown files, then commit and push them to the GitHub repository.

How to edit your site's GitHub repository
------
Many people use a git client to create files on their local computer and then push them to GitHub's servers. If you are not familiar with git, you can directly edit these configuration and markdown files directly in the github.com interface. Navigate to a file (like [this one](https://github.com/academicpages/academicpages.github.io/blob/master/_talks/2012-03-01-talk-1.md) and click the pencil icon in the top right of the content preview (to the right of the "Raw | Blame | History" buttons). You can delete a file by clicking the trashcan icon to the right of the pencil icon. You can also create new files or upload files by navigating to a directory and clicking the "Create new file" or "Upload files" buttons. 

Example: editing a markdown file for a talk
![Editing a markdown file for a talk](/images/editing-talk.png)

For more info
------
More info about configuring Academic Pages can be found in [the guide](https://academicpages.github.io/markdown/). The [guides for the Minimal Mistakes theme](https://mmistakes.github.io/minimal-mistakes/docs/configuration/) (which this theme was forked from) might also be helpful.
