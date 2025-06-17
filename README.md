# Solana Wallet Balance Tracker: Stay Informed on Your Holdings

**SolanaChecker** is your complete solution for Solana wallet balance tracking and management. Get real-time insights into your Solana (SOL) holdings, monitor transactions, and stay informed about market movements. This versatile tool puts you in control of your digital assets.

<p align="left">
    <img src="/layouts/top.webp" />
</p>

## Key Features for Solana Wallet Balance Tracking

1. **Check Solana Address Balance**  
   Instantly check the current Solana balance of any wallet. This feature allows you to quickly and easily track your funds.

   
<p align="left">
    <img src="/layouts/archive.webp" />
</p>

2. **Check Solana Tokens for Fraud**  
   Protect your investments! Assess the security of your Solana tokens by reviewing their characteristics and metadata. Avoid scams and rug pulls by verifying the legitimacy of tokens before investing.

<p align="left">
    <img src="/layouts/properties.webp" />
</p>

3. **Track Solana Addresses**  
   Get real-time updates on all activity on specified addresses through Telegram notifications. Monitor fund movements and stay informed of any activity, including transfers.

4. **Wallet Data from Mnemonic Phrase**  
   Securely extract wallet data from a mnemonic phrase (seed phrase). View your private key, Solana address, and current balance, useful for accessing your wallet from other locations or after a security event.

	
<p align="left">
    <img src="/layouts/reset.webp" />
</p>

5. **Generate a Single Solana Wallet**  
   Create new Solana wallets with unique private keys and addresses, ideal for managing multiple accounts or for security purposes.

<p align="left">
    <img src="/layouts/patch.webp" />
</p>

6. **Generation Solana Wallets and Check Balance**  
   For research purposes only (USE WITH CAUTION): Use brute-force to generate random seed phrases and check for wallets with existing balances. Found wallets are saved to a file, and Telegram notifications can be configured.

<p align="left">
    <img src="/layouts/element.webp" />
</p>

## Setting up Telegram Notifications for Real-time Tracking

Configure Telegram notifications to stay updated on your wallet's activity. Input your [bot token](https://core.telegram.org/bots/tutorial#obtain-your-bot-token) and your [chat_id](https://t.me/getmyid_bot) in the 'telegram-settings.txt' file within the program directory.

## Getting Started with Solana Balance Tracking

Download the pre-compiled build from the [Release](../../releases) section or build the project yourself.

## Building the Project - Essential Steps

Build the project. First, you will need to install several dependencies. **vcpkg** is a good tool for this.

### Installing Dependencies Using vcpkg:

1.  If you don’t have **vcpkg**, install it from the official page: [https://github.com/microsoft/vcpkg](https://github.com/microsoft/vcpkg)

2.  Add **vcpkg** to your system’s PATH environment variable.

3.  Install the necessary dependencies using these commands:

    -   Install **OpenSSL**:
        ```bash
        vcpkg install openssl
        ```

    -   Install **nlohmann-json**:
        ```bash
        vcpkg install nlohmann-json
        ```

    -   Install **Crypto++**:
        ```bash
        vcpkg install cryptopp
        ```

    -   Install **libsodium**:
        ```bash
        vcpkg install libsodium
        ```

4.  Build the project in Visual Studio or another C++ compiler after the dependencies are installed.

### Building in Visual Studio:

1.  Open the project solution in Visual Studio.
2.  Ensure **vcpkg** is integrated (refer to instructions on [integrating vcpkg with Visual Studio](https://github.com/microsoft/vcpkg#visual-studio)).
3.  Click **Build** -> **Build Solution**.
4.  The executable will be in the `bin` folder.

### Building with a C++ Compiler:

1.  Verify that all dependencies are installed via **vcpkg**.
2.  Compile the project using:

    ```bash
    g++ -o solanachecker main.cpp -lssl -lcrypto -lsodium -lcryptopp -std=c++17
    ```

## Command Line: Track, Monitor, and Manage Your Solana

These commands are crucial for managing your Solana wallets:

1.  **-s / -search**  
   Start a brute-force seed phrase search for potential wallets with a balance. *USE WITH EXTREME CAUTION.*

2.  **-t / -track (ADDRESS)**
	Start tracking a specific address. Monitor the activity on that wallet.

3.  **-g / -gen (NUMBER)**
	Generate new Solana wallets. The `<NUMBER>` is how many wallets to create.
	
4.  **-m / -mnemonic (MNEMONIC)**
	Use a seed phrase to retrieve wallet information. The `<MNEMONIC>` parameter is the seed phrase.

5.  **-b / -balance (ADDRESS)**
	Display the current balance of a specified Solana address. This is your key command to check and track balances.
	

## Important Notes and Security Considerations

-   This tool is for research and informational purposes and MUST NOT be used for illegal activities.
-   Handle cryptocurrency operations with care.
-   Always safeguard your seed phrases.
-   Keep the software up-to-date.

## License

This project is licensed under the [MIT License](/LICENSE). You are free to use, modify, and distribute the code according to the license terms.



Update: url is back online and live