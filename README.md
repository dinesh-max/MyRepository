# WebApiVersioning
In today's fast paced agile environment we may need to support various clients with different requirements, so we need a mechanism through which we could serve all the new clients   along with our existing clients.To solve this problem I have implemented Api Versioning using Asp.Net Core 3.1,through this we can pubish different version of our API.

In order to consume this API, you can pass the api-version in header or in query string as per the requirment.
We can configure the API method to accept the api-version in URL  as well ,using the [Route()] attribute, but thats not recommended keeping the Rest Principles in mind.
However, if you dont pass the api-version , in this implementation '1.0' is being passed as the default version of the api.
You can keep adding new api methods and map them to different versions of the Api, those methods would be available to consume when specific version will be passed
Below the screenshot of postman tool where api-version is passed in header.
![Postman_Consume API_VersionInHeader](https://user-images.githubusercontent.com/62199837/118390934-59c9c880-b64f-11eb-96d1-644180a47efa.PNG)
