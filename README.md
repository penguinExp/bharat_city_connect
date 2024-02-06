# Bharat City Connect 🇮🇳

Welcome to Bharat City Connect, your one-stop destination for detailed geographical information
about different states and cities across Bharat 🇮🇳! This repository contains JSON files filled with
valuable data that will help you understand the layout of our diverse country better.

## Overview

The goal of this API is to provide an easy-to-use yet comprehensive collection of state and city data,
facilitating smooth integration into applications and projects requiring such details.

By promoting awareness and accessibility, I aim to strengthen the bond between every corner
of Bharat 🇮🇳.

## Documentation

### Base API URL

The base URL for the API is as follows:

```bash
https://adityamotale.github.io/bharat_city_connect/api/
```

You may use this base URL to construct specific endpoint paths for fetching desired data sets.

### Accessing State Data

To obtain all available states, simply navigate to:

```bash
https://adityamotale.github.io/bharat_city_connect/api/bharat.json
```

The response format will resemble this example output:

```js
[
  {
    "state_name": "Andaman_and_Nicobar_Islands"
  }
  // ...other states follow here
]
```

### Retrieving City Information

Once you acquire the name of a particular state from the master list (accessed via `<base_url>/bharat.json`),
you can proceed by appending its name (without spaces or special characters) to the following path:

```bash
https://adityamotale.github.io/bharat_city_connect/api/states/{state_name}.json
```

Replace `{state_name}` with the actual state name you wish to explore further.

For instance, if you want to find out which cities belong to the Andaman & Nicobar Islands,
query the respective endpoint below:

```bash
https://adityamotale.github.io/bharat_city_connect/api/states/Andaman_and_Nicobar_Islands.json
```

The corresponding response will look like this:

```js
[
  {
    "city_name": "Port Blair"
  }
  // ...other cities follow here
]
```

For more information or to report issues, please open a PR or Issue with your proposed changes.

Happy exploring 🇮🇳!
