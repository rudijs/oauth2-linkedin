# oauth2-linkedin

[![Build Status](https://travis-ci.org/rudijs/oauth2-linkedin.svg?branch=master)](https://travis-ci.org/rudijs/oauth2-linkedin)
[![Coverage Status](https://coveralls.io/repos/rudijs/oauth2-linkedin/badge.svg?branch=master&service=github)](https://coveralls.io/github/rudijs/oauth2-linkedin?branch=master)

Serverside Oauth2 LinkedIn Signin using Node.js

## Overview

Node.js oauth2 Facebook sign in module.

This module is written in Typescript, uses Promises and the author's intended case use is with KoaJS.

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
