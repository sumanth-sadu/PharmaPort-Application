# PharmaPort-Application

# SOAD

We present before you the Pharmaport website. (we care, for your health)
Business plan
the website provides the facility to store all the medical records like prescriptions given by doctors, scanned copies of X-rays, CT-scan, MRI and everything related to reports of a person from birth to present in digital format.

## Example
***Let us see an example to make the idea clear :
Murali, a 25 year old boy, has a skin problem, so he booked an appointment and went to Apollo hospital. The receptionist takes his phone number and a unique code generated by our website. The receptionist gives the details of murali along with unique code of respective doctor to authorisation service. Which in turn connects the doctor and patient by giving the doctor access to patients medical records on successful verification. Now when the doctor is about to prescribe medicines he fills in a form along with timelines. Now muralis website account is updated with prescriptions and test reports given by the doctor. Murali can also rate the doctors and give feedback to the hospital services.

I hope the example shows how helpful was Pharmaport to murali 
*

Userpage is considered to be the heart of the website, it is where the user uploads and makes necessary changes to his health reports, rate and give back feedback for doctors and have a collection of all the prescriptions given.

### Web Services :
#### Services we use are using : 
- For Payment we use stripe API which doesn’t share the card details with the website and helps through data breach.
- For Storage of uploaded files we are using Amazon s3 bucket which is a cloud service and a cost efficient way of storing files as the cost depends on the usage and not fixed. Provides more flexibility. 
- Authentication through Google authenticator API as this is secure than using otp authentication.
- And Robot checking for recaptcha to keep away malicious software from engaging in abusive activities on this website.

#### Services which we providing are : 
- Doctor authentication
Doctor id is sent along with user generated pin which returns a secret key which is a unique 128bit coe that don't repeat and generated by uuid library for communication of user data like reports to doctor
- Get Data 
With the key obtained above one can get the patient data
- Post Data
With the obtained key above a doctor can post report under user
- Get Dataset
We decided to provide dataset of medical records(if patient agerees for open sourse community to enhance human lives. By entering file names they can obtain all files with that name
- Doctor rating
Webservice for 3rd party websites to use the rating provided by user from our websites.
One should provide doctor id or hospital
- Prescription 
Prescription details as a dataset for others to gain knowledge. 
