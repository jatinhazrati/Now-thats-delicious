# Now That's Delicious!

👋 there, and welcome to the repository for _Now That's Delicious!_ This project is a single page application I developed in an attempt to learn how to use JavaScript to create the backend of a site! It takes advantage of **Node**, **Express**, and **MongoDB Atlas**, and definitely keeps true to traditional **MVC** design principals.

## Using the app

Haven't you ever wanted a place to keep track of your favorite local eateries? Well this app is just for you! Upon launch, you'll be greeted a bunch of _stores_ that have been uploaded by other users. The descriptions, images, reviews, and locations are all specified by the user.

For you to get started, simply make an account by clicking on _register_. Once you set up an account you can now _add_ a new store, _edit_ an existing one, or start _reviewing_. You can review with a simple _like_ or perhaps, leave a review (along with a star-rank out of 5)! These reviews all contribute to the store's overall score on the **Top** page!

The search bar is tailored to the store name, and description allowing you to search for things like 'Coffee' or 'beer' with ease! The map will also show you all the stores in a given location, try 'Hamilton' for the best results. Lastly, incase you ever forget your password, the app has a 'Forgot your Password' work flow which will easily get you back up and running!

## How it works

This app was written almost entirely in **Node/Express** and with best practices kept through **MVC** design patterns. Express handles how we specify routes, and from there we pass the code along to `controllers` who run the middleware for each function we use.

The `controllers` use the `exports` system to control the _models_ as well as render the views. For a templating engine, we use `pug` since it integrates with helper functions, and javascript seamlessly. The models are specified in `MongoDB` and with the help of the _mongoose_ npm library, wire the data throughout the whole application.

## Sample Data

To load sample data, run the following command in your terminal:

```bash
npm run sample
```

If you have previously loaded in this data, you can wipe your database 100% clean with:

```bash
npm run blowitallaway
```

That will populate 16 stores with 3 authors and 41 reviews. The logins for the authors are as follows:

| Name          | Email (login)          | Password |
| ------------- | ---------------------- | -------- |
| Jatin Hazrati | jatinhazrati@gmail.com | jatin123 |
