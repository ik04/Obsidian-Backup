
# Api Docs:
## Org Search Endpoint
## Org Entity Endpoint
## Autocomplete Endpoint

## Use Cases:
research and refer gpt, yt, stackoverflow
## bing chat:
1. **Company Profiles**: Display detailed profiles of companies, including their funding rounds, key people, and recent news.
2. **Investor Tracking**: Track the activities of investors, their portfolio companies, and their investment trends.
3. **Industry Trends**: Analyze industry trends based on funding rounds, acquisitions, and IPOs.
4. **Job Listings**: Use the data to list job openings at various companies.
5. **Networking**: Help users find potential business partners or competitors.
6. **Event Calendar**: Display upcoming industry events.



[To track the activities of investors, their portfolio companies, and their investment trends using the Crunchbase API, you would typically use the `/entities/organizations/{permalink}` endpoint](https://data.crunchbase.com/docs/using-the-api)[1](https://data.crunchbase.com/docs/using-the-api)

The `{permalink}` in the endpoint would be the unique identifier for the investor whose activities you want to track. [This endpoint will return detailed information about the organization, including its investments](https://data.crunchbase.com/docs/using-the-api)[1](https://data.crunchbase.com/docs/using-the-api).

For example, if you wanted to track the activities of an investor with the permalink ‘sequoia-capital’, your API request would look like this:

```
GET https://api.crunchbase.com/api/v4/entities/organizations/sequoia-capital?user_key=INSERT_YOUR_API_KEY_HERE
```

[Remember to replace `INSERT_YOUR_API_KEY_HERE` with your actual API key](https://data.crunchbase.com/docs/using-the-api)[1](https://data.crunchbase.com/docs/using-the-api).

[You can also use the `/search/organizations` endpoint to search for organizations (including investment firms) based on certain criteria](https://medium.com/priyanshumadan/extract-data-from-crunchbase-api-using-python-8e99ed6bc73e)[2](https://medium.com/priyanshumadan/extract-data-from-crunchbase-api-using-python-8e99ed6bc73e). This could be useful for identifying new investors or investment trends.

Please note that you’ll need to refer to the [Crunchbase API documentation](https://data.crunchbase.com/docs/using-the-api) [for more details on how to structure your API requests and handle the responses](https://data.crunchbase.com/docs/using-the-api)[1](https://data.crunchbase.com/docs/using-the-api).


**Listing Job Openings**: The Crunchbase API does not directly provide job listings. [However, you can use the `/entities/organizations/{permalink}` endpoint](https://data.crunchbase.com/docs/using-the-api)[1](https://data.crunchbase.com/docs/using-the-api) [to get detailed information about an organization, including its size and industry](https://data.crunchbase.com/docs/using-the-api)[1](https://data.crunchbase.com/docs/using-the-api). You can then use this information to infer potential job openings or direct users to the organization’s careers page.


 **Displaying Upcoming Industry Events**: The Crunchbase API does not directly provide information about upcoming events. [However, you can use the `/entities/organizations/{permalink}` endpoint](https://data.crunchbase.com/docs/using-the-api)[1](https://data.crunchbase.com/docs/using-the-api) [to get detailed information about an organization, including its recent news](https://data.crunchbase.com/docs/using-the-api)[1](https://data.crunchbase.com/docs/using-the-api). You can then parse this news for mentions of upcoming events.


## Todo:
- [x] api integration 
- [x] lookup orgs
- [x] use the api folder for calling crunchbase (api key hide)

## Approach:
- get all search results 
- let the user select a card 
- add load more (optional)
- on selecting save the perma link and if perma link exists in db hydrate the page with crunchbase details


## Response Body:
facet_ids: Array(3) [ "company", "rank", "builtwith" ]

0: "company"

1: "rank"

2: "builtwith"


identifier: 

entity_def_id: "organization"

image_id: "v1397194627/71161f85b6d660ea70a32d08d767ce7a.png"

permalink: "zaggle"

uuid: "fc8ff3cd-54d5-9f93-fbd6-87ced978c451"

value: "Zaggle"

short_description: "Zaggle is the specialist that helps with DIY, gardening, and technology."