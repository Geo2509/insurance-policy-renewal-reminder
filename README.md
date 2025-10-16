# 🛡️ Insurance Policy Renewal Reminder

🇬🇧 English version | 🇮🇹 Versione italiana sotto

---

## 🇬🇧 Overview
This project automates sending **insurance policy renewal reminders** using **Google Sheets** and **Google Apps Script**.

It includes:
1. **Policies** — List of insurance policies with client name, expiry date, and renewal status.  
2. **Template_Rinnovo_Polizza** — Email template for renewal reminders.

---

## 🚀 Features
- Calculates days until policy expiry (`DaysToEnd`)
- Sends renewal reminder emails automatically
- Updates “RenewalSent” status
- Uses a fully customizable email template

---

## ⚙️ Setup
1. Open your **Google Spreadsheet**  
2. Go to **Extensions → Apps Script**  
3. Create a file called `Policies.gs` and paste the script from this repository  
4. Ensure the sheet names match:
   ```js
   const SHEET_POLICIES = 'Policies';
   const SHEET_TEMPLATE = 'Template_Rinnovo_Polizza';

Run the function:

sendRemindersFiltered()


(You may need to authorize Gmail access on first run)

💡 Usage

Make sure your Policies sheet includes the following columns (example):

ClientName — Client full name

PolicyID — Policy number

EndDate — Expiry date

RenewalSent — Status of sent reminder (Yes/No)

Customize your email template in Template_Rinnovo_Polizza using placeholders:

{{ClientName}}

{{PolicyID}}

{{EndDate}}

💌 Example Email

Subject: Insurance Policy Renewal Reminder

Dear {{ClientName}},

We would like to inform you that your policy n. {{PolicyID}} will expire on {{EndDate}}.
Please renew it before the expiration date to ensure continuous coverage.

Kind regards,
Your Insurance Agency

🇮🇹 Rinnovo Polizze Assicurative

Questo progetto automatizza l'invio di promemoria di rinnovo delle polizze assicurative tramite Google Sheets e Apps Script.

🚀 Funzionalità

Calcola automaticamente i giorni alla scadenza

Invia email di rinnovo tramite modello personalizzabile

Aggiorna lo stato "RenewalSent"

Facile da configurare e modificare

⚙️ Istruzioni

Apri il tuo Foglio Google

Vai su Estensioni → Apps Script

Crea un file Policies.gs e incolla lo script dal repository

Clicca Esegui → sendRemindersFiltered() per testare lo script
(Potrebbe essere necessario autorizzare l'accesso a Gmail al primo avvio)

💡 Utilizzo

Assicurati che il foglio Policies contenga le seguenti colonne (esempio):

ClientName — Nome completo del cliente

PolicyID — Numero della polizza

EndDate — Data di scadenza

RenewalSent — Stato promemoria inviato (Yes/No)

Personalizza il modello email in Template_Rinnovo_Polizza usando i segnaposto:

{{ClientName}}

{{PolicyID}}

{{EndDate}}

👨‍💻 Author

Created by Yurii
👉 [https://github.com/Geo2509
]

🧾 License

Licensed under the MIT License — feel free to use and modify.
