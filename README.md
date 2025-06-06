# Decentralized Coin Creator

A simple, browser-based application for creating and managing your own decentralized digital coins, powered by Gun.js. This project allows anyone to launch their unique currency, manage user accounts, and track transactions directly in their browser without the need for a central server.

## Features

* **Create Your Own Coin:** Define a unique name and symbol for your digital currency.
* **Decentralized:** Built on Gun.js, meaning data is distributed and stored across connected peers.
* **Admin Panel:** Securely manage user accounts and mint (give) coins as the owner.
* **User Accounts:** Users can create accounts for any listed coin, log in, view their balance, and transfer coins to other users.
* **Transaction History:** View a record of all transactions (mints and transfers) for a coin.
* **Browser-Based:** No backend setup required; simply open the HTML file in a web browser.

## How It Works

This application leverages [Gun.js](https://gun.eco/), a real-time, decentralized, offline-first, graph database. All coin data, including creation, accounts, and transactions, is stored and synchronized across the Gun.js network.

## Live Demo

Experience the Decentralized Coin Creator live in your browser:
[https://jlaiii.github.io/Decentralized-Coin-Creator/](https://jlaiii.github.io/Decentralized-Coin-Creator/)

## Getting Started

To run this project locally:

1.  **Clone the repository:**
    ```bash
    git clone [https://github.com/jlaiii/Decentralized-Coin-Creator.git](https://github.com/jlaiii/Decentralized-Coin-Creator.git)
    ```
2.  **Navigate to the project directory:**
    ```bash
    cd Decentralized-Coin-Creator
    ```
3.  **Open `index.html` in your web browser.**

That's it! The application will connect to a public Gun.js peer and be ready for use.

## Usage

### Creating a New Coin

1.  Click the "Create a New Coin" button.
2.  Enter a **Coin Name**, a unique **Coin Symbol** (2-5 uppercase letters), and an **Admin Password**.
3.  Click "Create My Coin".
4.  Remember your **Coin ID (Symbol)** and that the default **Username for Admin Panel is `owner`**.

### Accessing the Admin Panel (as Owner)

1.  Find your coin in the "Explore All Coins" list.
2.  Click "Login to Account" on your coin card.
3.  Enter **Username:** `owner` and your **Admin Password**.
4.  Upon successful login, you will be redirected to the Admin Panel for your coin.

### Creating a User Account

1.  Find the desired coin in the "Explore All Coins" list.
2.  Click "Create Account" on the coin card.
3.  Choose a **Username** and a **Password**.
4.  Click "Create Account".

### Logging In as a User

1.  Find your coin in the "Explore All Coins" list.
2.  Click "Login to Account" on your coin card.
3.  Enter your **Username** and **Password**.

### Transferring Coins

1.  Ensure you are logged into a user account on a coin.
2.  Click "Transfer Coins" on that coin's card.
3.  Enter the **Recipient Username** and **Amount** to transfer.
4.  Click "Confirm Transfer".

## Contributing

Feel free to fork this repository, open issues, or submit pull requests.

## License

This project is open-source and available under the [MIT License](LICENSE).
