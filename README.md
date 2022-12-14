# ATIS_GENERATOR

<!-- PROJECT SHIELDS -->
<!--
*** I'm using markdown "reference style" links for readability.
*** Reference links are enclosed in brackets [ ] instead of parentheses ( ).
*** See the bottom of this document for the declaration of the reference variables
*** for contributors-url, forks-url, etc. This is an optional, concise syntax you may use.
*** https://www.markdownguide.org/basic-syntax/#reference-style-links
-->
[![Contributors][contributors-shield]][contributors-url]
[![Issues][issues-shield]][issues-url]
[![Forks][forks-shield]][forks-url]
## Rudimentary instructions to get started:
1. Download Code
2. Import redbbqhz_atis_generator.sql using your preferred method into MySQL. This file includes ICAO codes and associated airport names.
3. Open /includes/constants.php in a text editor and change the MySQL database connection information to your database
4. Upload files to your server.
5. Profit.

## Advanced Instructions:
1. Download Code
2. MariaDB
	1. Create database
		1. name: redbeard-atis-generator
	2. Create atis-generator user
		1. username: redbeard_atis_generator(or whatever works for you)
		2. password: (create secure password or have mariaDB generate it for you)
		3. permissions: only enable SELECT for the database: redbeard-atis-generator
	3. Import redbbqhz_atis_generator.sql using your preferred method into MySQL. This file includes ICAO codes and associated airport names.
3. Open /includes/constants.php in a text editor and change the database connection information to your database and user info

## Requirements:
1. PHP: version 8.1 or greater
2. MYSQL: My current server setup is running 10.3.36-MariaDB-log-cll-lve
3. cURL: is used to fetch weather info, so this function must be enabled.

## Basic rules:
1. Credit me for any use.
2. Do NOT, and I mean DO NOT charge for this, or put it behind a paywall.

<!-- CONTRIBUTING -->
## Contributing

Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
Don't forget to give the project a star! Thanks again!

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## Contributors
<a href = "https://github.com/RedbeardTFL/ATIS_GENERATOR/graphs/contributors">
<img src = "https://contrib.rocks/image?repo=RedbeardTFL/ATIS_GENERATOR"/>
</a>

<!-- MARKDOWN LINKS & IMAGES -->
<!-- https://www.markdownguide.org/basic-syntax/#reference-style-links -->
[contributors-shield]: https://img.shields.io/github/contributors/RedbeardTFL/ATIS_GENERATOR.svg?style=for-the-badge
[contributors-url]: https://github.com/RedbeardTFL/ATIS_GENERATOR/graphs/contributors

[forks-shield]: https://img.shields.io/github/forks/RedbeardTFL/ATIS_GENERATOR.svg?style=for-the-badge
[forks-url]: https://github.com/RedbeardTFL/ATIS_GENERATOR/network

[issues-shield]: https://img.shields.io/github/issues/RedbeardTFL/ATIS_GENERATOR.svg?style=for-the-badge
[issues-url]: https://github.com/RedbeardTFL/ATIS_GENERATOR/issues