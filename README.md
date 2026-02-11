# ssei-website
Space Science and Engineering Initiative website

This repository contains the source and configuration for the Space Systems Engineering and Integration (SSEI) website. The site is built using Sphinx and MyST-Parser, allowing for content to be written in both reStructuredText and Markdown.

🛠 Setup and Installation
To work on this website locally, follow these steps:

1. Clone the repository
In Bash: 
    git clone git@github.com:sebviev/ssei-website.git
    cd ssei-website

2. (Optional) Create a virtual environment
It is recommended to use a virtual environment to manage dependencies:

In Bash: 
    python3 -m venv venv
    source venv/bin/activate

3. Install dependencies
In Bash : 
    pip install -r requirements.txt

🚀 Building the Website
To compile the source files into a viewable website, use the provided Makefile:

In Bash :
make html


🖥 Local Preview
Open build/html/index.html in your web browser.


📂 Repository Structure
source/: Contains all website content.

index.rst: The main landing page and site navigation tree.

pages/: Markdown (.md) files for individual pages (About, Team, etc.).

_static/: Custom CSS (custom.css) and images (logos, faculty photos).

conf.py: The Sphinx configuration file where extensions and themes are defined.

requirements.txt: List of Python packages required to build the site.

.github/workflows/: Automation script to deploy the site to GitHub Pages on every push.

🌐 Deployment
The website is hosted via GitHub Pages.

Automatic Deployment: Any changes pushed to the main branch will trigger a GitHub Action that builds and deploys the site automatically.

Live URL: https://sebviev.github.io/ssei-website/