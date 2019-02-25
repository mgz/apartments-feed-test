# Apartments feed

You need to create a feed of apartments for rent. Data about apartments provided by multiple rental agencies and may contain duplicates. A user shouldn't see duplicates in the feed. So we need to filter apartments and keep only unique results based on the priority of each rental agency.

## Example

Let's say we have rental agencies: A (priority 10) and B (priority 9). And we have the same apartments with agencies A and B. In the filtered result we should keep apartment from rental agency A since it has larger priority.

## Data

List of apartments: https://raw.githubusercontent.com/kirillplatonov/apartments-feed-test/master/apartments.yml

List of rental agencies with priorities: https://raw.githubusercontent.com/kirillplatonov/apartments-feed-test/master/rental_agencies.yml

## Task definition

Create Ruby on Rails app which will load data using links above and return apartments feed without duplicates. It should be deployed to Heroku and return feed as a table under `/feed` route.
