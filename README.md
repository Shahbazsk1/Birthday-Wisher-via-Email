# Birthday-Wisher-via-Email
<h2>This project automatically sends a personalized birthday email to friends or family if their birthday matches today's date. It reads birthday data from a CSV file, selects a random birthday message template, customizes it with the recipient’s name, and sends the email using Gmail’s SMTP server.</h2>
<h3>Main Features:</h3>
<ol>
  <li>✅ Date Matching:
    <ul>
      <li>Checks if today matches any birthdays in the birthdays.csv file.</li>
    </ul>
  </li>
  <li>✅ Custom Email Message:
    <ul>
      <li>Picks a random message from the letter_templates/ folder.</li>
      <li>Replaces [NAME] with the recipient’s actual name.</li>
    </ul>
  </li>
  <li>✅ Email Sending via SMTP:
    <ul>
      <li>Sends the email securely using Gmail (TLS encryption).</li>
    </ul>
  </li>
</ol>
<h3>🔹 Modules Used:</h3>
<ul>
  <li><b>random :</b>	Picks a random birthday letter template.</li>
  <li><b>smtplib :</b>	Used to send emails through Gmail’s SMTP server.</li>
  <li><b>datetime	:</b> Checks today’s date to match birthdays.</li>
  <li><b>pandas :</b>	Reads and parses the CSV file containing birthday data.</li>
</ul>
<h3>🔹 Folder Structure:</h3>
<p>
  📁 Birthday Wisher/<br>
  ├── main.py<br>
  ├── birthdays.csv<br>
  ├── 📁 letter_templates/<br>
  │   ├── letter_1.txt<br>
  │   ├── letter_2.txt<br>
  │   └── letter_3.txt<br>
</p>
<h3>How to Run the Project:</h3>
<ol>
  <li>Create a birthdays.csv file with correct format.</li>
  <li>Add a few letter templates like this:
    <p>letter_1.txt</p>
    <p>Dear [NAME],<br>
        Wishing you the happiest of birthdays! May your day be filled with joy.<br>
      Best,<br>
      Your Friend</p><br>
  </li>
  <li>Install dependencies:
    <p>pip install pandas</p>
  </li>
  <li>Run the script:
    <p>python main.py</p>
  </li>
</ol>
<br>
<h4>🔐 Security Note:</h4>
<p>
  MY_EMAIL = "youremail@gmail.com"<br>
  MY_PASSWORD = "your_app_password"<br>
</p>
<ul>
  <li>Never share your real Gmail password in code.</li>
  <li>Use Gmail App Passwords for this.</li>
</ul>

<h3>✅ Step-by-Step: Use Gmail App Password</h3>
<ol>
  <li>
    <strong>Enable 2-Step Verification on Your Google Account</strong><br>
    App passwords only work if 2FA is enabled.<br><br>
    Go to: 
    <a href="https://myaccount.google.com/security" target="_blank">
      https://myaccount.google.com/security
    </a><br><br>
    Under “Signing in to Google”, enable 2-Step Verification
  </li>
  <br>
  <li>
    <strong>Generate App Password</strong><br>
    After enabling 2FA, go to: 
    <a href="https://myaccount.google.com/apppasswords" target="_blank">
      https://myaccount.google.com/apppasswords
    </a><br><br>
    Select <code>Mail</code> as the app and <code>Windows Computer</code> (or other) as the device<br>
    Click <strong>Generate</strong><br><br>
    Google will give you a 16-character password like:<br>
    <code>abcd efgh ijkl mnop</code>
  </li>
  <br>
  <li>
    <strong>Use the App Password in Your Script</strong><br>
    Update your script like this:<br><br>
    <pre><code>MY_EMAIL = "yourgmail@gmail.com"
MY_PASSWORD = "abcd efgh ijkl mnop"  # Your app password here</code></pre>
  </li>
</ol>
