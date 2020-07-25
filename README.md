# App-Store-Reviews
<h2> What does it do </h2>
Extracts reviews of an app from App Store and saves them into json file (specifically date, rating, title, and content of each review).<br/>
The json
Makes further manipulation of this data easier.

<h2> How to use it </h2>
First find the app id and the two-letter code of the country where you would like to see App Store reviews.<br/>
        - The app id is found at the end of its App Store link (e.g. in ht<span>tps://apps.</span>apple.com/app/wei-xin/id414478124 (WeChat), "414478124" is the id of this app.)<br/>
        - Here is a comprehensive list of country codes: https://gist.github.com/daFish/5990634<br/>
<br/>
There are three ways of extraction:<br/>

~~~~
get_reviews_on_page(country, page, app_id, sort_by='mostRecent', out_filename='reviews.json')
get_reviews_on_pages(country, from_page, to_page, app_id, sort_by='mostRecent', out_filename='reviews.json')
get_all_reviews(country, app_id, sort_by='mostRecent', out_filename='reviews.json')
~~~~

By default, they sort by the most recent and save reviews in a file called "reviews.json".
<br/><br/>
Simply add function calls in the file, or import the functions to your own file and call them.
