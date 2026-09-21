<p align="center">
	<img 
        width="320"
        src="https://github.com/ervinsvilumsons/bloom/blob/main/wp-content/logo.png"
        alt="Bloom In Your Day"
    >
</p>

##

![PHP 8.4+](https://img.shields.io/badge/PHP-8.4%2B-777BB4?logo=php)
[![Docker](https://img.shields.io/badge/Docker-required-2496ED?logo=docker&logoColor=white)](https://docs.docker.com/get-docker/)
[![Docker Compose](https://img.shields.io/badge/Docker%20Compose-%3E%3D2-2496ED?logo=docker&logoColor=white)](https://docs.docker.com/compose/)

## 🎨 Design 

Theme [Kadence](https://wordpress.org/themes/kadence/)

Font [Josefin Sans](https://fonts.google.com/specimen/Josefin+Sans?preview.script=Latn)
<details>
<summary>Color Palette</summary>

| Color | Hex |
|---|---|
| 🟥 Pink Gold | `#F2D6CE` |
| 🟫 Eunry | `#CFA69A` |
| ⬛ Dravit Grey | `#5D5D5D` |
| ⬜ Pale Silver | `#EBEBEB` |

</details>

## 🧩 Plugins

<details>
<summary>Installed with Composer</summary>

- AccessiYes (`accessibility-widget`)
- CookieYes | GDPR Cookie Consent (`cookie-law-info`)
- EWWW Image Optimizer (`ewww-image-optimizer`)
- Flexible SSL for CloudFlare (`cloudflare-flexible-ssl`)
- Google Analytics Dashboard for WP (`google-analytics-dashboard-for-wp`)
- Meta Tag Manager (`meta-tag-manager`)
- OneSignal Push Notifications (`onesignal-free-web-push-notifications`)
- Polylang (`polylang`)
- Really Simple Security (`really-simple-ssl`)
- Simple Local Avatars (`simple-local-avatars`)
- Smash Balloon Social Photo Feed (`instagram-feed`)
- Hubbub Lite (`social-pug`)
- Ultimate Dashboard (`ultimate-dashboard`)
- UpdraftPlus - Backup/Restore (`updraftplus`)
- W3 Total Cache (`w3-total-cache`)

</details>

<details>
<summary>Install manually</summary>

- WP Cerber (`wp-cerber`)

</details>

## 🚀 Setup

### 📋 Requirements

- A running MySQL container or service reachable as [mysql](https://github.com/ervinsvilumsons/public-services#-services)

### 📦 Installation

1. Clone the repository and open its directory.
    ```bash
    git clone git@github.com:ervinsvilumsons/bloom.git
    ```

2. Create the local environment file:

    ```bash
    cp .env.example .env
    cp wp-config-sample.php wp-config.php
    ```

3. Update `.env` and `wp-config.php` with the database credentials and site URL for your environment.
4. Add [.htaccess](https://developer.wordpress.org/advanced-administration/server/web-server/httpd/#basic-wp) file.
5. Run Composer install.

    ```bash
    composer install
    ```

6. Start the WordPress container:

    ```bash
    make build
    ```

7. Open the site at the URL configured by `WP_SITEURL` (the example uses `http://localhost:9001`).