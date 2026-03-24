# Your organization requires a customized Linux distribution without age attestation for internal use, and you've been tasked with creating it.

_Create a custom Linux distribution based on Pop_os without age attestation._

## Steps

1. Download the latest Pop_os ISO from the official System76 website using `wget` (e.g., `wget https://cdn.pop-os.org/current.iso`)
2. Create a new directory for your custom distribution and change into it (`mkdir mydistro`, `cd mydistro`)
3. Use `sudo` and `apt` to install necessary build tools (`sudo apt install -y build-essential`)
4. Modify the Pop_os configuration to disable age attestation as described in previous steps
5. Use tools like `mkisofs` to create a custom ISO image of your modified distribution (`mkisofs -o mydistro.iso mydistro/`)

## Pitfalls

- Inadvertently including proprietary software in your custom distribution, which could lead to legal issues