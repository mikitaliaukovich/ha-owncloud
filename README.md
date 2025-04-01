![Supports aarch64 Architecture][aarch64-shield]
![Supports amd64 Architecture][amd64-shield]
![No support for armhf Architecture][armhf-shield]
![No support for armv7 Architecture][armv7-shield]
![No support for i386 Architecture][i386-shield]


<div align="center">
  <img src="https://upload.wikimedia.org/wikipedia/commons/f/f6/OwnCloud_logo_and_wordmark.svg" alt="ownCloud x Home Assistant" width="200"/>
  <img src="https://upload.wikimedia.org/wikipedia/en/thumb/4/49/Home_Assistant_logo_%282023%29.svg/1200px-Home_Assistant_logo_%282023%29.svg.png" alt="ownCloud x Home Assistant" width="80"/>

  <h3 align="center">ownCloud x Home Assistant</h3>
  Home Assistant ownCloud Add-on

  <p align="center">
    <a href="https://owncloud.com">ownCloud</a>
    &middot;
    <a href="https://www.home-assistant.io/docs/">Home Assistant</a>
  </p>
</div>

This repository contains an add-on for Home Assistant that allows you to run an ownCloud server in a Docker container. ownCloud is a powerful open-source file sync and share solution that enables you to store and manage your files securely.

## Project Structure

The project consists of the following files:

- **owncloud/Dockerfile**: Instructions to build the Docker image for the ownCloud application.
- **owncloud/config.json**: Configuration file for the Home Assistant add-on, defining metadata and options.
- **owncloud/run.sh**: Shell script executed when the add-on is started, containing commands to run the ownCloud server.
- **owncloud/README.md**: Documentation specific to the ownCloud add-on, including installation and usage guidelines.

## Installation

The installation of this add-on is the same way as any Hass.io add-on.

[![Add repository on my Home Assistant][repository-badge]][repository-url]

1. [Add this repository][repository] to your Home Assistant instance.
1. Install the add-on.
1. Click the `Save` button to store your configuration.
1. Start the add-on.
1. Carefully configure the add-on to your preferences, see the [official documentation](https://doc.owncloud.com/server/next/) for for that.

## Usage

Once the add-on is installed and running, you can access your ownCloud server through the web interface. Refer to the `owncloud/README.md` for detailed usage instructions and configuration options.


<!--

Notes to developers after forking or using the github template feature:
- While developing comment out the 'image' key from 'example/config.yaml' to make the supervisor build the addon
  - Remember to put this back when pushing up your changes.
- When you merge to the 'main' branch of your repository a new build will be triggered.
  - Make sure you adjust the 'version' key in 'example/config.yaml' when you do that.
  - Make sure you update 'example/CHANGELOG.md' when you do that.
  - The first time this runs you might need to adjust the image configuration on github container registry to make it public
  - You may also need to adjust the github Actions configuration (Settings > Actions > General > Workflow > Read & Write)
- Adjust the 'image' key in 'example/config.yaml' so it points to your username instead of 'home-assistant'.
  - This is where the build images will be published to.
- Rename the example directory.
  - The 'slug' key in 'example/config.yaml' should match the directory name.
- Adjust all keys/url's that points to 'home-assistant' to now point to your user/fork.
- Share your repository on the forums https://community.home-assistant.io/c/projects/9
- Do awesome stuff!
 -->

[aarch64-shield]: https://img.shields.io/badge/aarch64-yes-green.svg
[amd64-shield]: https://img.shields.io/badge/amd64-yes-green.svg
[armhf-shield]: https://img.shields.io/badge/armhf-no-red.svg
[armv7-shield]: https://img.shields.io/badge/armv7-no-red.svg
[i386-shield]: https://img.shields.io/badge/i386-no-red.svg


[repository]: https://github.com/alexbelgium/hassio-addons
[repository-badge]: https://img.shields.io/badge/Add%20repository%20to%20my-Home%20Assistant-41BDF5?logo=home-assistant&style=for-the-badge
[repository-url]: https://my.home-assistant.io/redirect/supervisor_add_addon_repository/?repository_url=https%3A%2F%2Fgithub.com%2Fmikitaliaukovich%2Fha-owncloud
[repo-url]: https://github.com/mikitaliaukovich/ha-owncloud
