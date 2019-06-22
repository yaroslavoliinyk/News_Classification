# News Classification
*Created by Yaroslav Oliinyk*

* The purpose of the following program is 
***to teach AI to classify news by categories***

* Topics of news: 
    * ***ATHEISM***
    * ***BASEBALL***
    * ***AUTO***
    * ***COMPUTER GRAPHICS***
    * ***MEDICINE***
    * ***SPACE***
    * ***IBM HARDWARE***
    * ***WINDOWS X***
    
* Used algorithms: 
    * **Naive Bayes**
    * **Multinomial Naive Bayes**
    
### Launching the program
1. Download the repository
2. Extract the program in "Downloads" folder
3. Use the following command: *"cd ~/Downloads/News_Classification/program/src"*
4. Then this: *"javac Main.java"*
5. Then run it: *"java Main"*
6. Well done! The program is running.

### Scope of program
* Firstly, I found a service with news *to classify*(it's already included into the program)
   * You can get aquainted with them here: http://qwone.com/~jason/20Newsgroups/
* The data was divided in **TRAINING** and **TESTING** data
>![Fetched data](https://raw.githubusercontent.com/yaroslavoliinyk/News_Classification/master/pics/1.png)
* Testing data contains of the following categories:
>![Categories](https://raw.githubusercontent.com/yaroslavoliinyk/News_Classification/master/pics/2.png)
* Let's take a look into category: **ATHEISM**
>![Atheism Category](https://raw.githubusercontent.com/yaroslavoliinyk/News_Classification/master/pics/3.png)
* As you can see, each topic includes *.\*txt files* with **NEWS**
* Let's **open** the first file
>![File_open](https://raw.githubusercontent.com/yaroslavoliinyk/News_Classification/master/pics/4.png)
* Pay attention on the *document structure*. It contains of some **garbage** like *email*,*subject*,*organisation* and so on
* Our goal: **parse and fetch only valuable data**
* To *Classify* the data I will use **WEKA Explorer** -  *a collection of machine learning algorithms for solving real-world data mining problems*
>![WEKA](https://raw.githubusercontent.com/yaroslavoliinyk/News_Classification/master/pics/5.png)
* So, my program has to:
   * Go to every document
   * Parse only valid data
   * Transfer it into readable for **WEKA** format **\*.arff**
* The format **\*.arff** has to have the following structure:
>![ARFF structure](https://raw.githubusercontent.com/yaroslavoliinyk/News_Classification/master/pics/6.png)
### After program has run
* You will get appropriate **TRAINING** and **TESTING** data ready to be **CLASSIFIED**
* In the following folder: *News_Classification/program/src* you'll find 2 created by a program files:
>![ARFF structure](https://raw.githubusercontent.com/yaroslavoliinyk/News_Classification/master/pics/12.png)
* Now, **we're ready to Classify it**
* Open *WEKA Explorer*
>![ARFF structure](https://raw.githubusercontent.com/yaroslavoliinyk/News_Classification/master/pics/7.png)
* Here you can see the statistics of the number of articles:
>![ARFF structure](https://raw.githubusercontent.com/yaroslavoliinyk/News_Classification/master/pics/9.png)
### Classification results
* **Naive Bayes**
>![ARFF structure](https://raw.githubusercontent.com/yaroslavoliinyk/News_Classification/master/pics/10.png)
* **Multinomial Naive Bayes**
>![ARFF structure](https://raw.githubusercontent.com/yaroslavoliinyk/News_Classification/master/pics/11.png)
* As you can see **Multinomial Naive Bayes** was more precise *82%* against *58%*
* With the program you can try out different Classifiers like **Decision Trees**, **Boosted Trees**, **Random Forest**, **Neural Networks** and so on
### Have fun! :+1: 

	All rights are reserved
		2019





