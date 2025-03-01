# Cloud Computing

# updated todos:

- make API documentation
- make deployment documentation
  - firebase
  - cloud run
    - ml
    - backend
- ✅ deploy backend
- optional - validate requests first before able to hit endpoint (https://simonplend.com/how-to-handle-request-validation-in-your-express-api/)

# done

- ✅ implement auth (jwt)
- update user and job endpoints so a POST response have properties of:
  - user:
    - ✅ timestamp
    - ✅ profilePhoto
      - link from cloud storage
    - ✅ Contact
      - Phone
      - Email
      - Links
        - Linkedin
        - Github
        - etc
  - job:
    - ✅ timestamp
    - ✅ Contacts
      - Email
      - Phone
      - HR Contact
- problems:
  - ✅ getAllUser response isn't formatted correctly
  - ✅ getAllJobsOfOneUser is broken
  - ✅ because registeredUser and userData is seperated we need to also delete registeredUser in db when deleting userData
- make update and delete endpoints for:
  - update:
    - user:
      - ✅ update a user (profile)
    - job:
      - ✅ update a job
  - delete:
    - user:
      - ✅ a user
    - job:
      - ✅ a job
      - ✅ all job of one user

# TODOS:

- implement JWT for auth (go to firebase auth)
- make database
  - express + cloudSQL https://austinhale.medium.com/building-a-node-api-with-express-and-google-cloud-sql-9bda260b040f
  - express + firebase + cloud functions https://medium.com/@savinihemachandra/creating-rest-api-using-express-on-cloud-functions-for-firebase-53f33f22979c
  - Table:
    - Jobs data
      - Job title
      - Company name
      - Alamat
      - Desc
      - Kualifikasi
      - Contacts
        - Email
        - Phone
        - HR Contact
    - Users data
      - CV
        - link
      - Photo
        - Links from cloud storage
      - Name
      - Username
      - Passwords
      - Description
      - Skills
      - Alamat
      - Contact
        - Phone
        - Email
        - Links
          - Linkedin
          - Github
          - etc
- make api
