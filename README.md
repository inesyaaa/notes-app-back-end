# NutriMatch-CloudComputing Documentation

- ## 1. Write the Flask server app using Python & Install prequisite
    - Source Code for Flask Server:
https://github.com/NutriMatch/NutriMatch-CloudComputing.git
 
- ## 2. Setup Google Cloud Platform
    - Enable Cloud Run and Cloud Build API
 
 
- ## 3. Set up the required environment variables
    ```sh
      pip install -r requirements.txt
    ```
- ## 4. Build the container image using the provided Docker file
    - https://cloud.google.com/run/docs/quickstarts/build-and-deploy#containerizing

- ## 5. Deploy the container image to Cloud Run
    ```sh
      gcloud builds submit --tag gcr.io/<your_project>/nutrimatch
    ```
    ```sh
      gcloud run deploy --image gcr.io/<your_project>/nutrimatch --platform managed
    ```
- ## 6. Configure databases using Firebase Authentication, Realtime Database, and Storage

- ## 7. Connect all services to one domain using API gateway
    ### REST API Documentation
    NutriMatch REST-API: App to Database
    #### How to Use
    - Local Host: Run with python, local IP and Port:5000 
    `http://127.0.0.1:5000/` or `http://localhost:5000/`
    - Online Domain: `https://nutrimatch-api-3yfsigu4tq-et.a.run.app/` 

    #### Endpoint Route
    For API documentation, see the following link: \n
    [NutriMatch-API Documentation](https://documenter.getpostman.com/view/26516803/2s93m7W1de)
    
