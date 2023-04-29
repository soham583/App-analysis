# App-analysis

In this simple project, we are going to scrap the app reviews from the google play store and apple app store and then analyze the reviews. The app which we are choosing is an Indian streaming app called “Loco”. Finally, we will try to summarise the results in the Tableau dashboard.

## Scraping

For scraping the reviews, we are using the scrapper available on Python Package Index (PyPI). Google play store reviews are scrapped with “google-play-scraper” and for app store we used “app-store-scraper”.



## What is the distribution of ratings?

With the help of pandas and Matplotlib here is the distribution of ratings in both stores.

<img width="402" alt="gp1" src="https://user-images.githubusercontent.com/66030548/235307008-a718058f-5c63-40c7-8ecb-8ce49d83fe96.png">

<img width="389" alt="as1" src="https://user-images.githubusercontent.com/66030548/235307017-5297c9ae-55a4-47f0-8307-21c87e96150e.png">


As we can see most of the Android users rated 5-star rating which shows the app is going good. While the app store app for iphone users might have some issues as many rated it 1.

## What is average rating trend over the years?

Also, we can see the trend of avg ratings over the years for both stores

<img width="385" alt="gp2" src="https://user-images.githubusercontent.com/66030548/235307024-8a5515af-f0eb-40dd-b96f-4b5b9a4950e7.png">

<img width="382" alt="as2" src="https://user-images.githubusercontent.com/66030548/235307028-b28d625d-b10a-4494-b5c2-1fac02193c1c.png">


## How many negative reviews app team has addressed?
Let's look at the sentiments of the reviews. 

<img width="278" alt="gp3" src="https://user-images.githubusercontent.com/66030548/235307153-c6b8d62c-b552-42ef-861c-74794847dc8c.png">

<img width="272" alt="as3" src="https://user-images.githubusercontent.com/66030548/235307157-cdd78ea2-4a8d-4482-99e6-1c0b33355516.png">


We can see 70% of the reviews are positive for the Android app and 25% are negative. 
Whereas for ios apps it is 70% negative and 20% are positive which shows ios app have some major issues.

## What are sentiments distibution among the reviews?

Now let's look at how many negative reviews have been replied to by the app team on both stores.

<img width="263" alt="gp4" src="https://user-images.githubusercontent.com/66030548/235307175-5f549ff5-5bc5-45c2-9fdb-f0ebcc874181.png">

<img width="260" alt="as4" src="https://user-images.githubusercontent.com/66030548/235307182-50e5e98b-b970-4be3-8c32-5c6c06542a2d.png">

So here we can see on the google play store 60% of the reviews had been answered which is decent as many reviews don’t have sensible text. But on app stores, only 37% are answered which is bad.

## What topics arrre mostly mentioned in reviews?

Now we need to dig into reviews and get idea of what eviews are saying. For this we used pretained model Yet Another Keyword Extraction(YAKE) for extracting keywords.

Let’s look fo Google play store reviews for Loco app.

### Google play store reviews for Loco app.

Positive reviews:

<img width="400" alt="gp5_11" src="https://user-images.githubusercontent.com/66030548/235307192-27c7cb19-81cc-4f53-985a-f505eec88531.png">

<img width="700" alt="gp5_12" src="https://user-images.githubusercontent.com/66030548/235307200-81d78e0f-dbde-4968-b833-e288620f27b5.png">

From this we can see most of the positive reviews talk about 'earning money', 'pubg' and 'free fire' game streaming which are popula games amoung young people.

Negative reviews:

<img width="400" alt="gp5_21" src="https://user-images.githubusercontent.com/66030548/235307218-9cc935c7-52fa-4fa5-b5fd-f2d127f330fb.png">


<img width="700" alt="gp5_22" src="https://user-images.githubusercontent.com/66030548/235307229-9290cad8-3fda-4bc9-9e93-e9e0338abdc2.png">

From this we can see most negative reviews are about redeeming 'rewards' or using 'gift cards'. Some are about login issues.

### App store reviews for Loco app:

Positive reviews:

<img width="400" alt="as5_11" src="https://user-images.githubusercontent.com/66030548/235307243-1fe71529-68f9-400c-9135-a40a658475bf.png">


<img width="700" alt="as5_12" src="https://user-images.githubusercontent.com/66030548/235307251-b33b9b20-abd6-4cfd-8851-38d95e8e5b25.png">


Negative reviews:

<img width="400" alt="as5_21" src="https://user-images.githubusercontent.com/66030548/235307258-156e9fde-135e-4567-a2ef-89bd9ae28cec.png">

<img width="700" alt="as5_22" src="https://user-images.githubusercontent.com/66030548/235307264-85ea7743-27a3-46c3-9f3e-52a967f96f45.png">

For ios we can't get lot of insight as they are only around 900. Positive reviews are vey few. Negative are mostly about unable to see stream, full screen not working, device related, and money related.


## Conclusion

Android app:

From above analysis we can see that apart from some issues Android app is doing good. 70% users are happy with app. Users mostly liking free fire and bgmi streams. So loco can partner with more tournament organisers to stream competitions on their platform. Also the earning money while watching is also liked by users. There moght be some bugs related to claiming reward and using google/ amazon gift cards. So team should look into it.

ios app:

There are not many reviews to analyse but most of the users are not happy about it. There are lots of bugs like stream not showing, full screen not working and more. Team need to look into app deeply and solve the poblems.

