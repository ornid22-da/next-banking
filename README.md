# Horizon Banking Web App
### Using Next.js, Appwrite, Plaid, Dwolla, Typescript


## Deployment
The project is currently deployed on Vercel.
- **Demo**: [Open Live Demo](https://next-banking-horizon.vercel.app/)
- **Note**: The application is a little bit slow, because of how the data is rendered, so bear with it a little bit.


## Sign-in Page
### Users can sign-in into the application with their email or password
- **Note**: For testing, use these credentials: email: "email@test.com", password: "12345678"
### 
![Screenshot 2024-12-02 145131](https://github.com/user-attachments/assets/da93e2c7-4b17-4506-b9b5-1865de906f78)


## Sign-up Page
### Unregistered users can sign-up on this page, just by adding some basic info
- **Note 1**: Currently the web app is setup for users in USA, so to test, add USA specific values for fields like city, state, postal code, ssn, or else use these values: City: "New York", State: "NY", Postal Code: "11001", SSN: "1234"\
- **Note 2**: Setting up a bank account using Plaid, will require you to enter credentials at some point like username and password, which are username: "user_good", password: "pass_good", and for other pages like otp code, just hit submit\
- **Note 3**: Select any bank you want to add, then select any of the given bank account options that you want to add
### 
![Screenshot 2024-12-02 145055](https://github.com/user-attachments/assets/4643d454-8bbe-4778-a279-ab888bb85b2a)


## Home Page / Dashboard
### Main Page where users can view a super-useful dashboard, which includes their transactions, their spending categories, other banking facilities, their balance, bank accounts etc.
![Screenshot 2024-12-02 145246](https://github.com/user-attachments/assets/e37cc96a-5f15-47c0-b5b0-9ed59b33c248)


## My Banks Page
### Users can view their current bank accounts, as well as copy their account id, which they can use to do payments to other users
![Screenshot 2024-12-02 145349](https://github.com/user-attachments/assets/59764cac-fdbc-4a1a-bd93-92838179a708)


## Transaction History Page
### Users can view their account transaction history on this page
- **Note 1**: Whichever account is selected on the home page (if multiple), that account's transaction history will be displayed in this page\
- **Note 2**: Currently this page does not have the option of selecting different accounts, because that would simply mean that one of the section of the homepage is expanded here, which is not the motive of this page. Maybe the future update will have a solution to this.
###
![Screenshot 2024-12-02 145502](https://github.com/user-attachments/assets/9237195b-2124-4d5e-9009-fb50d7fcc319)


## Funds Transfer Page
### Users can transfer funds to other users of this application
- **Note**: Users can also transfer funds to one of their other bank accounts, since each account has an id, so one user having multiple bank accounts linked, each of their accounts will have a unique id for payments.
###
![Screenshot 2024-12-02 145524](https://github.com/user-attachments/assets/5c63a46f-ced4-4430-a4d6-526ae8dd35bb)


## Connecting Bank Accounts
### Users can connect their bank accounts through this functionality
- **Note**: Currently Plaid and Dwolla, which are used for Bank accounts and Fund Transfers, are running in Sandbox mode, hence all accounts of all banks will be in demo / test mode, and if you are stuck at some login credentials page, refer to Sign-up Page notes
###
![Screenshot 2024-12-02 145653](https://github.com/user-attachments/assets/a4a48e36-5b0a-4ee4-b315-9e64a6e64013)


## Getting Started...
### `npm run dev`
Runs the app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.\
Set up the database required in Appwrite, setup accounts in Plaid and Dwolla, and all the required keys in .env file, for example refer to .env.example file.
