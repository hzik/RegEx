# RegEx extension

With this custom element you can extend the Text element by a regular expression for its validation.

![screenshot](https://amend.cz/regex.gif)

## Setup

1. Configure a new custom element in your content type
2. Make the custom element *Required* 
3. Specify the *Text* element the regular expression is for (in both "Allow the custom element to read values of specific elements" and its codename as "element" JSON parameter)
4. Specify a regular expression you want to test against the *Text* element in the "regex" parameter
5. (optional) Add additional parameters (in "valid" and "invalid" parameters for messages that get displayed when the regular expression match/doesn't match the *Text* value)

When the validation fails you won't be able to publish the item until you meet the validation rules. Since the custom element is the one that is required you need to fix respective *Text* element to pass the validation.

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
