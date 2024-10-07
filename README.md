# Postman-Collection-Alphabetiser
Sort your Postman collection alphabetically.

(Works with sub-folders)

How to use:

(You don't need to fork from GitHub, this exists in a Postman workspace... To fork, click the link below.)

* [Fork the collection.](https://www.postman.com/dark-matter-505283/workspace/057f1c28-df06-4e91-b583-25c7600d680c/documentation/23596470-5d8fcf87-eaf6-4d2e-9058-9dd550e6cfe2)
* Open the collection level variables.
* Enter your Postman API Key.
* Enter the 'Collection ID' for the collection you want to sort.
* Enter the 'Workspace ID' where the collection being sorted is stored.
* Leave the 'JSONBODY' variable blank, this will be automatically populated.
* Run the collection via the 'Collection Runner'.

---

This collection utilises postman.setNextRequest("request_name");

This means that we need to run the collection via the 'Collection Runner' option.

If the collection is not run this way, the setNextRequest will not be triggered.

---

Once the correct information has been entered and the collection runner triggered, the collection will pull in the JSON response from the 'GET' call and sort it using the JavaScript inside the 'Tests' tab.

Once sorted it will pass the output to the 'Create new alphabetised collection' POST request, where a new collection will be created from the sorted data.

Then finally, the original collection will be deleted.
