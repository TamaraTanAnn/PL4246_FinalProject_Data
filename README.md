# PL4246_FinalProject_Data
Title: Examining Culture Traits in Popular Song Lyrics in Network Analysis (R-Studio)

This project has used network science to analyze the micro-level features of a network, consisting of pronouns in popular song lyrics to investigate the   increase in individualism from 2000 to 2019. 

Data Processing flow: 
  1. Upload song lyrics into individual txt.files and store into a shared folder 
  2. Use UDPipe (https://cran.r-project.org/web/packages/udpipe/vignettes/udpipe-annotation.html) to tokenise and tag each word with speech information. 
    <br>a. Following UDPipe tutorial, the tagged words will be stored into a dataframe 
     <br>b. Cleaning is done here to remove unwanted columns and rows (e.g. punctuation) 
  3. Convert each text dataframe (song lyric) into a string and store in a list 
    <br> a. This step is tidying up the data, combining the song lyrics of the same year into its individual dataframe 
    <br> b. This will create a list of dataframes per year
  4. Co-occurence function (https://github.com/csqsiew/cooccurNet) can be used to convert the list into edgelists to form igraphs for analysis 
  
 
