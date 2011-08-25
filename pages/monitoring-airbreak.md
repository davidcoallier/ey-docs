# Monitoring with Airbreak

This document will walk you through the basics of setting up and integrating Airbreak with your Rails 3 application.

## Setup

First go to airbrakeapp.com at setup an account. They offer a few tiers of service, including a free tier which is great for getting a feel of what Airbreak is all about.

## Integrate

Add the Airbreak gem to your Gemfile, then run bundle install.

    gem "airbrake", "~> 3.0.rc2"

## Configure

You will then need to configure Airbreak with your API key. This key is displayed on first screen when you login to Airbreak (along with the other commands listed here)

    script/rails generate airbrake --api-key [API KEY]

When you run the generate script it will throw a test error, this error should be reported by Airbreak and demonstrates  that the setup was successful.

You can run this test at anytime with the following command

    rake airbrake:test

Which can be useful to show that Airbreak is working both in development and production.

## Note: Rate Limit

It is important to note that each tier of Airbreak has a different rate limit. The free tier has a rate limit of 5, meaning it will only register 5 errors per minute. Any errors reported to Airbreak after the rate limit is reached will be ignored and discarded. 