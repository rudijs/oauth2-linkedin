# oauth2-linkedin

[![Build Status](https://travis-ci.org/rudijs/oauth2-linkedin.svg?branch=master)](https://travis-ci.org/rudijs/oauth2-linkedin)
[![Coverage Status](https://coveralls.io/repos/rudijs/oauth2-linkedin/badge.svg?branch=master&service=github)](https://coveralls.io/github/rudijs/oauth2-linkedin?branch=master)
[![Dependencies Status](https://david-dm.org/rudijs/oauth2-linkedin.svg)](https://david-dm.org/rudijs/oauth2-linkedin.svg)

Serverside Oauth2 LinkedIn Signin using Node.js

## Overview

Node.js oauth2 Facebook sign in module.

If you want or need to roll-your-own Facebook login this module with help with the user sign in and get profile.
 
Once you have the user's profile, in JSON format, saving it to your database of choice is then up to you.

## Requirements

Needs node v12.x or > iojs-v1.x

This module uses Promises and Generators. The author's intended case use is within KoaJS.

## API

signInUrl => Returns a Facebook Oauth sign in URL to send the user to.
 
getAccessToken => With the code returned from signInUrl, request a Facebook API access token.
 
getProfile => With the access token returned from getAccessToken, request the user profile.

## Usage

Setup/Configure your [LinkedIn App](https://developer.linkedin.com/docs/oauth2)

Use `signInUrl` in your routes to send the user to sign in with facebook.com.

Use `getAccessToken` and `getProfile` in your controller to retrieve the user profile from facebook's API.

Also review the test code, `*.spec.ts`, files in the github.com source repo.

Code review, suggestions and pull requests are welcome - thanks.
