# z100-preserved

## What is this?

I am preserving the contents of the Z100 Lifeline site. My dad used to own one of these and I think he still follows the site. The owner of the site indicated issues with continuing to host the work on EarthLink. I noted that it would be possible to (easily) migrate this static site over to a Github static page and use a CNAME file to preserve the custom domain link, too.

## How was this repo created?
At 5:25 PST on Wednesday, March 27, 2019 I ran the following command:

```
wget -m -p -E -k www.home.earthlink.net/\~z100lifeline/
```

Each of these optional argument parameters is explained below:

```
-m, --mirror            Turns on recursion and time-stamping, sets infinite 
                          recursion depth, and keeps FTP directory listings.
-p, --page-requisites   Get all images, etc. needed to display HTML page.
-E, --adjust-extension  Save HTML/CSS files with .html/.css extensions.
-k, --convert-links     Make links in downloaded HTML point to local files.
```

This had the effect of crawling the contents of the site and copying over the nested contents into a target directory.