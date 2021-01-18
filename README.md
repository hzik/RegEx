# RegEx

This custom element allows you to add regular expression for your Text element.

![screenshot](https://amend.cz/regex.gif)

## Setup

1. Configure a new custome element in your content type (either directly below the TExt element if you want to give additional information to your editor or to separate content group)
2. Make the custome element Required
3. Specify the Text element the regular expression is for
4. Add additional parameters

![screenshot](https://amend.cz/configuration.png)

## Deploying

Netlify has made this easy. If you click the deploy button below, it will guide you through the process of deploying it to Netlify and leave you with a copy of the repository in your GitHub account as well.

[![Deploy to Netlify](https://www.netlify.com/img/deploy/button.svg)](https://app.netlify.com/start/deploy?repository=https://github.com/hzik/RegEx)

## Configuration

You can specify the Parameters {JSON} part of the configuration to configure the default state or a lable.
Possible configurations:

```json
{
    "element": "name",
    "regex": "^([a-z0-9]{5,})$",
    "valid": "",
    "invalid": "Name is too short, please type at least 5 characters."
}
```
