## API_Advanced
 1. How to read API documentation to find the endpoints you’re looking for:
- **Endpoint Overview:** API documentation usually provides an overview of the available endpoints. Look for sections like "Endpoints," "Routes," or "Resources."

- **HTTP Methods:** Each endpoint supports specific HTTP methods (GET, POST, PUT, DELETE, etc.). This information is usually provided alongside the endpoint details.

- **Parameters:** Pay attention to the required and optional parameters for each endpoint. This includes query parameters for GET requests and request body parameters for POST and PUT requests.

- **Authentication:** Determine if the API requires authentication (e.g., API key, OAuth token, etc.) and how it should be included in the request.

2. How to use an API with pagination:
- Check the API documentation for information on pagination. It might specify a parameter (often page or offset) that allows you to request specific pages of results.

- Understand the response structure. The API will likely provide a way to know how many pages of data are available and which page you're currently viewing.

3. How to parse JSON results from an API:
- Most APIs return data in JSON format. You can use a programming language (like Python, JavaScript, etc.) to parse this data.

- In Python, you can use the json library to parse JSON. For example:
```
import json

response_data = '{"key": "value"}'
parsed_data = json.loads(response_data)
```

4. How to make a recursive API call:
- Recursion is used when you need to make a series of API calls that depend on the result of previous calls.

- Create a function that makes the API call and processes the result. Then, within the function, call itself with updated parameters.

5. How to sort a dictionary by value:
- If you have a dictionary in Python and you want to sort it by its values, you can use the sorted function along with a custom lambda function:
```
my_dict = {'a': 3, 'b': 1, 'c': 2}
sorted_dict = dict(sorted(my_dict.items(), key=lambda item: item[1]))
```

- This will produce a sorted dictionary based on the values.
