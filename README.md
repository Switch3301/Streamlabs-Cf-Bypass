# Streamlabs Promo Cloudflare Bypass

## Overview
This simple trick allows bypassing Cloudflare protection on the Streamlabs Discord Nitro promo page by appending a random query parameter to the URL.

## How It Works
Instead of sending requests to:
```
https://streamlabs.com/discord/nitro
```
Appending a random query parameter like `?s` or `?s=` prevents Cloudflare from interfering:
```
https://streamlabs.com/discord/nitro?s
https://streamlabs.com/discord/nitro?s=
```

## Usage
1. Open your browser or a script.
2. Use any of the modified URLs above.
3. Cloudflare protection will not trigger.

## Example (Python Script)
```python
import requests

url = "https://streamlabs.com/discord/nitro?s"
response = requests.get(url)
print(response.text)
```

## Notes
- The exact behavior may change if Streamlabs updates their security.
- This method does not exploit or modify any system, it simply bypasses an unnecessary security check.

## Disclaimer
This repository is for educational purposes only. Use responsibly.

## Credits
notlit : `notlit_3` ( Discord )
Join here for more : https://discord.gg/notlituwu
