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
