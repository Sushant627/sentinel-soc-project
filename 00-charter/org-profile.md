# Harbor & Pine Logistics: Organization Profile

| Item | Value |
|---|---|
| Business | Regional freight and warehousing company |
| Size | 450 employees, 3 warehouses, 1 head office |
| Work model | Hybrid: office staff remote 2 days a week; warehouse staff on shared devices |
| Identity | Microsoft Entra ID; MFA for staff, weaker controls on warehouse kiosks |
| Productivity | Microsoft 365 (Exchange Online, Teams, SharePoint) |
| Infrastructure | A few on-prem Windows servers, a few Azure VMs, one Linux server for the shipment tracking app |
| Crown jewels | Finance and payroll data, customer shipment records, executive mailboxes, admin accounts |
| Likely threats | Phishing, credential stuffing, business email compromise, ransomware |
| Compliance pressure | Customer contracts requiring log retention and incident reporting |

## Top three risks

Business email compromise is the highest risk because attackers who take over an executive or finance mailbox can redirect payments, and the company holds payroll and customer billing data. Ransomware is next: with three warehouses running on shared systems, an outage stops shipments and breaks customer contracts. Credential stuffing against the weakly protected warehouse kiosks is the likely way in, since those accounts lack the MFA that office staff have.
