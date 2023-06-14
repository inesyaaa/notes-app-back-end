# NutriMatch-CloudComputing Documentation

- ## 1. Write the Flask server app using Python & Install prequisite
    - Source Code for Flask Server:
    https://github.com/NutriMatch/NutriMatch-CloudComputing.git
 
- ## 2. Setup Google Cloud Platform
    - Enable Cloud Run and Cloud Build API
 
- ## 3. Set up the required environment variables
    ```sh
        python -r requirement.txt
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
    For API documentation, see the following link
