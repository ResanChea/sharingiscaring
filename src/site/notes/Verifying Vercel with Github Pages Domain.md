---
{"dg-publish":true,"permalink":"/verifying-vercel-with-github-pages-domain/"}
---

## If you create an app through Vercel and don't know how to add your github pages domain to the vercel app heres how
1. Go to https://github.com/settings/pages and add a custom domain
2. Paste in the link to your vercel app, for me it will be https://sharingiscaring-jade.vercel.app
3. Next github will ask you to verify the domain with vercel as below
![Screenshot_20260104_165339_Chrome.jpg](/img/user/Attachments/Screenshot_20260104_165339_Chrome.jpg)
	*1. Create a TXT record in your DNS configuration for the following hostname: github-pages-challenge-ResanChea.sharingiscaring-jade.vercel.app*
	*2. Use this code for the value of the TXT record:* 
		**Random code and characters for verification**
	*3. Wait until your DNS configuration changes. This could take up to 24 hours to propagate.*
4. From here, go to your vercel page, click your project you want to connect and open the 'Domain' tab and click 'Add Existing'
	![Screenshot_20260104_164411_Chrome.jpg](/img/user/Attachments/Screenshot_20260104_164411_Chrome.jpg)
	![Screenshot_20260104_164340_Chrome.jpg](/img/user/Attachments/Screenshot_20260104_164340_Chrome.jpg)
5. Select the repository you are publishing the app from 
6. From here put in your github pages link, it should be 'your-github-username.github.io'
7. After you must create a namerecord with the 
	1. Name: 1st copy from Github
	2. Type being 'TXT'
	3. Value: 2nd copy from Github
		![Screenshot_20260104_164910_Chrome.jpg](/img/user/Attachments/Screenshot_20260104_164910_Chrome.jpg)
8. Now do as the instruction says and wait 24 hours before pressing verify on github pages again.