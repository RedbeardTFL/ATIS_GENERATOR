# ATIS GENERATOR

[![License: CC BY-NC-SA 4.0][license-shield]][license-url]
[![Contributors][contributors-shield]][contributors-url]
[![Issues][issues-shield]][issues-url]
[![Forks][forks-shield]][forks-url]
[![Build Status][ci-shield]][ci-url]
[![Laravel Forge Site Deployment Status][forge-shield]][forge-url]

## Getting Started

1. Clone the repo

    ```sh
    git clone https://github.com/RedbeardTFL/ATIS_GENERATOR.git && cd ATIS_GENERATOR/src
    ```

2. Install Composer dependencies

    ```sh
    composer install
    ```

3. Fill in the .env file with your database credentials

    ```sh
    cp .env.example .env
    ```

4. Run artisan commands to generate a key and migrate the database

    ```sh
    php artisan key:generate & php artisan migrate --seed
    ```

5. Run git command to generate a version file for the footer

    ```sh
    git describe --always --tags --dirty > version
    ```

6. Run the development server

    ```sh
    php artisan serve
    ```

### Docker

1. Pull the image

    ```sh
    docker pull insidiousfiddler/redbeards-atis-generator
    ```

2. Run the container with your database credentials

    ```sh
    docker run -d -p 8000:80 insidiousfiddler/redbeards-atis-generator -e DB_HOST=<host> -e DB_PORT=<port> -e DB_DATABASE=<database> -e DB_USERNAME=<username> -e DB_PASSWORD=<password>
    ```

3. Visit the site at [http://127.0.0.1:8000](http://127.0.0.1:8000)

## Requirements

1. PHP: version 8.1 or greater
2. MYSQL: My current server setup is running 10.3.36-MariaDB-log-cll-lve
3. cURL: is used to fetch weather info, so this function must be enabled.
4. Composer: is used to install dependencies

## Roadmap

### Upcoming Features and Improvements

- [ ] Upgrades and Bug Fixes
- [ ] Added testing in the CI pipeline
- [ ] Add AWOS
- [ ] Upgrade UI to be more modern
- [ ] Added different TTS engine APIs, might try support for AI Generated voices

## Contributing

Contributions are what make the open source community such an amazing place to learn, inspire, and create. Any contributions you make are **greatly appreciated**.

If you have a suggestion that would make this better, please fork the repo and create a pull request. You can also simply open an issue with the tag "enhancement".
Don't forget to give the project a star! Thanks again!

1. Fork the Project
2. Create your Feature Branch (`git checkout -b feature/AmazingFeature`)
3. Commit your Changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the Branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

Distributed under the `CC BY-NC-SA 4.0` License. See `LICENSE` for more information. The `CC BY-NC-SA 4.0` License overrides the included `LICENSE` file. The LICENSE file included is a secondary license that also applies to this project and is included for reference.

## Contributors

<a href = "https://github.com/RedbeardTFL/ATIS_GENERATOR/graphs/contributors">
<img src = "https://contrib.rocks/image?repo=RedbeardTFL/ATIS_GENERATOR"/>
</a>

[contributors-shield]: https://img.shields.io/github/contributors/RedbeardTFL/ATIS_GENERATOR.svg
[contributors-url]: https://github.com/RedbeardTFL/ATIS_GENERATOR/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/RedbeardTFL/ATIS_GENERATOR.svg
[forks-url]: https://github.com/RedbeardTFL/ATIS_GENERATOR/network
[issues-shield]: https://img.shields.io/github/issues/RedbeardTFL/ATIS_GENERATOR.svg
[issues-url]: https://github.com/RedbeardTFL/ATIS_GENERATOR/issues
[license-shield]: https://img.shields.io/badge/License-CC_BY--NC--SA_4.0-lightgrey.svg
[license-url]: https://creativecommons.org/licenses/by-nc-sa/4.0/
[ci-shield]: https://woodpecker.vahngomes.dev/api/badges/RedbeardTFL/ATIS_GENERATOR/status.svg
[ci-url]: https://woodpecker.vahngomes.dev/RedbeardTFL/ATIS_GENERATOR
[forge-shield]: https://img.shields.io/endpoint?url=https%3A%2F%2Fforge.laravel.com%2Fsite-badges%2Fdfb30462-772c-4427-afe7-bb17de5c40f2%3Fdate%3D1%26commit%3D1&style=plastic
[forge-url]: https://forge.laravel.com/servers/699079/sites/2035675
