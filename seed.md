![](assets/banner.png)



<img src="assets/htb.png" style="margin-left: 20px; zoom: 60%;" align=left />    	<font size="10">Machine Name</font>

​		DD<sup>th</sup> Month YYYY

​		Machine Author(s): `RaidenZX`

​		

 



### Description:

This machine...  I am bringing for many people to learn beyond web exploration
happy hacking!!!

### Difficulty:

`easy`

### Flags:

User: `saket:e51762be19cf67d78cf7806a6ad3a123`

Root: `root:5375627363726962654f6e4d79436861`

# Enumeration

in the enumeration phase we can use nmap even to see which ports are initially open


<img src="assets/images/nmapscan.png" style="margin-left: 20px; zoom: 60%;" align=left />    	<font size="10">Machine Name</font>

looking for the source view i didn't find anything so giving a gobuster i noticed an open js/ so i came across the CMS version...

<img src="assets/images/jsonfile.png" style="margin-left: 20px; zoom: 60%;" align=left />    	<font size="10">Machine Name</font>

but of course I also looked a little bit about the source-forge version and i found this...

<img src="assets/images/settings.png" style="margin-left: 20px; zoom: 60%;" align=left />    	<font size="10">Machine Name</font>

and stay here...

<img src="assets/images/settings_xml.png" style="margin-left: 20px; zoom: 60%;" align=left />    	<font size="10">Machine Name</font>

# Foothold
I logged in with the credentials in mysql and...

<img src="assets/images/mysql.png" style="margin-left: 20px; zoom: 60%;" align=left />    	<font size="10">Machine Name</font>

and I found a CVE for this CMS.


<img src="assets/images/CVE.png" style="margin-left: 20px; zoom: 60%;" align=left />    	<font size="10">CVE</font>


# Lateral Movement



# Privilege Escalation

