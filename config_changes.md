# _config.yml changes needed

## 1. Update email
Find:
  email: "hxc5400@psu.edu"
Replace with:
  email: "hchoi342@gatech.edu"

## 2. Add ORCID to social links (if your theme supports it)
Add under the social links section:
  orcid: "0000-0003-0588-7301"

## 3. Add CV to navbar
Find your navbar-links section (looks something like):
  navbar-links:
    About Me: "aboutme"
    Research: "research"

Replace with:
  navbar-links:
    About Me: "aboutme"
    Research: "research"
    CV: "assets/data/hchoi_cv.pdf"

## 4. Homepage bio blurb
In index.html (or index.md), add this line above the news feed:

I am a postdoctoral scholar at Georgia Tech investigating the deep processes
that shaped early Earth — from the dynamics of ancient subduction zones to
the formation of the first continents.

## 5. PDF figure note
porosity_diff2.pdf needs to be converted to PNG for web display.
Suggested filename: porosity_diff2.png
Place in: assets/img/
The research.md file already references it as porosity_diff2.png
