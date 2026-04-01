Detailed Step-by-Step Guide: Launching and Stopping Your First AWS EC2 Instance

### Step 1: Access the AWS Management Console
- Navigate to **https://aws.amazon.com/free/**.
- Create a new account or sign in as the **root user**.
- You will land on the **Console Home** page (also called “Console Management”).

<img width="987" height="679" alt="image" src="https://github.com/user-attachments/assets/8d50e8eb-f352-4897-b00a-f838dbc0935d" />

**What the screenshot shows**: The main AWS dashboard with sections for “Recently visited” services on the left and “Applications” on the right. This is the starting point for all AWS services.

### Step 2: Open the Search Bar (Especially Important for New Users)
- On the Console Home page, click the **Search** field at the top (it may be empty if you’re a new user and have no “Recently visited” items).

<img width="987" height="679" alt="image" src="https://github.com/user-attachments/assets/64a1d530-284d-4ac0-bfcc-d59d0a12a701" />


**What the screenshot shows**: The top navigation bar with the search box highlighted in orange. The “Recently visited” panel is still blank on a fresh account.

### Step 3: Search for and Select EC2
- Type **EC2** in the search field.
- Click **EC2** from the results (it appears under “Services”).

<img width="987" height="679" alt="image" src="https://github.com/user-attachments/assets/59afa843-1eef-4a49-bb20-dcac2ee10d9f" />


**What the screenshot shows**: The search results dropdown with “EC2” highlighted. You can also see other services listed below.

### Step 4: Start the Launch Process
- On the EC2 dashboard, click the big orange button **Launch instance**.

<img width="987" height="679" alt="image" src="https://github.com/user-attachments/assets/eb30804d-f481-4090-beae-4cbd4232859f" />


**What the screenshot shows**: The EC2 console homepage with the “Launch instance” button circled in orange.

### Step 5: Name Your Instance
- In the “Name and tags” section, enter a friendly name.
- Example used in the guide: **“My first Instance”**.

<img width="987" height="679" alt="image" src="https://github.com/user-attachments/assets/aaec2b55-171f-4e13-80fd-ee04398295d5" />


**What the screenshot shows**: The launch wizard with the name field highlighted. A helpful blue “Take a walkthrough” banner may appear at the top.

### Step 6: Choose an Amazon Machine Image (AMI)
- Under “Application and OS Images”, select **Amazon Linux** (the recommended free-tier Linux option).

<img width="987" height="679" alt="image" src="https://github.com/user-attachments/assets/12b67bc8-d19d-4feb-8606-85ffd8e8504d" />


**What the screenshot shows**: The Quick Start tab with Amazon Linux highlighted. You can see other options like Ubuntu, Windows, etc., but Amazon Linux 2023 is selected.

### Step 7: Select the Instance Type
- Choose a **free-tier eligible** instance type (usually **t3.micro** or **t2.micro**).
- The guide confirms this is selected because the account is using the AWS Free Tier.

<img width="987" height="679" alt="image" src="https://github.com/user-attachments/assets/47bd735f-10a6-4a40-b42f-ef501d80dd8e" />


**What the screenshot shows**: The instance type table with “Free tier eligible” clearly marked in green and circled in orange.

### Step 8: Set Up a Key Pair (for Secure Login)
- In the **Key pair (login)** section, you can either:
  - Create a new key pair, **or**
  - Select an existing one from the dropdown.

<img width="987" height="679" alt="image" src="https://github.com/user-attachments/assets/881b6397-d57f-4fad-96bb-79b01871aeb4" />


**What the screenshot shows**: The key pair dropdown menu with the “Create new key pair” link highlighted.

### Step 9: Select an Existing Key Pair
- The guide uses a previously created key pair named **“Amazon Server”**.
- This .pem file is required later to connect to your instance via SSH.

<img width="987" height="679" alt="image" src="https://github.com/user-attachments/assets/4cf7c7a8-82db-491c-b1c5-04958eccc288" />


**What the screenshot shows**: The dropdown expanded with “Amazon Server” selected and highlighted.

### Step 10: Configure Network Settings (Security Group)
- Leave the default **“Create security group”** option selected.
- This automatically creates a new security group that allows SSH traffic from Anywhere (for initial access).

<img width="987" height="679" alt="image" src="https://github.com/user-attachments/assets/a5656983-c2af-4d4e-9f41-6d9d207a0641" />


**What the screenshot shows**: The “Network settings” panel with “Create security group” radio button selected and the SSH rule visible.

### Step 11: Configure Storage
- The default storage is **8 GiB** (gp3 volume).
- This is sufficient for a basic free-tier instance and requires no changes.

<img width="987" height="679" alt="image" src="https://github.com/user-attachments/assets/795c1467-e614-4049-a4a1-3a1b78269ffa" />


**What the screenshot shows**: The “Configure storage” section with 8 GiB selected and the volume type shown.

### Step 12: Launch the Instance
- Review the summary on the right side of the launch wizard.
- Click the orange **Launch instance** button at the bottom.

<img width="987" height="679" alt="image" src="https://github.com/user-attachments/assets/2149c21c-b2e4-4dc9-856c-e6ed8edbe8fd" />


**What the screenshot shows**: The final launch confirmation screen with the “Launch instance” button highlighted.

### Step 13: View Your Running Instance
- After launch, AWS shows a success message.
- Click the **Instance ID** (blue link) to go to the instance details page.

<img width="987" height="679" alt="image" src="https://github.com/user-attachments/assets/86cfe929-c2bf-4008-997b-c616a674ad62" />


**What the screenshot shows**: The Instances list with the new instance highlighted. The status shows “Running” and “Initializing”.

### Step 14: Return to the Instances List
- Click **Instances** in the left navigation (or breadcrumb) to return to the full list of your EC2 instances.

<img width="987" height="679" alt="image" src="https://github.com/user-attachments/assets/31be297e-fbe1-4ad6-8a2d-f6623db3cc04" />


**What the screenshot shows**: The top navigation with “Instances” tab highlighted, showing the full instance summary.

### Step 15: Open the Actions Menu
- Select your instance in the list.
- Click the **Actions** dropdown button at the top.

<img width="987" height="679" alt="image" src="https://github.com/user-attachments/assets/dfca4fe0-391d-49f7-be86-ec9579e9c954" />


**What the screenshot shows**: The Actions menu expanded with options like Instance settings, Security, Networking, etc.

### Step 16: Stop the Instance
- From the Actions menu, go to **Instance state** → **Stop instance**.
- (You could also choose Reboot or Terminate here if needed.)

<img width="987" height="679" alt="image" src="https://github.com/user-attachments/assets/c032f22d-565a-48cb-8cc1-48c2e485319f" />


**What the screenshot shows**: The Instance state dropdown with “Stop instance” highlighted.

### Step 17: Confirm the Stop Action
- A confirmation dialog appears.
- AWS shows a green message: **“Can stop”** (because stop protection was not enabled).
- Click the orange **Stop** button to confirm.

<img width="987" height="679" alt="image" src="https://github.com/user-attachments/assets/a9270959-62d6-4e08-aa63-008da29911ca" />


**What the screenshot shows**: The stop confirmation modal with the warning about billing for associated resources (Elastic IP, EBS volume) and the “Stop” button highlighted.

You have now successfully launched, viewed, and safely stopped your very first EC2 instance exactly as shown in the PDF screenshots! If you follow these steps in order, your console will look identical to the images in the document.
