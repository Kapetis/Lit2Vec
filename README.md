# Lit2Vec

--------------------------------------------------------------------------------

Using the Cbow version of the Word2Vec algorithm on Goodreads data, vectors were trained to represent books. 

This repository includes the Google Colab notebooks used to clean the original goodreads data, train the book vectors, and analyze the vectors. 

These notebooks requires the 'ratings.csv' and the 'books.csv' files which are described here

http://fastml.com/goodbooks-10k-a-new-dataset-for-book-recommendations/

and can be found here

https://github.com/zygmuntz/goodbooks-10k

These notebooks are set up to download these files from your Google Drive, and will ask permission to access your Google Drive. So if you would like to use these notebooks as is, download the files from the link above, and upload them to your Google Drive. 

For more information on how to run the notebooks, click on the HowTo.md file located in this repository. 

If you have any questions or comments or would like to post your results of using the notebooks / model, visit https://www.reddit.com/r/Lit2Vec/

The following images are from two 2D TSNE (quick explanation https://www.youtube.com/watch?v=p3wFE85dAyY ) plot of the resulting book embeddings. The first one is a TNSE of the 3000 most occurring books in the data (out of 10,000 book vectors that were trained), and the second one is a TSNE of all 10,000 books. I did two TSNE's because as the number of points increase, the accuracy tends to decrease, so I wanted to see the maps of the most occuring books, and then the rest

# TSNE maps of top 3000 books

The following pictures are zoom-ins from the full 3k book map TSNE image, followed by the full image. 

This section contains fantasty/high fantasy written within the last 30-40 years. 

![alt text](Images/Book2VecSample1.JPG)

The secton in the middle has mostly comic books with sci books sourrounding it. Near the bottom is Neil Gaiman's graphic novel series Sandman. 

![alt text](Images/Book2VecSample2.JPG)

The books at the top is a Neil Gaiman's section. I'm not familiar with the other books but they seem to have an element of Neil Gaiman's style of paranormal/magic/sci-fi with a humorous style. 

![alt text](Images/Book2VecSample4.JPG)

This section has space-focused sci-fi. There's a small section of Chuck Palahniuk books to the right. 

![alt text](Images/Book2VecSample3.JPG)

Pre-20th century classics which seem to be grouped by time-period and author. 

![alt text](Images/Book2VecSample5.JPG)

The top right is having a Stephan King party and the bottom left side is having a Michael Crichton party. Perhaps they're grouped together because their books have a thrilling / horror quality. The Dark Tower books which have more of a fantasy quality are placed on the opposite side of Michael Crichton books. 

![alt text](Images/Book2VecSample6.JPG)

Classic childrens' books. The majority of the ones on the bottom left are picture books. Roald Dahl has his own section on the top right. Paddington and Winnie the Pooh seem to enjoy each other's company. Actually, the bottom sourrounding section has mostly animal main characters. 

![alt text](Images/Book2VecSample7.JPG)

Top right has some classic plays. To the bottom left of that, there seems to be writings that tend to be cited as having significant cultural influence (Utopia, The Communist Manifesto, The Republic, The Prince, The Art of War). Further left are more classics. At the left there's a section for Kurt Vonnegut books. At the bottom there are many early to mid 20th century classics. On the right there's a section of books by Charlotte Brontë and Jane Austen.

![alt text](Images/Book2VecSample8.JPG)

Lots of classic non-picture childrens books on the left side. Lord of the Rings and CS Lewis books on the right. 

![alt text](Images/Book2VecSample9.JPG)

This section has modern (written in the 90's to current) childrens books series. A Series of Unfortunate Events. Harry Potter, Artemis Fowl, Alex Rider, Inkworld, Inheritance Cycle, etc. 

![alt text](Images/Book2VecSample10.JPG)

These books all seem to have informational themes. This section has the most fascinating trends to me. I still haven't fully interpreted these trends but here are the ones I noticed so far. 

The top right seem to be focused on relationship informaion, and below that are books focused on financial, career,  and organizational success (Think and Grow Rich, The 7 Habits of Highly Effective People, etc).  Elon Musk's biography is in that section, which seems to be a favorite of Silicon Valley tech start-up people. The the books on the middle right are productivity themed, (The 4-hour workweek, Flow: The Psycology of Optimal Experience ). 

The books in the middle have more narrative elements: Walter Issacson books, Michael Lewis books, Deliverying Happyness. To the right of that are books about startups. The bottom left has books on food and plant life. 

The middle right is focused on art-based informational books. 

![alt text](Images/Book2VecSample11.JPG)

This section continues the informational trend above, themes more focused on history. 

![alt text](Images/Book2VecSample13.JPG)

This picture continues the historical trend above. The right side tends to have historical ficion books. The middle is focused on American history. 

![alt text](Images/Book2VecSample15.JPG)

This section is focused on comedy, particularly by those working in television industry.  

![alt text](Images/Book2VecSample12.JPG)

A young adult section, the right side is focused on dystopia and paranormal elements, the left side is more realist. 

![alt text](Images/Book2VecSample14.JPG)

These section tends to have books with female main characters. 

![alt text](Images/Book2VecSample16.JPG)

Full map of the 3000 vector TNSE. You'll have to zoom in real close to make out the text. It might be easier to download the picture. 

![alt text](Images/Book2Vec0-3000New.jpg)

# TSNE maps of top 10,000 books

The following pictures are zoom-ins from the full 10k book map TSNE image, followed by the full image. 

American history to the left merging in with general world history to the right

![alt text](Images/10kTSNEHighlights/AmericanHistoryWorldHistory.JPG)

World history merging with universe history and origin theories

![alt text](Images/10kTSNEHighlights/WorldHistoryUniverseHistory.JPG)

Art guidance and history 

![alt text](Images/10kTSNEHighlights/ArtSelfArtHistory.JPG)

Children's classics 

![alt text](Images/10kTSNEHighlights/ClassicChildrens.JPG)

Comedy

![alt text](Images/10kTSNEHighlights/Comedy.JPG)

Comedy reflections and memiors 

![alt text](Images/10kTSNEHighlights/ComedyReflectionsMemiors.JPG)

Cooking and a partial of food science and journalism 

![alt text](Images/10kTSNEHighlights/CookingPartialofFoodScienceandJournalism.JPG)

Food science and journalism

![alt text](Images/10kTSNEHighlights/FoodScienceAndJournalism.JPG)

Religious

![alt text](Images/10kTSNEHighlights/Religious.JPG)

Spys

![alt text](Images/10kTSNEHighlights/Spys.JPG)

Classic societal analysis

![alt text](Images/10kTSNEHighlights/SocietalAnalysis.JPG)

Young adult from the 60s, 70s and 80s. 

![alt text](Images/10kTSNEHighlights/YoungAdult60s70s80s.JPG)

Young adult romance

![alt text](Images/10kTSNEHighlights/YoungAdultYoungAdultRomance.JPG)

Young adult VAMPIRES

![alt text](Images/10kTSNEHighlights/youngadultVampires.JPG)

Self help, this section seems to be focused on empowerment, relationships, and personal finance. 

![alt text](Images/10kTSNEHighlights/SelfHelpEmpowermentRelationshipsPersonalFinance.JPG)

Self help, this section seems to be focused on eartern philosophy

![alt text](Images/10kTSNEHighlights/SelfHelpSpiritialEasternPhilosophy.JPG)

Middle of the self help section, covers a bit of everything

![alt text](Images/10kTSNEHighlights/SelfHelpCenterEverything.JPG)

Self help, this section seems to be focused on self analysis and overall pscyhology

![alt text](Images/10kTSNEHighlights/SelfHelpSelfAnalysisPsychology.JPG)

Self help, this section seems to be focused on productivity, influence, leadership, and business. 

![alt text](Images/10kTSNEHighlights/SelfHelpProductivityInfluenceLeadershipBusiness.JPG)

Not so much self help anymore, more of a focus on innovation and biographies of major innovators. 

![alt text](Images/10kTSNEHighlights/SelfHelpInnovationBiographies.JPG)

Not so much self help anymore, books on overall business, finance, and economics

![alt text](Images/10kTSNEHighlights/BusinessFinanceEconomics.JPG)

Manga

![alt text](Images/10kTSNEHighlights/Manga.JPG)

High fantasy

![alt text](Images/10kTSNEHighlights/HighFantasy.JPG)

Graphic Novels

![alt text](Images/10kTSNEHighlights/GraphicNovels.JPG)

Young adult fantasy

![alt text](Images/10kTSNEHighlights/YoungAdultFantasy.JPG)

![alt text](Images/10kTSNEHighlights/YoungAdultFantasy2.JPG)

![alt text](Images/10kTSNEHighlights/YoungAdultFantasy3.JPG)

![alt text](Images/10kTSNEHighlights/YoungAdultFantasy4.JPG)

![alt text](Images/10kTSNEHighlights/YoungAdultFantsy5.JPG)

Entire 10k TSNE map. You'll have to zoom in real close to make out the text. It might be easier to download the picture. 

![alt text](Images/10kTSNEHighlights/Lit2VecFull.jpg)

# Similiarity Properties

The following images show examples of the book vectors' similiarity properties. Similiarity was measured via dot product. 

![alt-text-1](Images/sim1.JPG) 

![alt-text-2](Images/sim2.JPG)

![alt text](Images/sim3.JPG) 

![alt text](Images/sim4.JPG)

![alt text](Images/sim5.JPG) 

![alt text](Images/sim6.JPG)

![alt text](Images/sim7.JPG)


# Arithmetic Properties

The following images show some of the arithmetic properties of the book vectors. Although these properties are not as robust as word vectors' arithmetic properties, I hope to improve these with better hyperparameter optimization and more data. But in the meanwhile, here are some of the more interesting results I found. 

Vampire Classic - Vampire = Classics

![alt text](Images/va1.JPG)

Twilight Graphic Novel - Twilight + Coraline = Coraline Graphic Novel (in top 2 vectors returned)

![alt text](Images/va2.JPG)

Winnie-The-Pooh + Eastern Philosophy =  Pooh Eastern Philosophy

![alt text](Images/va3.JPG)

Romance Classic - Classic = Romance 

![alt text](Images/va4.JPG)

Neil Gaiman Childrens' - Neil Gaiman = Childrens'

![alt text](Images/va5.JPG)

Vampire Romance - Vampire = Romance

![alt text](Images/va6.JPG)

# Individual Bookmaps

The following are images of T-SNE plots that map the closest 500 embeddings for a particular book. 

Harry Potter and the Sorcerer's Stone by J.K Rowling(for very popular books I find it better to use the 2nd or 3rd book from the series to represent the whole series)

Zoomed in preview

![alt text](Images/BookMaps/HarryPotterPreview.JPG)

Full BookMap

![alt text](Images/EachBook.jpg)

Dune by Frank Herbert

Zoomed in preview

![alt text](Images/BookMaps/DunePreview.JPG)

Full BookMap

![alt text](Images/Dune.jpg)

Game of Thrones Clash A Clash of Kings by George R. R. Martin
 (for very popular books I find it better to use the 2nd or 3rd book from the series to represent the whole series)
 
 Zoomed in preview

![alt text](Images/BookMaps/ClashKingsPreview.JPG)

Full BookMap

![alt text](Images/ClashKings.jpg)

A Brief History of Time by Stephen Hawking

Zoomed in preview

![alt text](Images/BookMaps/BriefHistoryTimePreview.JPG)

Full BookMap

![alt text](Images/BriefHistoryTime.jpg)

The Hitchhiker's Guide to the Galaxy by Douglas Adams

Zoomed in preview

![alt text](Images/BookMaps/HitchhikerGalaxyPreview.JPG)

Full BookMap

![alt text](Images/HitchhikerGuideGalaxy.jpg)

Steve Jobs by Walter Isaacson

Zoomed in preview

![alt text](Images/BookMaps/SteveJobsPreview.JPG)

Full BookMap

![alt text](Images/SteveJobs.jpg)

Slaughterhouse-Five by Kurt Vonnegut

Zoomed in preview

![alt text](Images/BookMaps/Slaughterhouse-FivePreview.jpg)

Full BookMap

![alt text](Images/BookMaps/Slaughterhouse-Five.jpg)

Siddhartha by Hermann Hesse

Zoomed in preview

![alt text](Images/BookMaps/SiddharthaPreview.jpg)

Full BookMap

![alt text](Images/BookMaps/Siddhartha.jpg)

Night Watch (Discworld) by Terry Pratchett

Zoomed in preview

![alt text](Images/BookMaps/NightWatchPreview.JPG)

Full BookMap

![alt text](Images/BookMaps/NightWatch.jpg)

The Martian by Andy Weir

Zoomed in preview

![alt text](Images/BookMaps/MartianPreview.JPG)

Full BookMap

![alt text](Images/BookMaps/Martian.jpg)

11/22/63 by Stephen King 

Zoomed in preview

![alt text](Images/BookMaps/11-22-63Preview.JPG)

Full BookMap

![alt text](Images/BookMaps/JKFTimeTravel.jpg)

East of Eden by John Steinbeck

Zoomed in preview

![alt text](Images/BookMaps/EastEdenPreview.JPG)

Full BookMap

![alt text](Images/BookMaps/EastEden.jpg)

# Takeaways (Stuff for other Machine Learning fans)

-Smaller Batch Sizes

Smaller batch sizes (32 and 64) durng training are very important to making sure robust similiarity properties for all book vectors. At higher batch sizes (128, 256, and 512) most of the vectors had decent similiarity properties but there always seemed to be a few books whose vectors did not have decent similiarity properties (based purely on my domain knowledge of the data, aka knowing which books should be most similiar to certain books). 

In the case of Harry Potter books 2-7, from looking directly at the data, I knew that the most similiar books to these should be other Harry Potter books in the series, but this was not the case, even after 100 epoches (ignore the number in the gif, I didn't include a variable to keep track of the total epoches in the checkpoint file until ~60 or so epoches). However, when I switched to batch size 64, the similiarty properties for Harry Potter books 2-7 improved significantly after only a few epoches. This is demonstracted in the gif below (you probably have to tinker with the notebooks to know what's going on ). 

![alt text](Images/HarryPotterSmallBatch.gif)

I am not 100% sure what this is so, but this is my best guess:

Since the average window size is 112 and varies from 20 to 200 (depending on how many books a user has read), there was high probability that a particular book in a series like Harry Potter would get paired other books instead of Harry Potter. Say that there were 7 books in the series and the user had rated all 7 of them, and this user has also rated 112 other books; the probability of a Harry Potter book being paired with another Harry Potter book as a label for that user is 6/112. In this case, I theorized that maybe higher batch sizes would hinder the optimization more significantly than an application of the word2vec algorithm for a small and constant window size since word2vec is trying to optimize many embeddings at once. 

-Softmax Embeddings for Vector Arithmetic

So far, all the vector arithmetic examples above are cases where I performing the addition and/or subtraction on the book input embeddings, and then performing similiarity on the resulting vector against the softmax embeddings. The results were much more robust than comparing the resulting vector to the input embeddings. 

-Variable Length Window  (VLW)

In the original Word2Vec Cbow algorithm, there is a fixed window size of words to be used as input for a particular target. For example, if the window size is 2 words to the left and to the right of a target word, in this sentence "The cat in the hat", if the target word (label) is 'in', then the words 'The', 'cat', 'the', and 'hat' would have their vectors averaged, and the resulting vector would be used as the input. 

In this project, having a fixed window size is not possible. For a particular data point (input), all the potential labels are all other books rated by the user who rated the book of the input, and there is a lot of variation in the number of books each user has reviewed, so window sized was not constant. 

Although the window sized was not constant, the number of input vectors to average was kept constant. All of the data presented used 2 averaged vectors as the input, since this seemed to have resulted in the most robust arithmetic properties for the vectors. There were no noticeable advantages in similiarity properties for any number of vectors averaged for the input; I have looked at vectors that were trained with using 4 and 6  averaged vectors as the input. 

# Future plans / projects

Currently working on doing the same thing for research papers, check it out at https://github.com/Santosh-Gupta/Research2Vec and https://www.reddit.com/r/Research2Vec/

# Shoutouts!

![alt text](Images/SpecialThanks/BeSpokeMedia.png)

![alt text](Images/SpecialThanks/RaythonSolarLogo.png)
