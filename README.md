# study_on_inapp_ads
For this project, I'll pretend I'm working as data analysts for a company that builds Android and iOS mobile apps. This company make their apps available on Google Play and the App Store.  They only build apps that are free to download and install, and their main source of revenue consists of in-app ads.

They only build apps that are free to download and install, and their main source of revenue consists of in-app ads. This means our (the company I work for) revenue for any given app is mostly influenced by the number of users who use our app — the more users that see and engage with the ads, the better. Our goal for this project is to analyze data to help our developers understand what type of apps are likely to attract more users.

To do this, we'll need to collect and analyze data about mobile apps available on Google Play and the App Store.

As of September 2018, there were approximately 2 million iOS apps available on the App Store, and 2.1 million Android apps on Google Play, based on Statista's data.

I will be using two datasets from kaggle:

A data set containing data about approximately 10,000 Android apps from Google Play; the data was collected in August 2018 → https://www.kaggle.com/lava18/google-play-store-apps

A data set containing data about approximately 7,000 iOS apps from the App Store; the data was collected in July 2017 → https://www.kaggle.com/ramamet4/app-store-apple-data-set-10k-apps

It is important to clarify a few things in the header's row for the latest of those two. Unlike Google play's header row, AppleStore header row is not as clear, as you can see here:

['id', 'track_name', 'size_bytes', 'currency', 'price', 'rating_count_tot', 'rating_count_ver', 'user_rating', 'user_rating_ver', 'ver', 'cont_rating', 'prime_genre', 'sup_devices.num', 'ipadSc_urls.num', 'lang.num', 'vpp_lic']

That list represents all the columns this dataset has, so I will explain the ones that I think are more difficult to grasp:

rating_count_tot: User Rating counts (for all version)
rating_count_ver: User Rating counts (for current version)
user_rating_ver: Average User Rating value (for current version)
ver: Latest version code
cont_rating: Content Rating
sup_devices: Number of supporting devices
ipadSc_urls.num: Number of screenshots showed for display
lang.num: Number of supported languages
vpp_lic: Vpp Device Based Licensing Enabled
