#### The following is a README for a private repository of a backend assessment (code 'interview') I completed for Hatchways.io. (It also includes some changes after it was submitted). The company asks that solutions to the backend assessment not be hosted publicly as they use this assessment for many different people. I have hosted the code privately on github and could make it available if needed. 

#

## Backend Assessment for Hatchways.io
Written in Javascript     
See Back-end Assessment.pdf for assessment details.
#
## Summary of Tasks:

[x] Task 1: Create api/ping route which returns successful status code **(index.js)**   
*   Ex: of valid route:
*   http://localhost:3000/api/ping

[x] Task 2: Create api/posts route which takes in mandatory tag(s) and can optionally take in sortBy and direction. Response must combine requests but return unique objects which are sorted correctly. Error codes must be sent back for absent tags or invalid sortBy/direction parameters. **(index.js)**  
*  Ex: of valid routes/requests:
*  http://localhost:3000/api/posts?tags=tech
*  http://localhost:3000/api/posts?tags=tech&sortBy=id
*  http://localhost:3000/api/posts?tags=tech&direction=asc
*  http://localhost:3000/api/posts?tags=tech&sortBy=popularitydirection=desc

[x] Task 3:  Unit tests - utilizing Jest - **(index.test.js)**  
[x] Task 4: Bonus- implement a server side cache
*   **apicache** is used as the server side cache. Times in Postman go from 600-700 ms for return of data to 4-6 ms with use of the cache. A duplicate unit test is provided in **index.test.js** to compare times in ms.

#
## This project uses:
* Node.js: v18.2.0               -- https://nodejs.org/en/
* Express: 4.18.1                 -- https://www.npmjs.com/package/express
* Jest: 28.1.0                    -- https://www.npmjs.com/package/jest
* apicache: 1.6.3                -- https://www.npmjs.com/package/apicache

#
## Instructions:
* In the terminal/project directory type "npm install"
* Type "node index.js" to start server at http://localhost:3000/
* Interact with step one (http://localhost:3000/api/ping) and step two (ex: http://localhost:3000/api/posts?tags=tech,history,culture,science&sortBy=popularity&direction=desc)
* Utilize "npm test" to see unit test results
