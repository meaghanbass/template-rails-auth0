# TEMPLATE - Rails & Auth0 App
[Full Tutorial](https://auth0.com/docs/quickstart/webapp/rails/01-login)

## Running the Sample Application
In order to run the example you need to have ruby installed.

Register `http://localhost:3000/auth/auth0/callback` as `Allowed Callback URLs` in your client setting in [Auth0's dashboard](https://manage.auth0.com/#/).

You also need to set the Client Secret, Client ID, Domain and Callback URL for your Auth0 app as environment variables with the following names respectively: `AUTH0_CLIENT_SECRET`, `AUTH0_CLIENT_ID`, `AUTH0_DOMAIN` and `AUTH0_CALLBACK_URL`.

Set the environment variables in `.env` to match those in your Auth0 Application Settings.

````bash
# .env file
AUTH0_CLIENT_ID=YOUR_CLIENT_ID
AUTH0_CLIENT_SECRET=YOUR_CLIENT_SECRET
AUTH0_DOMAIN=<YOUR_TENANT>.auth0.com
AUTH0_CALLBACK_URL=http://localhost:3000/auth/auth0/callback
````
Once you've set those 4 environment variables, run `bundle install` and then `rails s`. Now, browse [http://localhost:3000/](http://localhost:3000/).
__Note:__ Remember that you need to have `./bin` in your path for `rails s` to work.

Shut it down manually with Ctrl-C.

__Note:__ If you are using Windows, uncomment the `tzinfo-data` gem in the gemfile.

