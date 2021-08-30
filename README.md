# Instagram-Automation-Tool
# Objective
You will be able to automate general activities like following, likes, comments and exploring in Instagram apps using python and selenium automation.

# Project Context
1. Instagram is one of the leading social media apps today. You yourself must have had some experience in using Instagram. But often you might have got tired of following, liking, commenting some person or some post every now and then. So why not automate the process using simple selenium automation techniques? Using Selenium webdriver we can interact with a webpage like a real user and perform various actions like clicking, scrolling, typing to achieve goals like following, liking and commenting (here).

2. Web automation today is a goto solution for testing an application, but it also has various other use cases like automating redundant processes for digital marketers, and SEO specialists. Also we can use automation to gather data for a particular business page, helping them with better user engagement by helping them figure out their audience's sentiment using NLP analysis on comments (challenge yourself by trying this out). For various computer vision models datasets are required. A good way to gather the data specific to the use case is by using automation rather than using the generic datasets on the web. This project can be a headstart for your data extraction journey. Use skills acquired in this project and build scripts for other websites as well.

3. Modern websites dynamically load data which makes it hard to just make curl requests to that site, rather we need to interact with the page in order to extract the data. Apart from this it is also really fun to build automation scripts for your daily web chores.

4. This project is a good start for beginners and a refresher for professionals who have dabbled in python scripts/selenium/web crawlers before. The experience of implementing this basic automation will be helpful in learning web crawlers and more, so feel free to innovate and explore!

# Product Architecture
This Product Architecture consists of 5 stages as follows:
1. Login to your Instagram profile to begin
2. Redirecting to several URL endpoints like Explore page or tag pages
3. Redirecting to target interest pages or our own profile page
4. Traversing the images and storing metadata along the way
5. Using the metadata to fetch images, and use text data scraped for other sentiment analysis projects

# Primary goals
1. Automate various actions and interaction
2. Storing various meta data regarding the profiles, pages and posts we visit

# High-Level Approach
1. The main aim is to perform is to automate user interaction with Instagram
2. Firstly we need to automate login process, which includes entering username, password and clicking login button
3. Next we need a starting point to begin scraping, there are many choices for this, for example explore page
4. Now when we are at the explore page, we will try to go through the posts one by one and then perform a set of tasks, which are liking, commenting, following and saving. To achieve these we will use selenium webdriver tools to perform browser interactions such as clicking, scrolling, and typing, etc.
5. While going through posts we will save the image/video URL of these posts, and then we will consolidate these URLs to fetch the media and store it on our system.
6. We will also store metadata like profile name, follower count, likes, comments, date posted, etc. to process them later for an extended usage.
7. Now that we have collected this metadata, we will use this data to analyse this text using NLP algorithms. We may also use the image fetched to train computer vision models. Note that this step is completely optional and beyond scope of this tutorial, but the idea for this is to motivate you and to build thought processes for data extraction.
