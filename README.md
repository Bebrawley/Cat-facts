![CatCat](http://www.readersdigest.ca/wp-content/uploads/2016/05/sickcat.jpg)

# Cat API
This is the Cat API and it provides Cat facts as a service CatCat :Cat:

## Add to Slack
Soon to come

This will enable two things:

- One daily random fact posted in the channel you select.
- A Slack slash command (`/dogfact`) to retrieve a single fact on any channel.

If installation was successful you'll receive a welcome message :)

### Privacy Policy
Dog Facts is just for fun. The only data retained by Dog Facts is your team webhook url (which is required to post Dog Facts messages to your Slack). Otherwise, no data is kept.

For questions or support, please email `el@kinduff.com` or contact directly through Twitter `http://twitter.com/kinduff`

## Use it as an API

**Live endpoint:** `http://dog-api.kinduff.com`

| Path         | Description  | Parameters
| ------------ | ------------ | ----------
| `/api/facts` | Returns an object with dog facts | `?number=5`

## Host it yourself
First make sure you have the following dependencies installed.

- Ruby greater than 2.3.0
- SQLite3

Go ahead and clone this repository.

```
git clone git@github.com:kinduff/dog-api.git
```

Then install the dependencies.

```
bundle install
```

After that you'll need to setup your database, run the following command to run migrations. 

```
rake db:migrate
```

And finally, fill out your database with the latest dog facts included in the `db/seeds.rb` file.

```
rake db:seed
```

Run the application by running the following command.

```
rake server
```

Or just `rake` by it self. The application should now be running in `http://localhost:4567`.

## Why you made this?
There's a [Cat API](http://catfacts-api.appspot.com) that returns cat facts. I like cats but I like dogs more. Equilibrium must exists.

## Sources
Lot's of places, I'll list them tomorrow, mom.
