# Web-Scraping-and-Scientific-News
A program to look through web pages and return articles and their respective DOIs

The program, called a spider (term I learned when I tried using Scrapy), **is not a Scrapy object**. These spiders will be unique to each journal until I divise a spider Class which will be birthed after a couple of more tries. 

Each program will try to use as few as possible module imports but these will be the cornerstones for navigating and manipulating:

*Firstly*: **BeautifulSoup4 (*bs4*)** For parsing html and getting the respective titles and links

*Secondly*: **Selenium** For interacting with web pages, because some web pages only allow some html elements to exist ***AFTER*** clicking on them. 

*Thirdly*: From the Selenium module **ActionChains** will be imported in order to perform the clickings and the interactive things needed in order to activate html elements for scraping. 

For the moment there will be various spiders for scraping different scientific journals for their titles and their respective links. 
Each journal's spider's bugs will be documented here:

**Developmental Biology **

   Journal of Developmental Biology. (ELSEVIER)
   So far the program works pretty well. All of the titles until 2001 (which is up to where I decided to scrape for information) are present. The **bugs** are in the links. I've only **managed** to correct the offset by a couple of titles which is a lot compared to the initial offset of at least 20 titles. *Offset* meaning that the title link for title D, corresponds to title A. And title link for title H, corresponds to title D. But this doesn't happen for the first few issues but actually offsetting appears after a few issues of scraping down the line.
   
**Biotechnology and Bioprocess Engineering**

   *The Korean Society for Biotechnology and Bioengineering and Springer-Verlag GmbH Germany, part of Springer Nature*
   This scrape turned out quite well, there was no offsetting between titles and links. Article Link corresponds to Article Title.
  
**Physical Biology**

   Official Journal of *Sociedad de Biofísicos Latino Americanos*. Physical Biology scraped perfectly
   
**Sydowia**

   An international Journal of Mycology. Sydowia Fungus Journal scraped but there is an offset between titles and links. Links are also incomplete. 
   
**Immunity**

   Journal of Cell *Immunity*. Parses perfectly and extracts full link text files plus article's title.
   
**Ecology**

   Journal of Ecological Society of America. Scrapes perfectly all titles and there respective DOIs.
   
**Forest Sciences**

   Journal of Forest and Environmental Science. Undergoing scraping
   
**Biophysical Reviews**

   Journal of Biophysical Reviews (BiophyRev). Scrapes perfectly all titles and there respective DOIs.
   
**Theoritical and Applied Genetics**

   Journals of Theoritical and Applied Genetics (Genetics). Scrapes perfectly all titles and there respective DOIs.
   
**Meterials Science**

   Journal of Materials Science (MatSci). Scrapes perfectly all titles and there respective DOIs.
   
**Chronobiology**

   Journal of Chronobiology. Scrapes perfectly all titles and there respective DOIs.
   
**Critical Reviews in Biotechnology**

   From the Journal of Critical Reviews in Biotechnology (CRinBiotech). Scrapes perfectly all titles and there respective DOIs.
   
**Journal of Applied Statistics**

   Journal of Applied Statistics. Scrapes perfectly all titles and there respective DOIs.
