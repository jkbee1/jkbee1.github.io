Introduction MD
Complete installation guide: https://doc.owncloud.org/server/latest/admin_manual/installation/
First, check the Release Notes: https://doc.owncloud.org/server/latest/admin_manual/release_notes.html
Install and configure Owncloud server: https://doc.owncloud.org/server/latest/admin_manual/installation/
System Requirements: https://doc.owncloud.org/server/latest/admin_manual/installation/system_requirements.html
Consider the deployment recommendations: https://doc.owncloud.org/server/latest/admin_manual/installation/deployment_recommendations.html
Download: https://owncloud.org/download/#owncloud-server-tar-ball
 and install: https://doc.owncloud.org/server/latest/admin_manual/installation/linux_installation.html
Linux Package Manager Installation¶
Package managers should only be used for single-server setups. For production environments, we recommend installing from the tar archive.
Available Packages
The recommended package to use is owncloud-files. It only installs ownCloud, and does not install Apache, a database, or any of the required PHP dependencies.
Installing ownCloud Community Edition
First, install your own LAMP stack, as doing so allows you to create your own custom LAMP stack without dependency conflicts with the ownCloud package. Then, update package manager’s configuration.
Configurations are available for the following Linux distributions:
•	Ubuntu 14.04 & 16.04
•	Debian 7 & 8
•	RHEL 6 & 7
•	CentOS 7.2 & 7.3
•	SLES 11SP4 & 12SP2
•	openSUSE Leap 42.2 & 42.3
Repositories for Fedora, openSUSE Tumbleweed, and Ubuntu 15.04 have been dropped. If you use Fedora, use the tar archive with your own LAMP stack. openSUSE users can rely on LEAP packages for Tumbleweed.
Once your package manager has been updated, follow the rest of the instructions on the download page to install ownCloud. Once ownCloud’s installed, run the Installation Wizard to complete your installation.
See the System Requirements for the recommended ownCloud setup and supported platforms.
Note: Do not move the folders provided by these packages after the installation, as this will break updates.
What is the Correct Version?
Package versions are composed of a major, a minor, and a patch number, such as 9.0, 9.1, 10.0, 10.0.1, and 10.0.2. The second number represents a major release, and the third number represents a minor release. See https://doc.owncloud.org/server/latest/admin_manual/installation/linux_installation.html for further Release version information.
Installing ownCloud Enterprise Edition
See Installing & Upgrading ownCloud Enterprise Edition for instructions on installing ownCloud Enterprise edition.
Installation Wizard
When the ownCloud prerequisites are fulfilled and all ownCloud files are installed, the last step to completing the installation is running the Installation Wizard. This involves just three steps:
1.	Point your web browser to http://localhost/owncloud
2.	Enter your desired administrator’s username and password.
3.	Click “Finish Setup”.
 
You’re now finished and can start using your new ownCloud server. Of course, there is much more that you can do to set up your ownCloud server for best performance and security. For important installation and post-installation steps, see . 
https://doc.owncloud.org/server/latest/admin_manual/installation/configuration_notes_and_tips.html 


As an administrator, how do I enable users to connect to the Owncloud server using the server's IP address and port 8080? Maybe: https://doc.owncloud.org/server/latest/admin_manual/configuration/server/config_sample_php_parameters.html
Add user account: https://doc.owncloud.org/server/10.0/admin_manual/configuration/user/user_configuration.html
Creating a New User¶
As an Administrator, add new user
On the User management page of your ownCloud Web UI you can:
•	Create new users
•	The default view displays basic information about your users.
•	 

To create a user account:
•	Enter the new user’s Login Name and their initial Password
•	Optionally, assign Groups memberships
•	Click the Create button
 
Login names may contain letters (a-z, A-Z), numbers (0-9), dashes (-), underscores (_), periods (.) and at signs (@). After creating the user, you may fill in their Full Name if it is different than the login name, or leave it for the user to complete.
If you have checked Send email to new user in the control panel on the lower left sidebar, you may also enter the new user’s email address, and ownCloud will automatically send them a notification with their new login information. You may edit this email using the email template editor on your Admin page (see Email Configuration).

As a user, how do I connect to the Owncloud server using a desktop or mobile client? 
https://doc.owncloud.org/server/10.0/user_manual/files/desktop_mobile_sync.html

Desktop: https://doc.owncloud.org/desktop/latest/
Installing the Desktop Synchronization Client¶
First, you must install:
You can download the latest version of the ownCloud Desktop Synchronization Client from the ownCloud download page. There are clients for Linux, macOS, and Microsoft Windows.
Installation on Mac OS X and Windows is the same as for any software application: download the program and then double-click it to launch the installation, and then follow the installation wizard. After it is installed and configured the sync client will automatically keep itself updated; see The Automatic Updater for more information.
Installation Wizard
The installation wizard takes you step-by-step through configuration options and account setup. First you need to enter the URL of your ownCloud server.
 
Enter your ownCloud login on the next screen.
 
On the “Local Folder Option” screen you may sync all of your files on the ownCloud server, or select individual folders. The default local sync folder is ownCloud, in your home directory. You may change this as well.
 
When you have completed selecting your sync folders, click the “Connect” button at the bottom right. The client will attempt to connect to your ownCloud server, and when it is successful you’ll see two buttons:
•	one to connect to your ownCloud Web GUI
•	one to open your local folder
It will also start synchronizing your files.
Mobile device connections:
iOS: https://doc.owncloud.org/ios/ios_app.html

Using the ownCloud iOS App 3.6.2¶
Accessing your files on your ownCloud server via the Web interface is easy and convenient, as you can use any Web browser on any operating system without installing special client software. However, the ownCloud iOS app offers some advantages over the Web interface:
•	A simplified interface that fits nicely on an iPhone or iPad
•	Automatic synchronization of your files
•	Share files with other ownCloud users
•	Easily upload files from your device to ownCloud
•	Optional PIN for stronger security
Getting the ownCloud iOS App
Open Safari, or any Web browser, and point it to your ownCloud server. Log in and look on your Personal page for a link to the ownCloud app on iTunes. When you install the ownCloud app and open it you’ll be prompted for your ownCloud server URL and login. When it connects it opens to your Files page.
 
You’ll also find links and information at the ownCloud installation page.
Managing Your Files¶
All your files on your ownCloud server are listed on the Files page, but are not downloaded to your iPhone or iPad until you tap on them. Downloaded files are marked with a little green arrow. Thumbnails are displayed for both downloaded and not-downloaded files (owncloud 8.0+ only). Click the overflow button at the top right (the three-dot button) to upload files to your server, create a new folder, or sort your files alphabetically or by date.
The Files button at the bottom takes you back to your main Files page. The Uploads button shows your history of uploads to your ownCloud server. The Shared Links button shows how many files you have shared by link.
When you’re in the Files view, slide any filename to the right to expose your file management options. These are: Trash, Share, and More. The More button has options for Open With, Rename, Move, Available Offline.
 
The More button has different options for folders. These are: Rename, Move, Download Folder, and Available Offline.

Android: https://doc.owncloud.org/android/android_app.html
Using the ownCloud Android App¶
Accessing your files on your ownCloud server via the Web interface is easy and convenient, as you can use any Web browser on any operating system without installing special client software. However, the ownCloud Android app offers some advantages over the Web interface:
•	A simplified interface that fits nicely on a tablet or smartphone
•	Automatic synchronization of your files
•	Share files with other ownCloud users and groups, and create multiple public share links
•	Upload of photos and videos recorded on your Android device
•	Easily add files from your device to ownCloud
•	Two-factor authentication
Installing
One way to get your ownCloud Android app is to log into your ownCloud server from your Android device using a Web browser such as Chrome, Firefox, or Dolphin.
The first time you log into a new ownCloud account, you’ll see a screen with a download link to the ownCloud app in the Google Play Store.
 
You will also find these links on your Personal page in the ownCloud Web interface. Find source code and more information from the ownCloud download page. Users of customized ownCloud Android apps, for example from their employer, should follow their employer’s instructions.
Connecting to Your ownCloud Server¶
The first time you run your ownCloud Android app, it opens to a configuration screen. Enter your server URL, login name, password, and click the Connect button. Click the eyeball to the right of your password to expose your password.
 
For best security, your ownCloud server should be SSL-enabled so that you can connect via HTTPS. The ownCloud app will test your connection as soon as you provide it and tell you if you entered it correctly. If your server has a self-signed SSL certificate, you’ll get a warning that it is not to be trusted. If this happens, click the “YES” button to accept the certificate and complete your account setup.
 
With that completed, you’re now ready to use the Android application. At this point, you’ll be on the “All Files” screen, which you see below.
 
By clicking the main menu at the top left, you will be able to manage the core functionality of the app. The options are:
•	Manage Users Accounts
•	Current Uploads
•	All Files
•	Application Settings
For more user, config, and deployment guides, see: https://doc.owncloud.org/#
And : https://owncloud.org/help/


