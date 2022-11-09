# gnu-c-to-pdf

The [GNU C Library](https://www.gnu.org/software/libc/manual/html_node/index.html) documentation is horrendous and hard to read. I want to fix this.

## Goal

The goal is to scrape all of the online documentation of the library and output a beautiful PDF book of the GNU C Library in the directory of your choice.

The goal could be achieved by these proposed methods:

1. Scrape every individual section to get all of the data into my program, then use a PDF framework to create a styled PDF book.
2. Manipulate each page's styling to be more readable. Then use a web driver to literally save every updated page as PDF

I think I'll rule out method 2 because using a web driver will likely have the most overhead as far as runtime since it's literally running a web browser.

## Tools

Since I'll most likely be using Python for web scraping (unless I find a simple method without the need for scraping), I'm looking at Python libraries that support PDF generation. Here are some contenders from a Google search:

    - Pdfkit
    - pyPDF
    - ReportLab
