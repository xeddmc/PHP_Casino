
# Casino Script

This is a PHP-based web casino platform that provides slot games, jackpots, promotions, and user management.  
It allows you to set up a simple online casino environment/platform with modular components.

This project is *BETA* 0.2.0
Please don't use this yet in production settings unless you know what you're at. I have yet to scour this for possible vulnerabilites as the codebase is older.

---

## Project Structure

The repository is organized into several key directories:

- **`engine/`** – Core backend logic and casino engine functions  
- **`engine_acp/`** – Admin control panel engine scripts  
- **`games/`** – Game logic and assets (slot machines, etc.)  
- **`jackpot/`** – Jackpot system implementation  
- **`modules/`** – Reusable modules (payment, authentication, etc.)  
- **`promo/`** – Promotional features and bonus handling  
- **`templates/`** – HTML/Smarty templates for UI rendering  
- **`images/` / `img/`** – Static assets (icons, banners, etc.)  
- **`logs/`** – Logging system for activity and errors  
- **`share42/`** – Social sharing integration  
- **Root files:**
  - `index.php` – Main entry point  
  - `game.php` – Game execution logic  
  - `slots.php` – Slot machine handler  
  - `page.php` – Page rendering  
  - `payeer_merchant.php` – Payment gateway integration (Payeer)  
  - `bd.sql` – Database schema (MySQL)  
  - `winners.xml` – Stores recent winners for display  

---

## Requirements

- **Web Server:** Apache/Nginx with PHP 5.6+  
- **Database:** MySQL/MariaDB  
- **Extensions:**  
  - `mysqli`  
  - `mbstring`  
  - `gd` (for image handling)  

---

## Installation

1. **Clone the repository:**
   ```bash
   git clone https://github.com/RomaniukVadim/casino_script.git
   cd casino_script
   
   ````

2. **Set up the database:**

   ```bash
   mysql -u root -p casino_db < bd.sql
   ```

   Update the database credentials in `engine/config.php`.

3. **Configure the web server:**

   * Point your document root to the repo folder.
   * Ensure `index.php` is accessible.

4. **Payment integration:**

   * Configure `payeer_merchant.php` with your Payeer merchant credentials.

---

## Features

* Slot machine games with configurable odds
* Jackpot system with progressive accumulation
* User registration and authentication
* Payment gateway integration (Payeer)
* Admin control panel (`engine_acp/`)
* Logging and reporting system
* Promotional bonuses and campaigns
* Social sharing support via `share42`

---

## Security Notes

* This project is **educational/demo software** and not production-ready.
* Always sanitize user input and secure database connections.
* Consider using **HTTPS** and modern PHP versions for deployment.

---

## Contributing

Pull requests are welcome!
Please read **CONTRIBUTING.md** for guidelines.

---

## License

This project is licensed under the **GNU GPL v3.0** – see `LICENSE.md` for details.

---

## Authors

* **Vadim Romaniuk** – Initial work
* **Community contributors**

---

## Disclaimer

This script is provided *as-is* for educational purposes.
Running real-money casinos may require legal compliances, KYC and AML Laws in your jurisdiction.
Use responsibly. Use your head.

