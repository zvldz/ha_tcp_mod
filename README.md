# Modified [tcp](https://www.home-assistant.io/integrations/tcp/) component for Home Assistant

## Installation
*__Manual mode__*

Place the `tcp_mod` folder into your `custom_components` folder.

*__Adding custom repository to [HACS](https://hacs.xyz/)__*

Go to the Integrations page in HACS and select the three dots in the top right corner. Select Custom repositories.
Add repository url. Category - Integration. Read more on https://hacs.xyz/docs/faq/custom_repositories.

## Changes compared to the original component

* Added `payload_template`.
* Added `data` attribute containing the full response.
* Added configuration variable `send_eol`. Boolean variable for forced sending newline character. Default value: false.

## Example
```yaml
# Example configuration.yaml entry
sensor:
  - platform: tcp_mod
    host: IP_ADDRESS
    port: PORT
    payload: PAYLOAD
```
