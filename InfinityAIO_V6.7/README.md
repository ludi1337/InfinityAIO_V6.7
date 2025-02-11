** MOST UP 2 DATE GUIDE **
https://infinity-scripts.gitbook.io/infinity-aio
https://infinity-scripts.gitbook.io/infinity-aio
https://infinity-scripts.gitbook.io/infinity-aio
https://infinity-scripts.gitbook.io/infinity-aio
https://infinity-scripts.gitbook.io/infinity-aio
https://infinity-scripts.gitbook.io/infinity-aio
https://infinity-scripts.gitbook.io/infinity-aio
https://infinity-scripts.gitbook.io/infinity-aio
https://infinity-scripts.gitbook.io/infinity-aio
https://infinity-scripts.gitbook.io/infinity-aio
** MOST UP 2 DATE GUIDE **
















First Time Installation
1. Install NodeJS (https://nodejs.org/en/download/)
2. Install Dependencies (npm install)
3. Run the project (npm run start)

** DO NOT SHARE YOUR PRIVATE KEYS WITH ANYONE **
** I SUGGEST HIGHLY TO RUN STEPS 1-6 IN ORDER (4 is optional) FOR BEST RESULTS **
** STOP USING FREE RPCS AND COMPLAINING NOTHING LANDS, USE A PAID RPC **

ENV SETUP
RENAME THE FILE TO .env

SIGNER_PRIVATE_KEY = PRIVATE KEY OF DEV WALLET
DEV_ADDRESS = WALLET ADDRESS OF DEV WALLET (PUBLIC KEY)
FUNDER_PRIVATE_KEY = PRIVATE KEY OF FUNDER WALLET (WALLET THAT WILL FUND THE SUB WALLETS)
RPC_URL = YOUR RPC URL (HTTP OR HTTPS)
WS = YOUR WS URL (WSS OR WS)
BLOCKENGINEURL = JITO BLOCKENGINE URL (see list below)
JITO_TIP = JITO TIP AMOUNT (SOL)
SELL_TIP = SELL TIP AMOUNT (SOL)
NFT_STORAGE_TOKEN = DO NOT EDIT THIS DO NOT EDIT THIS DO NOT EDIT THIS DO NOT EDIT THIS DO NOT EDIT THIS 
DEVBUY = AMOUNT OF SOL TO BUY ON DEV WALLET
MINBUY = NO LONGER USED
MAXBUY = NO LONGER USED
LUT_Address = LOOKUP TABLE ADDRESS (DO NOT EDIT THIS, THE BOT WILL CREATE & UPDATE THIS)
BLOXKEY = BLOXROUTE API KEY (BEARER/HEADER/AUTH TOKEN FROM DASHBOARD)
BLOX_EP = BLOXROUTE ENDPOINT (LIST BELOW)
COMPUTE_LIMIT_PRICE = COMPUTE LIMIT PRICE (LAMPORTS) (https://www.solconverter.com/)
COMPUTE_UNIT = COMPUTE UNIT (LAMPORTS) (https://www.solconverter.com/)
CAP_SOLVER_API_KEY = CAP SOLVER API KEY (https://www.capsolver.com/)

NOTE: DUE TO SLIPPAGE THESE VALUES MAY NOT BE EXACT SO FUND WALLETS WITH EXTRA SOL

METADATA.JSON (METADATA SETUP)
1. Change the metadata in metadata.json to your desired metadata
2. MAKE SURE TO LEAVE IMAGE VALUE BLANK
3. YOU MUST PUT THE TOKEN IMAGE IN THE /img DIRECTORY 
4. TICKER / SYMBOL MAX 10 CHARACTERS
**ONE IMAGE IN DIRECTORY ONLY (NAME + EXTENTION DONT MATTER NOW)**

BLOCKENGINEURLS (pick the closest to your location):
AMSTERDAM: amsterdam.mainnet.block-engine.jito.wtf
FRANKFURT: frankfurt.mainnet.block-engine.jito.wtf
NEW YORK: ny.mainnet.block-engine.jito.wtf
TOKYO: tokyo.mainnet.block-engine.jito.wtf

BLOXROUTE ENDPOINTS:
NEW YORK: https://ny.solana.dex.blxrbdn.com
ENGLAND: https://uk.solana.dex.blxrbdn.com

MODES:
1. WALLET GEN: Generates wallets and stores the keypairs to /keypairs directory as JSON files & wallet.txt as pubkey:privkey 
2. WALLET UI:
  1: FUND: Funds the wallets with SOL (MUST RUN THIS BEFORE BUNDLER)
  2: BALANCE: Checks SOL Balance of all Sub Wallets
  3: TRANSFER TOKENS: Transfers the token from the SUB Wallets to the DEV wallet
  4: REFUND SOL: Returns all SOL from SUB wallets to Dev Wallet! (note 0.001 SOL is left in each wallet to pay rent fees)
  5: VANITY GEN: Creates a vanity token address ending in pump saved to /token directory
  6: CLOSE TOKEN ACCTS: Closes all token accounts in sub wallet to reclaim rent fees
  7: EXIT: Return to main menu

3. CREATE LOOKUP TABLE: Creates a lookup table to allow for 20 wallet buys in one go (MUST RUN THIS BEFORE BUNDLER)

4. PROFILE GEN: Generates profiles for the sub wallets on pump.fun (Random username + bio + coin holdings)

5. Launch UI:
  1: BUY AMOUNTS: SET THE BUY AMOUNTS PER WALLET
  2: LAUNCH TOKEN: LAUNCH & BUNDLE BUY YOUR TOKEN ON PUMP.FUN
  3: PNL: CHECK SUB WALLET PROFIT/LOSS AFTER YOU SELL (MAY BE INACCURATE)

6. SELL: 
  1: DUMP ALL: DUMPS 100% of tokens in every SUB wallet AND DEV WALLET in 1 go 
  2: DUMP %: DUMPS A SPECIFIC PERCENTAGE OF TOKENS IN EVERY SUB WALLET AND DEV WALLET
  3: DELAY SELL ALL: Sells 100% of supply in all SUB wallets with a delay between each TX 
  4: DELAY SELL %: Sells a specific percentage of supply in all SUB wallets with a delay between each TX
  5: SINGLE SELL (%): Sells a specific percentage of supply in a single SUB wallet (enter 100 to sell all tokens in a single wallet)
  6: DEV DUMP: Transfers all tokens from SUB wallets -> Dev Address from .env then DUMPS 100% of tokens in Dev Wallet

7. RAYDIUM:
  1: CREATE WSOL: Creates WSOL Accounts for every wallet + dev wallet
  2: RAY LUT: Extends LUT to include Raydium Data (SUPER IMPORTANT)
  3: RAY SELL: Sells tokens on Raydium (Enter % and include dev (T F)) (T = True, F = False) (0-100 %)
  4: UNWRAP: Unwraps WSOL to SOL
  5: EXIT: Return to main menu

8. EXIT: Exits the program

NOTE:
1. WALLETS WILL BE OVERWRITTEN IF YOU RUN WALLET GEN AGAIN SO REMOVE ALL SOL FROM THEM BEFORE RUNNING WALLET GEN AGAIN

NOTE: As of v0.04 All Keypairs/Wallets ever made on the version will be stored in /keypairBackup directory & /walletBackup directory

2. DO NOT MODIFY MINT.JSON or ANY FILES IN THE /res directory
3. DO NOT MODIFY THE NFT STORAGE KEY IN .env
4. DO NOT MODIFY THE PUMP-IDL.JSON FILE

** DO NOT SHARE YOUR PRIVATE KEYS WITH ANYONE **
** I SUGGEST HIGHLY TO RUN STEPS 1-6 IN ORDER (4 is optional) FOR BEST RESULTS **
** STOP USING FREE RPCS AND COMPLAINING NOTHING LANDS, USE A PAID RPC **
