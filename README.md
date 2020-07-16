# indie_SAGE Technical Publishing Working Group #iSTPWG

A volunteer research working group to provide technical publishing assistance for The Independent Scientific Advisory Group for Emergencies (SAGE) in the fight against COVID.

Here you can see a pilot example of converting an existing [PDF report](https://www.independentsage.org/wp-content/uploads/2020/05/Independent-Sage-Brief-Report-on-Schools.pdf) into a multi-format publication and applying basics DOI, ISBN identifiers and metadata - web, screen PDF, ebook, print-on-demand, and as HTML source. See results: [Should Schools Reopen?](https://independent-sage.github.io/Should-Schools-Reopen/#/)

## Work group volunteers!

The working group is looking for volunteers and resources to help in the rapid publishing, dissemination and innovations for public engagement of indie_SAGE publications.

See the GitHub ['Issues'](https://github.com/Independent-SAGE/Technical-Publishing-Working-Group/issues) for current tasks and join us on [Gitter](https://gitter.im/indie_SAGE/TPWG) chat if you have a question or comment.

Currently we're looking for people with skills in the following (July 2020):

[Ordered alphabetically]

  - Converting graphics and charts into SVG data driven objects
  - Controlled vocabulary metadata
  - Data science visualisations
  - Docsify
  - DOIs
  - eBook validation and conversion to Kindle
  - Editorial production for multi-format and multi-channel Publishing
  - Graphic designers, artists and illustrators
  - Hugo
  - Jupyter Notebooks creation
  - Language translation - and Weblate/Crowdin GitLab CI setup
  - Librarians and health librarians
  - Managing GitHub and GitLab setup and organisation
  - Metadata wranglers
  - Open Access repository services
  - Proofers and copy editors
  - Publishing pipeline specialists
  - SEO
  - Technical writers and editors
  - Wordpress design, admin, staging
  - XML format experts: MECA, BITS, Xproc, XSLT, etc

## Roadmap

  1. Convert all existing reports to multi-format publications
  2. Ready a 'rapid publishing' workflow for future reports
  3. Develop an Open Science workflow for all other outputs: video, slides, data, etc.
  4. Introduce 'computation publishing' and data science workflows. e.g., Juypter Notebooks
  5. Ensure high quality metadata workflows - Help! Really need a multidimensional metadata management systems
  6. Develop strategy for public engagement of indie_SAGE publications

## Log

Started with report #002 [Should Schools Reopen?](https://independent-sage.github.io/Should-Schools-Reopen/#/)

1. Rip original PDF report
1. Download as HTML , EPUB (source) from Fidus Writer
1. Load repo as Atom project
1. Run R script for HTML to MD conversion https://github.com/akademie-oeffentliches-gesundheitswesen/fidus2github
   - sudo R
   - fidus2github:::convert_fidus_to_github(fiduszipfile = "your-download.zip")
1. Copy all files accross to /docs/isr002/
1. Unzip HTML to a folder to access other assets, e.g., ToC
1. Paste in ToC from index.html to chapter_0.md
1. Provide graphic alternatives for tables
1. Generate front matter
1. Render website with Hugo and Docsify
1. Aquire identifiers and PIDs from Nielsen UK ISBN services and Zenodo DOI service
1. Write metadata
1. Add HTML to Vivliostyle CSS Typesetter and generate Web Book and PDF from Google Chrome
1. Distribute print-on-demand via Lightningsource and ebook via Ingram Spark
1. Publishing on GitHub Pages.
1. Deposit with Zenodo - only usable media and not whole repo as confusing otherwise
1. Deposit all citations in Zotero
1. Make GitHub release

# To Do

 1. GitLab release
 1. Make ISBN legal deposit
 1. Enable Docsify multilingual translation
 1. Add Weblate translation services
 1. Re-render graphics and add SVG chart rendering
 1. Rationalise system
 1. Improve ebook Metadata
 1. Produce ebook Amazon Kindle AZW/kf8 file
 1. Amazon and Google Book - look inside, view inside
 1. Serving or embedding files inside Docsify

## Members

  - Simon Worthington - iSTPWG team leader. Twitter [@mrchristian99](https://twitter.com/mrchristian99); Acting in an individual capacity as research lead of the Hybrid Publishing Consortium an independent research group for book liberation. https://consortium.io/
  - Raquel Perez de Eulate - Designer, CSS Typesetting. Interpunct Studios - Full Stack Graphic Design https://interpunct.dev/

  ## Software Stack

  ### Fidus Writer

  https://github.com/fiduswriter/fiduswriter

  GNU Affero General Public License v3.0

  Donate https://www.fiduswriter.org/donate/

  ### Vivliostyle

  https://github.com/vivliostyle/vivliostyle.js/tree/master/packages/viewer

  AGPL Version 3

  ### Transpect

  https://github.com/transpect

  BSD 2-Clause "Simplified" License

  Copyright (c) 2015, transpect.io All rights reserved.

  ### EPUBCheck W3C

  https://github.com/w3c/epubcheck

  BSD 3-Clause "New" or "Revised" License

  ### Docsify

  https://github.com/docsifyjs/docsify

  MIT License

  Copyright (c) 2016 - present cinwell.li

  ### Docsify Open Publishing Starter Kit

  https://github.com/hibbitts-design/docsify-open-publishing-starter-kit

  MIT License

  Copyright (c) 2020 Paul Hibbitts

  ### Hugo

  https://github.com/gohugoio/hugo

  Apache License 2.0
