## Project Lesson Notes

- In this project we worked with a third party free API called ExchangeRateAPI.

- Fetch is used to make HTTP requests to a backend from your frontend in order to get your data.

- A .json object is very similar to a JavaScript object we have key-value pairs inside of curly braces.

- The difference is that we use ""

- There are different types of HTTP requests, when we are just taking data from a server it tipically will be a GET request.

- If we are posting data to the server, meaning like we are filling out a form that is going to be saved in a backend database this tipically will be a POST request.

- If we are updating data on a server it will be a PUT or PATCH request, if we are going to delete is a DELETE request.

- With fetch API if you want the data, you have to format the function that .then receives and format it to what you want, according to the example, you want the .json information.

`function calculate() {fetch('items.json').then(res => res.json()).then(data => console.log(data));}`

- If we want to "print" into the screen the content of the fetched .json file, we can do something like this:

`function calculate() {`
`fetch('items.json')`
`.then(res => res.json())`
`.then(data => (document.body.innerHTML = data[0].text))`
`;`
`}`


