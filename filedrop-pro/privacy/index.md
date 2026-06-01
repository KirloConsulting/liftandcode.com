---
layout: page
title: Privacy Statement
description: FileDrop Pro Privacy Statement
permalink: /filedrop-pro/privacy/
---

**Product:** FileDrop Pro
**Publisher:** Lift & Code
**Last updated:** 2026-05-26
**Effective date:** From first publication on Microsoft AppSource

This Privacy Statement explains how **Lift & Code** ("**we**", "**us**", "**our**") handles personal data in connection with the Microsoft Dynamics 365 Business Central extension **FileDrop Pro** (the "**Software**").

Lift & Code is the data controller for any personal data we collect directly from You as defined in Section 4. For all data processed inside Your Business Central tenant, **You** are the data controller and Microsoft is the data processor under Your existing agreements with Microsoft.

---

## 1. About us

**Lift & Code** (a brand of Kirlo Consulting), CVR no. 18803747
Istedgade 105 2TV, 1650 Copenhagen V, Denmark
Email: <support@liftandcode.com>

## 2. Scope

This Privacy Statement applies to:

- The FileDrop Pro extension installed in a Microsoft Dynamics 365 Business Central tenant
- The marketing and support pages at <https://liftandcode.com/filedrop-pro/>
- Any direct correspondence between You and Lift & Code regarding the Software

It does **not** apply to:

- Microsoft Dynamics 365 Business Central itself, which is governed by Microsoft's [Privacy Statement](https://privacy.microsoft.com/privacystatement)
- Microsoft AppSource, which is governed by Microsoft's [Commercial Marketplace](https://learn.microsoft.com/legal/marketplace/) terms

## 3. What FileDrop Pro does with data

FileDrop Pro is a client-side and server-side extension that runs **entirely inside Your Business Central tenant**. It does not transmit business data, file contents, or document metadata to Lift & Code or to any third party.

When You drop a file onto the FileDrop Pro factbox:

1. The file is read in Your browser by the JavaScript control add-in (`readAsDataURL`) and base64-encoded
2. The encoded file is sent over Your existing Business Central session to AL code running in Your tenant
3. The AL code writes the file to the standard Business Central tables `Incoming Document` and `Incoming Document Attachment` and links it to the host record (journal line, ledger entry, posted document, etc.)

No part of the file leaves Your Microsoft tenancy as a result of using FileDrop Pro.

## 4. Personal data we collect directly

The following limited categories of personal data may reach Lift & Code:

| Category | When collected | Purpose | Legal basis (GDPR) |
|---|---|---|---|
| Name, email, company | When You contact <support@liftandcode.com> or request a quote | Respond to Your enquiry, provide support | Art. 6(1)(b) — performance of contract / Art. 6(1)(f) — legitimate interest in supporting our customers |
| Tenant ID, environment name, BC version | If You include them voluntarily in a support request | Reproduce and diagnose the reported issue | Art. 6(1)(b) — performance of contract |
| Diagnostic telemetry (anonymised event names, error codes, stack traces — **no document content, no record IDs, no personal identifiers**) | When the Software encounters an error and Application Insights is enabled | Detect and fix defects in the Software | Art. 6(1)(f) — legitimate interest in maintaining a reliable product |

We do **not** collect:

- The content of any file You drop onto the factbox
- The content of any Business Central record (customer names, amounts, document numbers, etc.)
- Personally identifiable information about Your end-users beyond what You voluntarily share

## 5. Cookies and tracking

The FileDrop Pro extension itself sets **no cookies** and runs no tracking scripts. The marketing pages at <https://liftandcode.com> may use a minimal first-party analytics solution to count page views — details are disclosed in the site's cookie banner.

## 6. Sharing with third parties

We do not sell, rent, or trade Your personal data. We share data only with:

- **Microsoft Application Insights** (Microsoft Ireland Operations Ltd., Ireland), to receive the anonymised diagnostic telemetry described in Section 4. Microsoft's processing is governed by the [Microsoft Online Services Data Protection Addendum](https://www.microsoft.com/licensing/docs/view/Microsoft-Products-and-Services-Data-Protection-Addendum-DPA).
- **Email provider** — Microsoft 365, used to host the <support@liftandcode.com> mailbox.
- **Legal or regulatory authorities**, where required by law or to defend our legal rights.

All transfers within the EU/EEA rely on the applicable lawful basis under GDPR. We do not currently transfer personal data outside the EU/EEA in connection with FileDrop Pro.

## 7. Retention

| Data | Retention |
|---|---|
| Support correspondence | Up to 3 years from last contact, then deleted |
| Diagnostic telemetry in Application Insights | 90 days (default Application Insights retention) |
| Invoices / accounting records | 5 years, as required by Danish bookkeeping law (Bogføringsloven) |

## 8. Your rights under GDPR

If You are an individual in the EU/EEA, You have the right to:

- **Access** the personal data we hold about You
- **Rectify** inaccurate or incomplete data
- **Erase** data ("right to be forgotten"), subject to legal retention obligations
- **Restrict** or **object** to certain processing
- **Data portability** — receive Your data in a machine-readable format
- **Withdraw consent** at any time, where processing is based on consent
- **Lodge a complaint** with the Danish Data Protection Authority (Datatilsynet, <https://www.datatilsynet.dk>)

To exercise any of these rights, contact <support@liftandcode.com>. We will respond within one month.

## 9. Security

We apply reasonable technical and organisational measures to protect personal data, including: encrypted transit (HTTPS / TLS), access controls on Lift & Code systems, and a documented incident-response process. No system is perfectly secure; in the unlikely event of a breach affecting Your personal data, we will notify You and the Danish Data Protection Authority as required by GDPR Art. 33–34.

## 10. Children

FileDrop Pro is a business tool not directed at children. We do not knowingly collect personal data from anyone under the age of 16.

## 11. Changes to this Privacy Statement

We may update this Privacy Statement from time to time. Material changes will be communicated through the FileDrop Pro AppSource listing and on this page. The "Last updated" date at the top of this page indicates when the current version took effect.

## 12. Contact

For any privacy-related question or to exercise Your rights:

**Lift & Code**
Email: <support@liftandcode.com>
Postal: Istedgade 105 2TV, 1650 Copenhagen V, Denmark
