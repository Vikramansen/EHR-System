EHR_Health_Systems:

EHR_Health_Systems is a comprehensive Electronic Health Record (EHR) system designed as a course project for Clinical Decision Support Systems. It's developed leveraging the powerful FARM stack to offer robust, scalable, and responsive functionalities tailored for health professionals and patients alike.

Stack Components:

Backend: Developed using FastAPI, ensuring rapid, effective, and type-safe APIs.
Frontend: Implemented using ReactJS, offering a dynamic and intuitive user interface.
Databases: Presently considering MongoDB for flexible, document-based data storage.
Media Dataset: Media objects, like images, will be stored using Amazon S3 or Infura IPFS, ensuring scalability and security.
Primary Development Tools:

uvicorn: To serve the FastAPI application swiftly and efficiently.
motor: Bridging the gap between FastAPI and MongoDB for seamless data operations.
Setting Up:

To get the system up and running, follow the steps below:

1. Backend Setup:
   bash conda create -n mhi_few_shot python=3.10 conda activate mhi_few_shot pip3 install fastapi uvicorn motor pip3 install torch torchvision torchaudio

2. MongoDB Configuration:

- Sign up on MongoDB Atlas and install MongoDB Compass, MongoDB Shell, and MongoDB Community Server.
- Use the provided URI to establish a connection between the server and atlas.

3. Frontend Setup:
   bash cd frontend npm cache clean -f sudo npm install -g n sudo n latest npm install npm start

4. FastAPI Execution:
   bash cd backend uvicorn main:app --reload
