# Creating a Domain with the .anet TLD

**Note:** Everything starts with cloning the repository.

## Steps to Create Your Domain

1. **Gather Basic Server Information**: For verification, we will need the following details:
   - Domain address.
   - The host's IP address.

   **Example**: Open `records.json`, add a new element (enclosed with `{}`), inside it add field "thn", this is your domain, then add field "hn", this is your server's IP. by default anet uses port 80, or 443 depending on the protocol and so it's solely your choice to make it http:// or https://

2. **Open a Pull Request**: Submit a pull request to this repository and wait for approval.

   In the meantime, you can set up your web server (e.g., Nginx, Apache, or any other server). ***If you are setting up a file-sharing service, please note that We, Asper do not guarantee the security of its files; the responsibility for security lies with you.***

3. **Restart Your Local DNS Resolver**: After your pull request is approved, restart your local DNS resolver and wait for it to fetch the updated DNS records. Once this is complete, you should be able to visit your domain, provided that ANet's DNS resolver is set up correctly.

## Tips

1. **Make Local DNS File Changes**: You can make changes to your local DNS file to immediately test the results. This allows you to create hidden domain names as well. Just ensure that these changes do not interfere with the global DNS file.
