# App-analysis

In this simple project, we are going to scrap the app reviews from the google play store and apple app store and then analyze the reviews. The app which we are choosing is an Indian streaming app called “Loco”. Finally, we will try to summarise the results in the Tableau dashboard.

## Scraping

For scraping the reviews, we are using the scrapper available on Python Package Index (PyPI). Google play store reviews are scrapped with “google-play-scraper” and for app store we used “app-store-scraper”.



## What is the distribution of ratings?

With the help of pandas and Matplotlib here is the distribution of ratings in both stores.


As we can see most of the Android users rated 5-star rating which shows the app is going good. While the app store app for iphone users might have some issues as many rated it 1.

## What is average rating trend over the years?

Also, we can see the trend of avg ratings over the years for both stores



Let's look at the sentiments of the reviews. We can see 70% of the reviews are positive for the Android app and 25% are negative. 
Whereas for ios apps it is 70% negative and 20% are positive which shows ios app have some major issues.

## How many negative reviews app team has addressed?

Now let's look at how many negative reviews have been replied to by the app team on both stores.
So here we can see on the google play store 60% of the reviews had been answered which is decent as many reviews don’t have sensible text. But on app stores, only 37% are answered which is bad.

## What topics arrre mostly mentioned in reviews?

Now we need to dig into reviews and get idea of what eviews are saying. For this we used pretained model Yet Another Keyword Extraction(YAKE) for extracting keywords.

Let’s look fo Google play store reviews for Loco app.

Positive reviews:

Negative reviews:

App store reviews for Loco app:

Positive reviews:

Negative reviews:
