# TripleTen_AB_test
## Purpose of the test: testing changes related to the introduction of an improved recommendation system

## Technical description:
- Purpose of the test: testing changes related to the introduction of an improved recommendation system
- Expected result: within 14 days of signing up, users will show better conversion into product page views (the `product_page` event), product card views (`product_card`) and purchases (`purchase`). At each of the stage of the funnel `product_page → product_card → purchase`, there will be at least a 10% increase

## Main Conclusions:
- * Conversion funnel shows that round 30% of users are makning purchases in the end, which is quite high conversion rate
* 6.1% of users took part in both tests and were excluded from further calculations
* Most users are performing 6 actions on a website
* Since test B is applied we can see that share of android users is slightly increasing, compared to other devices
* We can see from pie charts above that most users are from EU region for `recommender_system_test` (round 95%) and `interface_eu_test` has only european users
* Share of users from the EU region from all new users from the EU region is 21.8%
* There was 1 event which was active during the test being conducted and it probably affected our test results: 'christmas&new year promo' was running for eu and n.america regions, and we still see that most of the clients are from EU
* According to the technical requirements we are supposed to run `recommender_system_test` with groups А (control) and B (new payment funnel) having 6000 expected test participants, but there are less than 4000 participants for `recommender_system_test` so we are  analysing both tests keeping in mind that we dont have enough users for `recommender_system_test` in group B
* Launch date is 2020-12-07 (same we can see from the graph above), while the date when they stopped taking up new users is 2020-12-21 according to technical requirements, but we see that new users were coming up untill 2020-12-23 so all the users were kept
* End date is 2021-01-01 according to tech description but we see 0 info after 2020-12-29, looks like there was a tech issue and some of data havent been saved
* Expected result: within 14 days of signing up, users will show better conversion
* After doing EDA and A/B testion I can say that I wouldn't trust the way the test was planned and executed (which means that the results from users who signed up after the 2020-12-15 are questionable statistically wise)
* Suggestion is to admit test was a fail and continue with other projects.
