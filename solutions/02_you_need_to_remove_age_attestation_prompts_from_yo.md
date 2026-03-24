# You need to remove age attestation prompts from your Pop_os installation to comply with specific project requirements.

_Modify your Pop_os system to bypass age attestation prompts._

## Steps

1. Open a terminal and run `sudo nano /etc/Pop_os.conf` to edit the Pop_os configuration file.
2. Add the line `age_attestation=false` to the end of the file and save changes.
3. Execute `sudo systemctl restart pop-os-services` to apply the changes.
4. Verify the absence of age attestation prompts by running `sudo pop-os --version` and checking for any warnings or prompts.
5. Document your changes for future reference and potential reversals using `git` (e.g., `git add .`, `git commit -m 'Disabled age attestation'`)

## Pitfalls

- Incorrectly editing system files, which can lead to system instability