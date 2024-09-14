# Installing a Self-Signed Certificate to Avoid Browser Warnings (for asper, ann and some other, official domains)

To avoid browser warnings when using a self-signed certificate, you need to install the self-signed certificate in the trusted root certificate store of your operating system or browser. Follow the instructions below for your specific platform.

## For Windows

1. **Open the Certificate Manager**:
   - Press `Win + R`, type `mmc`, and press Enter.
   - In the MMC console, go to `File` > `Add/Remove Snap-in`.
   - Select `Certificates` and click `Add`.
   - Choose `Computer account` and click `Next`, then `Finish`.

2. **Import the Certificate**:
   - In the left pane, expand `Certificates (Local Computer)`.
   - Right-click on `Trusted Root Certification Authorities`, then select `All Tasks` > `Import`.
   - Follow the wizard to import your self-signed certificate (`selfsigned.crt`).

3. **Complete the Import**:
   - Browse to the location of your self-signed certificate, select it, and complete the import process.

4. **Restart Your Browser**:
   - Close and reopen your browser to ensure it recognizes the new trusted certificate.

## For macOS

1. **Open Keychain Access**:
   - Open `Keychain Access` from `Applications` > `Utilities`.

2. **Import the Certificate**:
   - Drag and drop your self-signed certificate (`selfsigned.crt`) into the `System` keychain or use `File` > `Import Items`.

3. **Trust the Certificate**:
   - Find your certificate in the list, double-click it, and expand the `Trust` section.
   - Set `When using this certificate` to `Always Trust`.

4. **Close Keychain Access**:
   - Close the Keychain Access application. You may need to enter your password to confirm the changes.

5. **Restart Your Browser**:
   - Close and reopen your browser to ensure it recognizes the new trusted certificate.

## For Linux

1. **Copy the Certificate**:
   - Copy your self-signed certificate to the appropriate directory. For example:

   ```bash
   sudo cp path/to/self-signed.crt /usr/local/share/ca-certificates/

2. **Restart Your Browser**:
   - Close and reopen your browser to ensure it recognizes the new trusted certificate.
