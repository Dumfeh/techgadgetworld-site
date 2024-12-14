# techgadgetworld-site
Creating an e-commerce shop to sell electrical gadgets
This is a modern, responsive, static e-commerce website for an electronics store. The website features product listings with images, descriptions, prices, and "Buy Now" buttons. The design is clean, responsive, and follows modern design principles using HTML, CSS, and Bootstrap 5.

Features
Responsive Design: The website is optimized for desktop, tablet, and mobile devices.
Product Listings: Products are listed with images, names, and prices.
Hover Effects: Product cards have smooth hover effects for a dynamic feel.
Modern User Interface: Clean and minimalist UI with intuitive navigation.
No Backend: The site is static and requires no server-side logic.
Technologies Used
HTML5 for the structure of the website.
CSS3 for styling and responsive design.
Bootstrap 5 for a responsive grid layout.
Google Fonts for modern typography.


Project Structure

e-commerce-electronics-shop/
│
├── index.html          # Main HTML file for the website
├── styles.css          # Custom CSS for styling
└── README.md           # Project description

How to Run Locally
Clone the repository:

If you haven’t already cloned this repository to your local machine, you can do it using the following Git command:
git clone https://github.com/your-username/e-commerce-electronics-shop.git

Navigate to the project folder:

Change to the project directory:
cd e-commerce-electronics-shop
Open index.html in your browser:

You can open the index.html file directly in your browser to view the website.


open index.html   # For macOS
start index.html  # For Windows
xdg-open index.html # For Linux

Optional: Use a local server (e.g., Live Server in VSCode) for a more accurate testing environment.

How to Deploy with AWS CloudFront
Step 1: Set Up an S3 Bucket

Log in to your AWS Management Console.
Go to S3 and create a new S3 bucket:
Choose a globally unique name for the bucket (e.g., techgadgetworld-site).
Leave the other options as default (we'll enable static website hosting next).

Step 2: Upload Files to S3 Bucket

Inside your S3 bucket, click on Upload and select all your files (index.html, styles.css, etc.).
After uploading, ensure that the files are publicly accessible:
Go to the Permissions tab of the S3 bucket.
Enable public access (or configure permissions as per your needs).

Step 3: Enable Static Website Hosting

In your S3 bucket settings, go to the Properties tab.
Under the Static website hosting section, enable it and set index.html as the Index document.
You’ll receive an S3 website endpoint URL (something like http://techgadgetsworld-site.s3-website-us-east-1.amazonaws.com).

Step 4: Set Up CloudFront

Go to the CloudFront service in the AWS Management Console.
Create a new CloudFront distribution:
For Origin Domain Name, select your S3 bucket's website endpoint.
Set Viewer Protocol Policy to Redirect HTTP to HTTPS for better security.
Leave the rest of the settings as default and click Create Distribution.
After the distribution is created, you’ll get a CloudFront URL (e.g., d1234567890abc.cloudfront.net).
You can now access your static website via the CloudFront URL.

Pushing the Website to GitHub
Follow these steps to push the project to GitHub for version control and sharing:

Initialize Git in Your Local Project Folder:

If you haven't already initialized a Git repository, open your terminal in the project folder and run:

git init
Add All Files to Git:

Add the files in the folder to your Git repository:
git add .

Commit the Changes:
Commit the added files with a meaningful commit message:
git commit -m "Initial commit of the e-commerce electronics shop"

Create a Repository on GitHub:

Go to GitHub and create a new repository (e.g., techgadgetsworld-shop).
Don't initialize the repository with a README if you're pushing an existing project.
Push Your Local Repository to GitHub:

Copy the repository URL from GitHub (e.g., https://github.com/your-username/techgadgets-shop.git) and push your local repository to GitHub:

git remote add origin https://github.com/your-username/e-commerce-electronics-shop.git
git branch -M main
git push -u origin main
Verify the Push:

Go to your GitHub repository page and check that your project files are there.
