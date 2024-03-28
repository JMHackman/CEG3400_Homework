* What CWE you chose (name, CWE number, link to web, and an explanation in your own words).  
	- Name: Use of Hard-coded Credentials

	- CWE number: CWE-798  

	- Link: https://cwe.mitre.org/data/definitions/798.html

	- Explanation: A password, passkey, passphrase, confidential login code numbers, etc. One of these credential type things, that are coded directly into the code.  

* Your Well Formed CPE name (fake but well formed!!!, unless you actually have a CPE for it), explain each field you chose to use, be sure to assign a version via Semantic Versioning 2.0.  
	- CPE name:  `cpe:2.3:a:hackman_company:pass_storage:1.0:1.4:GoldTier:en:windows_11:*`

	- Explanation: 
* `cpe:2.3` Is the CPE specification being used. 
* `a` Represents the CPE string that specifies the type of entity which is application.
* `hackman_company` Is the name of the vendor, which is me.
* `pass_storage` Is the product that is representing the Password Storage software.
* `1.0` Is the version number that was initially released.
* `1.4` Is the update version which indicates the subsequent version of the Password Storage software.
* `GoldTier` Would be the edition of the software.
* `en` Standard English language.
* `windows_11` Target software platform, indicates that the software was made for windows 11.
* `*` Shows that there is another field that could be filled in but was not, indicates no additional information was provided.

	- Version: 1.4 would be the current update and 1.0 being the initial release.

* Is it in the top 10 KEV list as well? What are your thoughts on the severity of the weakness.  
	- Top 10: CWE-798 is not in the top 10.

	- Severity: Its severity is quite high but, it is not common as only amateurs would hardcode a password, or allow a password to be implanted and stored with the same credentials everytime.

* What your personal experience is with the CWE.  
	- Experience: I made a thing that would have an actual password stored in the code itself that would allow access. To me it made thet piece of code easier to work with as I did not have to type in a password. If someone wanted to however, they could check the hard code and see that the password was already in place, therefore violating and being a CWE-798. 

* How you could have fixed it (what would you need to have done to not implement this weakness in your code). 
	- The most simple solution, and only solution should be to remove the password. The password should have never been stored and should never be saved into the code itself as it is a hazard to any and all who use that command or code. There should be no work arounds to incorporate passwords into code as they are meant to be secure and safe, and being paraded to all that look even a bit harder than any other is not a good method of safekeeping.

* List and link one actual CVE and related CPE that also fell prey to this weakness.  
	- Link: https://cybernews.com/news/attackers-exploit-atlassians-hard-coded-password-bug/

	- List: The company Atlassian, had issues with a hardcoded password. There was a critical vulnrability in its Confluence app. The vulnrability was labeled as a CVE-2022-26138, but can be boiled down to a CWE-798. The password vulnrability was leaked on twitter and spread quickly and allowed actors to gain full access over unpatched servers.
