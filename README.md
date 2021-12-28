# Getir CASESTUDY

## Heroku
The project is on live.

https://patika-mfcicek-getir-casestudy.herokuapp.com/docs/
## Installation
1. Clone the repo 
   ```
    git clone https://github.com/mfcicek/patika.dev-getir-casestudy.git
   ```
2. Install NPM packages
   ```
    npm install
   ```
3. Rename .env.example file as .env
   
## Usage
Run the command to start the app
   ```
   npm run-script start-dev
   ```
Run the command for integration test
   ```
   npm run test:integration
   ```
Run the command for unit test
   ```
   npm run test:unit
   ```
## Endpoints
`POST /records`
</br>
<h4>Parameters</h4>
<table>
<thead>
<tr>
<th align="left">Name</th>
<th align="center">Type</th>
<th align="left">Description</th>
<th align="left">Optional</th>
</tr>
</thead>
<tbody>
<tr>
<td align="left">startDate</td>
<td align="center">date</td>
<td align="left">Start date of records, Format : YYYY-MM-DD</td>
<td align="left">Optional</td>
</tr>
<tr>
<td align="left">endDate</td>
<td align="center">date</td>
<td align="left">Finish date of records, Format : YYYY-MM-DD</td>
<td align="left">Optional</td>
</tr>
<tr>
<td align="left">minCount</td>
<td align="center">string, integer</td>
<td align="left">Minimum number of total count</td>
<td align="left">Optional</td>
</tr>
<tr>
<td align="left">maxCount</td>
<td align="center">string, integer</td>
<td align="left">Maximum number of total count</td>
<td align="left">Optional</td>
</tr>
</tbody>
</table>

### Documentation
The project is documented with Swagger.

resource: https://www.borakasmer.com/nodejs-uzerinde-swagger-entegrasyonu/

### Validation 
We used Joi library to validate incoming request. 

resource: https://jasonwatmore.com/post/2020/07/22/nodejs-express-api-request-schema-validation-with-joi

### Error Handling
Centralized error handling is used. We have a middleware that catches all errors.

resource: https://sematext.com/blog/node-js-error-handling/
