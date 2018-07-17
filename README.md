# React-Static-Website-Builder

This is a Laravel/Spark application which communicates between bitbucket and Netlify to dynamically generate react-static sites after payment. After account creation, but before subscription the user enters in fields of data such as company name, address, logo, ect to populate the JSON for their website. Once payment is processed, authentification is requested from both bitbucket and netlify. Afterwards, netlify pulls down the repo and initiates the build commands passed in the WebsiteController.pho. This saves a local json file with a unique user ID that is referenced on yarn build, which makes sure the user JSON data is correctly passed.