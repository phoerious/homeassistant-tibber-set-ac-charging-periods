# Set AC Charging Price Limits

HomeAssistant blueprint for setting an electricty price window for AC charging your PV battery from the grid.

The blueprint uses the Tibber price information obtained via the [Tibber Price Information & Ratings integration](https://github.com/jpawlowski/hass.tibber_prices) to set two input number helpers, which can then be used in automations (e.g. the [Solakon Zero-Export Blueprint](https://github.com/D4nte85/Solakon-One-Nulleinspeisung-Blueprint-homeassistant)).

## Installation

This blueprint relies on the "Tibber Price Information & Ratings" integration, which can be installed via HACS.

### Step 1:

Install [HACS](https://hacs.xyz/):

### Step 2:

Install the Tibber price integration:

[![Open your Home Assistant instance and open a repository inside the Home Assistant Community Store.](https://my.home-assistant.io/badges/hacs_repository.svg)](https://my.home-assistant.io/redirect/hacs_repository/?owner=jpawlowski&repository=hass.tibber_prices&category=integration)

### Step 3:

Set up and configure the integration (you may want to adjust the limits for best and peak price periods).

[![Open your Home Assistant instance and start setting up a new integration.](https://my.home-assistant.io/badges/config_flow_start.svg)](https://my.home-assistant.io/redirect/config_flow_start/?domain=tibber_prices)

### Step 4:

Import the blueprint.

[![Open your Home Assistant instance and show the blueprint import dialog with a specific blueprint pre-filled.](https://my.home-assistant.io/badges/blueprint_import.svg)](https://my.home-assistant.io/redirect/blueprint_import/?blueprint_url=https%3A%2F%2Fgithub.com%2Fphoerious%2Fhomeassistant-tibber-set-ac-charging-periods%2Fblob%2Fmain%2Fblueprint.yaml)

You have to create two numerical input numbers, which will contain the lower and upper price limits, as well as a boolean toggle. The toggle can be used to halt automatic price window updates if you want to manually override the prices.
