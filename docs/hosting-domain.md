# Starting making a domain using .anet TLD.
# Notice, everything starts from cloning the repo.

1. Gather basic server info: For verification we'll need your username, domain's description (optional) and host's ip address (with port if needed, 443 will be set otherwise.)

Example domain: test.json will result in a test.anet domain, you can use file !!!domain_template.json as your record base.

2. Open a pull request to this repo, and wait for approval.

In the meantime, you can setup webserver nginx, apache or pretty much anything. ***if its a file sharing, for example. I do not guarantee the security of it's files, meaning, everything depends on You.***

3. After approval restart your local DNS resolver & wait for it to fetch the updated DNS and after its completed you can now visit your domain, if ANet's DNS resolver is setted up correctly.

# Tips
1. Make local DNS file changes to immediately test the results, you can also make hidden domain names like this, just please make sure it doesnt interfere with global DNS file.
