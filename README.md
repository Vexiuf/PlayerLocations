# PlayerLocations Plugin Documentation

## Introduction

PlayerLocations is a Minecraft plugin designed to enhance the server experience by providing information about player locations based on their IP addresses. This documentation will guide you through the installation, configuration, and usage of the plugin.

## Installation

1. Download the latest version of the plugin from [SpigotMC]().
2. Place the plugin JAR file into the 'plugins' folder of your Bukkit or Spigot server.
3. Restart the server to load the plugin.

## Configuration

The plugin requires an API key from ipstack to fetch location information. Follow these steps to configure the plugin:

1. Sign up for a free ipstack account at [ipstack signup page](https://ipstack.com/signup).
2. Confirm your email by clicking on the confirmation link sent to you.
3. Log in to your ipstack account.
4. Copy your API key from the ipstack dashboard.
5. Open the `plugins/PlayerLocations/config.yml` file.
6. Add your API key to the configuration file:

```yaml
# Configuration for PlayerLocations
key: "YOUR_IPSTACK_API_KEY"
```

Replace `YOUR_IPSTACK_API_KEY` with the API key you obtained from ipstack.

## Features

- Display player join events in the server console, including player name and their country based on IP address.

## Commands

- **/playerlocations** Shows information about plugin and restarts the plugin 
- **/location <username>** Shows the location of a user

## Permissions

- **playerlocations.command.playerlocations**
- **playerlocations.command.location**

## Events

- `PlayerJoinEvent`: Displays player join events in the server console, including player name and their country based on IP address.

## Troubleshooting

If you encounter any issues while using the plugin, consider the following:

1. Check the server console for error messages.
2. Verify that your ipstack API key is correctly configured in the `config.yml` file.
3. Ensure that the plugin is compatible with your server version.

## API Usage (if applicable)

PlayerLocations does not currently provide an external API for developers.

## Contributing

We welcome contributions! If you would like to contribute to the development of PlayerLocations, please follow our [Contribution Guidelines](link_to_contributing_docs).

## License

PlayerLocations is licensed under the **Creative Commons Attribution-NonCommercial-NoDerivs 3.0 Unported License**.

### You are free to:

- **Share** — Copy and redistribute the material in any medium or format.
- **Adapt** — Remix, transform, and build upon the material.

Under the following terms:

- **Attribution** — You must give appropriate credit, provide a link to the license, and indicate if changes were made. You may do so in any reasonable manner, but not in any way that suggests the licensor endorses you or your use.
- **NonCommercial** — You may not use the material for commercial purposes.
- **NoDerivatives** — If you remix, transform, or build upon the material, you may not distribute the modified material.
