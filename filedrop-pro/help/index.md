---
layout: page
title: FileDrop Pro — Help
description: How to install, set up, and use FileDrop Pro for Microsoft Dynamics 365 Business Central
permalink: /filedrop-pro/help/
---

This page covers installation, setup, and day-to-day use of FileDrop Pro.

## Install

1. Open Microsoft AppSource from inside Business Central (**Settings** → **Extension Marketplace**) or browse to <https://appsource.microsoft.com/>
2. Search for **FileDrop Pro**
3. Click **Get it now** and follow the install prompts
4. Wait for Business Central to finish installing the extension (usually less than a minute)

Once installed, FileDrop Pro is available in every company in your tenant, but the drag-and-drop factbox is *off* by default per area — see Setup.

## Setup

1. In Business Central, search (**Tell Me**) for **FileDrop Pro Setup** and open the page
2. Tick the areas you want to enable the drag-and-drop factbox on:
   - **Finance** — General Journal, Customer Ledger Entries, Vendor Ledger Entries, General Ledger Entries
   - **Purchase** — Purchase Order List, Purchase Invoices, Purchase Credit Memos, Posted Documents With No Inc. Doc.
   - **Sales** — Sales Invoice List, Sales Credit Memos
   - **Inventory** — Item Journal
3. *(Optional)* Click **Activate Drag and Drop in all companies** if you want to roll out the same setting to every company in the tenant in one go

The toggles take effect immediately — no restart needed. Open one of the host pages and the FileDrop Pro factbox will appear on the right-hand side.

## Day-to-day use

### Attach a file to a single record

1. Open any supported page (e.g. General Journal)
2. Place the cursor on the line you want to attach a file to
3. Drag a file from your desktop or file explorer onto the **FileDrop Pro** factbox on the right
4. FileDrop Pro creates an **Incoming Document** entry, stores the file as an **Incoming Document Attachment**, and links it to the journal line via *Incoming Document Entry No.*
5. A confirmation message appears: *"Import of 1 file finished."*

### Attach multiple files at once

Drop several files together onto the factbox. Each file becomes its own Incoming Document attachment linked to the current record.

### Attach a file to multiple records at once

1. Multi-select the records you want (Ctrl+Click or Shift+Click in the list)
2. Drop a single file onto the factbox
3. Every selected record gets linked to the same Incoming Document

### Document No. propagation on journals

When you drop a file onto a General Journal or Item Journal line, FileDrop Pro automatically links every *other* line in the journal that shares the same **Document No.** to the same Incoming Document. This is the common case where one invoice spans multiple G/L splits.

### Vendor Invoice No. propagation on purchase documents

When you drop a file onto a Purchase Order (or Purchase Invoice / Credit Memo), FileDrop Pro can optionally link the same file to every other purchase document that shares the same **Vendor Invoice No.** This is useful when the same scan supports multiple POs from the same vendor.

## Supported pages

| Area | Page | Multi-select | Doc.-No. propagation |
|---|---|---|---|
| Finance | General Journal | ✓ | ✓ |
| Finance | Customer Ledger Entries | ✓ | — |
| Finance | Vendor Ledger Entries | ✓ | — |
| Finance | General Ledger Entries | ✓ | — |
| Inventory | Item Journal | ✓ | ✓ |
| Purchase | Purchase Order List | ✓ | ✓ (Vendor Invoice No.) |
| Purchase | Purchase Invoices | ✓ | — |
| Purchase | Purchase Credit Memos | ✓ | — |
| Purchase | Posted Documents With No Inc. Doc. | ✓ | — |
| Sales | Sales Invoice List | ✓ | — |
| Sales | Sales Credit Memos | ✓ | — |

## Permissions

Users need the **D365 BUS PREMIUM** permission set (or equivalent) in addition to the FileDrop Pro permission set. This grants them write access to **Incoming Document** and **Incoming Document Attachment** — the standard Business Central tables FileDrop Pro writes into.

## Troubleshooting

**The factbox doesn't appear on a supported page.**
Check **FileDrop Pro Setup** — the area for that page must be ticked. Refresh the page (F5) after toggling.

**Dropping a file does nothing.**
Verify your browser allows file drag-and-drop and that your account has write permission to **Incoming Document** in the current company.

**Wrong record gets the attachment.**
The factbox attaches to the *currently selected* line. If you multi-selected and the cursor sat on a different line, the selection wins. Re-select carefully.

**File is rejected.**
Business Central's standard file-size limits apply to incoming documents. Very large files (typically > 30 MB) may be rejected by the platform.

## Support

For anything not covered here: <support@liftandcode.com>

When reporting an issue, please include:

- Business Central version (**Help** → **About**)
- The page you were on
- The browser you were using
- A brief description of what you did and what happened (a screenshot helps a lot)
