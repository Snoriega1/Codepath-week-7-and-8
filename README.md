# Codepath-week-7-and-8
Homework assignment for WordPress Pen testing assignment
<hr>
WordPress Exploits
<hr>
everything <br>
12233
<img src="https://i.ibb.co/DCWbcWc/WPDistillery-wont-work.png" alt="WPDistillery-wont-work" border="0">
<img src="https://i.ibb.co/FJjFDTk/Word-Press-V4-2.png" alt="Word-Press-V4-2" border="0">
<img src="https://i.ibb.co/B4TnbfB/Not-showing-all-vulnerabilities.png" alt="Not-showing-all-vulnerabilities" border="0">
<img src="https://i.ibb.co/2df3Ddq/Still-not-working-no-alert.png" alt="Still-not-working-no-alert" border="0">
<img src="https://i.ibb.co/CsD2DR4/Change-the-title.png" alt="Change-the-title" border="0">



<hr>

<b><h3>EXPLOIT # 1:</h3></b> NAME OF EXPLOIT
https://nvd.nist.gov/vuln/detail/CVE-2016-7168

<b>REFERENCE:</b> https://sumofpwn.nl/advisory/2016/persistent_cross_site_scripting_vulnerability_in_wordpress_due_to_unsafe_processing_of_file_names.html

<b>THE VULNERABILITY:</b>
DESCRIBE VULNERABILITY HERE

<b>STEPS TO RECREATE:</b>
1.  Confirm that the WordPress target is vulnerable. To find the WordPress version, go to http://wpdistillery.vm/wp-admin/about.php. The WordPress version should be version 4.6 or older.<br>
   
2.  Save an image with a crafted name that includes malicious JavaScript code to be executed. In my example, I saved an image with the following name in order to execute a simple JavaScript prompt:<br>
   
3.  As an administrator, select Media from the Admin Dashboard page menu on the left. Click "Add New" near the top. Select the image with the crafted file name and upload.<br>

4.  From the same Media Library page, select the image just uploaded. NOTE: You may have to refresh the page to see the recently uploaded image.<br>

5.  Within 'Attachment Details' click "View attachment page" near the bottom right to view the page containing the uploaded image:<br>
   
6.  Here you will see the executed JavaScript code within the filename which will contine to be run whenever the image is loaded, demonstrating the possibility for persistent Cross-Site Scripting:<br>
<img src="https://i.ibb.co/BsDRyWD/Exploit-1.png" alt="Exploit-1" border="0">
<hr>
