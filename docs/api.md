**Get Dimension List**

Returns a list of dimensions recorded in the system

----
/api/dimension


* **Method:**
  
  `GET` 
  
*  **URL Params**

	None

* **Data Params**

	None
 
* **Success Response:**
  
  * **Code:** 200 <br />
    **Content:** 
	
	`{
  "error": false,
  "error_code": 0,
  "dimensions": [
    {
      "id": 1,
      "name": "Development Methods",
      "description": "Different methods like Scrum, Kanban, Waterfall etc. used by different teams"
    },
    {
      "id": 2,
      "name": "Product Maturity",
      "description": "Split across infrastructure, current or re-engineering products etc"
    },    {
    {
      "id": 3,
      "name": "Integrated Development Environment (IDE)",
      "description": "Development environments category, used by vast majority of the organization."
    }
   ]
}`
 
* **Error Response:**

  None
  
* **Sample Call:**

  ```javascript
	    var url = 'api/dimension' ;
		return $http({
			url: url,
			method: "GET",
		})
		.then(function(response) {
				// success
				return response;
		}, 
		function(response) { // optional
				// failed
				return response;
		});
  ```
* **Notes:**

	None 
  

----
