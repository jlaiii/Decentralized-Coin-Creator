# Decentralized Coin Creator

This is a simple, decentralized web application for creating and managing your own digital coins. It leverages the Gun.js database for peer-to-peer data storage, meaning your coin's data is distributed across the network and isn't dependent on a central server.

---

## Features

* **Create Your Own Coin:** Define a custom name and symbol for your unique digital currency.
* **Decentralized Data:** Coin information, accounts, and transactions are stored on the Gun.js peer-to-peer network.
* **Owner Admin Panel:** Securely manage user accounts and mint new coins for your currency.
* **User Accounts:** Users can create accounts for any listed coin, log in, view their balance, and transfer coins to other users.
* **Transaction History:** View a record of all transactions for your coin (as admin) or for your specific user account.

---

## How to Use

1.  **Host on GitHub Pages:** Clone this repository and host it on GitHub Pages. The application is a single HTML file and runs entirely in the browser.
    * [Link to this repository on GitHub](https://github.com/your-username/your-repo-name) (Remember to replace `your-username/your-repo-name` with your actual repository details after you push the code.)
2.  **Create a New Coin:**
    * Click "Create a New Coin".
    * Enter a **Coin Name**, a **Coin Symbol** (2-5 uppercase letters), and an **Admin Password**.
    * Click "Create My Coin".
    * **Important:** Note down your Coin ID (Symbol) and Admin Password. The username for the admin panel is always `owner`.
3.  **Explore Coins & Create Accounts:**
    * Browse the "Explore All Coins" section to see newly created coins (including yours!).
    * Click "Create Account" on any coin to make a new user account with a username and password.
4.  **Login & Transfer:**
    * Use "Login to Account" to access your user account.
    * If you log in as `owner` with your admin password on your coin's card, you'll be redirected to the **Admin Panel**.
    * As a user, you can transfer coins to other users from your account.
5.  **Admin Panel:**
    * From the admin panel, you can "Give Coins" (mint) to any user and view all accounts and transactions for your coin.

---

## Technical Details

* **Gun.js:** Provides the decentralized, real-time database capabilities.
* **CryptoJS:** Used for hashing passwords securely before storage.
* **HTML, CSS, JavaScript:** The entire application is built using standard web technologies and runs client-side.

---

## Getting Started (Development)

To run this project locally:

1.  Clone the repository:
    ```bash
    git clone [https://github.com/your-username/your-repo-name.git](https://github.com/your-username/your-repo-name.git)
    cd your-repo-name
    ```
2.  Open `index.html` in your web browser.

---

## Database Reset / Fresh Start

If you want to clear all data and start with a blank slate, you can modify the `DB_ROOT_NAME` constant in `index.html`. For example, change it from `'decentralized_coin_creator_v4'` to `'decentralized_coin_creator_v5'` (or any new unique string). This effectively creates a new, empty data space on the Gun.js network for your application instance.

```javascript
// In index.html, find this line:
const DB_ROOT_NAME = 'decentralized_coin_creator_v4';

// Change it to something new:
const DB_ROOT_NAME = 'decentralized_coin_creator_v5'; // Or any other unique name
