# B&M Web Application Requirements Document\n
## 1. Application Overview
### 1.1 Application Name
B&M

### 1.2 Application Description
B&M is an investment platform where users can deposit cryptocurrency and earn interest returns. The platform features a daily reward card system, referral rewards, recharge bonuses, secure crypto deposits, KYC verification, and monthly withdrawal functionality.
\n## 2. Core Features\n
### 2.1 User Authentication
- Google Login (OSS Google login method)
- User profile display with DP, name, flag, and KYC verification status

### 2.2 Home Page
- Attractive business-themed images (10 auto-scrolling promotional images)
- Finance section displaying:
  - Wallet box showing user balance
  - Credit counter (real-time counting display)
  - Interest display (showing accumulated interest)
  - Reward card indicator (showing collection status: e.g., '2 times collected, 1 time remaining')
  - Large-sized reward card (award-type display)
  - User profile section with DP, name, flag, and KYC status
\n### 2.3 Daily Reward Card System
- Users can redeem cards 3 times daily at fixed times: 8 AM, 4 PM, and 10 PM
- Each card provides 6% of user's wallet amount, divided into 3 daily distributions (2% per redemption)
- Card displays colorful design with coin rewards
- After clicking to redeem, card shows 'DONE ✅' status\n- Next available redemption time is displayed

### 2.4 Referral System\n- Each user receives a unique referral code/link
- Referral dashboard showing:
  - Total referrals count
  - Active referrals
  - Total earnings from referrals (one-time + monthly)
  - Referral history with timestamps\n- Referral rewards structure:\n  - One-time reward: 5% of referred user's first recharge amount
  - Monthly passive income: 4% of referred user's monthly earnings
- Share options: Copy referral link, share via social media (WhatsApp, Telegram, Facebook, Twitter)

### 2.5 Recharge Bonus System
- 8% bonus on every recharge/deposit
- Bonus is instantly credited to user wallet upon deposit approval
- Bonus history displayed in transaction record
- Example: User deposits $100, receives $108 total ($100 + $8 bonus)

### 2.6 Wallet System\n- Display sections: Wallet Balance, Deposit, Record
- Wallet shows total available balance
- Credit counter with real-time counting animation
- Interest display showing daily and total accumulated interest
- Deposit section shows pending and completed deposits\n- Record section shows transaction history including bonuses and referral earnings

### 2.7 Deposit System
- Support for 3 cryptocurrency networks:
  - BSC (BEP-20): 0xe5a646318e3909afabc11c1b0c2b29fcc961b280
  - TRON (TRC-20): TDvrj5yXXpdAje1bfcEvuKMWZ5UG5TrFuF
  - ETH (ERC-20): 0xe5a646318e3909afabc11c1b0c2b29fcc961b280\n- User interface:
  - Display all 3 wallet addresses\n  - Allow users to upload transaction receipt/proof image
  - Show 'Pending' status after submission
- Admin verification:
  - Admin can review and approve deposits
  - Upon approval, amount + 8% bonus reflects in user's wallet

### 2.8 KYC Verification
- Required documents:
  - ID verification
  - Live selfie
  - Mobile number verification
- Users can access basic features before KYC, but full functionality requires verification

### 2.9 Withdrawal System
- Monthly withdrawal available on the 10th of each month\n- Users can withdraw accumulated interest, bonuses, and referral earnings\n
### 2.10 Investment Model
- Company holds user deposits and provides interest returns
- Interest is distributed through daily reward cards (6% daily, split into 3 redemptions)

### 2.11 Owner Panel Dashboard
- Admin authentication with secure login
- Dashboard overview displaying:\n  - Total users count
  - Total deposits (pending and approved)
  - Total withdrawals processed
  - Active users today\n  - Total interest distributed
  - Total bonuses paid
  - Total referral commissions\n- User management:
  - View all registered users
  - Search and filter users by status, KYC verification, registration date
  - View individual user details (balance, deposits, withdrawals, referrals)
  - Suspend or activate user accounts
- Deposit management:
  - View pending deposits with uploaded proof images
  - Approve or reject deposits
  - View deposit history with filters
- Withdrawal management:
  - View withdrawal requests
  - Process monthly withdrawals
  - View withdrawal history
- KYC verification management:
  - Review pending KYC submissions
  - Approve or reject KYC documents
  - View user ID, selfie, and mobile verification status\n- Referral system monitoring:\n  - View referral statistics\n  - Track referral earnings distribution (one-time + monthly)
  - Monitor top referrers\n  - View referral network tree
- Financial reports:
  - Daily, weekly, monthly revenue reports
  - Interest distribution reports
  - Bonus payout reports
  - Referral commission reports
  - Export reports in CSV/PDF format
- System settings:
  - Configure interest rates
  - Set bonus percentages
  - Manage referral commission rates (first recharge bonus, monthly earnings percentage)\n  - Update cryptocurrency wallet addresses\n
### 2.12 Settings
- Settings button accessible from user profile
- Settings options include:
  - Language selection (support for multiple languages: English, Urdu, Hindi, Chinese, Spanish, Arabic)
  - Notification preferences (email, push notifications)
  - Account security settings (password change, 2FA toggle)
  - Display preferences (theme, currency display format)
  - Privacy settings (data sharing preferences)

### 2.13 FAQ Section\n- Comprehensive FAQ page covering:\n  - How to deposit cryptocurrency\n  - How the daily reward card system works
  - Interest calculation and distribution
  - Referral system and earning commissions (one-time + monthly passive income)
  - Recharge bonus details\n  - KYC verification process
  - Withdrawal schedule and procedures
  - Security and fund safety
  - Supported cryptocurrencies
  - Account management

### 2.14 Privacy Policy
- Data collection and usage disclosure
- User information protection measures
- Cookie policy and tracking technologies
- User rights regarding personal data (access, deletion, modification)
- Data retention and deletion policies
- Contact information for privacy inquiries

### 2.15 Security Measures\n- End-to-end encryption for all transactions
- Two-factor authentication (2FA) option for user accounts
- Secure storage of cryptocurrency wallet addresses
- Regular security audits and vulnerability assessments\n- Anti-fraud detection systems\n- Cold storage for majority of user funds

### 2.16 Third-Party Services\n- Disclosure of third-party service providers:
  - Payment processors for cryptocurrency transactions
  - KYC verification service providers
  - Cloud hosting and data storage partners\n  - Analytics and performance monitoring tools
- Third-party data sharing policies
- User consent for third-party integrations

### 2.17 Terms of Service
- User eligibility and account registration requirements
- Prohibited activities and user conduct guidelines
- Platform liability limitations
- Dispute resolution procedures
- Service modification and termination rights
- Governing law and jurisdiction

## 3. Design Style
- Color scheme: Full black background (#000000) throughout the entire application, white borders (#ffffff) for all boxes and containers, gold accents (#ffd700) for reward card elements with metallic sheen, green highlights (#00ff00) for bonus indicators
- Typography: Large-sized white text (#ffffff) for primary content to ensure high visibility, semi-transparent white text (rgba(255, 255, 255, 0.5)) for secondary information and labels
- Visual effects: Simple 3D appearance with subtle depth using layered shadows (04px 8px rgba(255, 255, 255, 0.1)), shining effects on interactive elements with animated gradient overlays, glossy finish on buttons and cards with light reflection effects, pulsing glow on bonus notifications
- Layout: Mobile-optimized single-screen layout with no scrolling required, all content fits within viewport height (100vh), compact card-based design with white outlined boxes (2px solid borders) featuring 3D elevation, collapsible sections for detailed information, swipeable tabs for navigation between wallet/deposit/record sections, prominent reward card with gold metallic shine positioned at top, referral section accessible via bottom navigation, settings icon in top-right corner with hover shine effect, owner dashboard with hamburger menu and condensed data cards