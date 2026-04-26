# Privacy Policy for NSW Property Insight

**Last Updated: April 2026**

This Privacy Policy explains how NSW Property Insight ("the Extension") handles information when you use it to research Sydney property market data. Our goal is to be fully transparent about what we collect, why, and for how long.

---

## 1. What We Collect and Why

When you click **Analyze Market Match**, the following data is sent to and stored on our secure backend (hosted on Render):

| Data field | Stored? | Why |
|---|---|---|
| **Full property address** | Yes | To look up suburb-level historical price benchmarks and calculate the Market Match Index. The full address is retained so that repeated queries for the same property can be deduplicated and suburb-level demand trends can be built accurately |
| **Suburb** (extracted from address) | Yes | To power suburb-level demand heat maps |
| **Budget** | Yes | To compare your target price against comparable suburb sales |
| **Bedrooms** *(optional)* | Yes, if provided | Helps select the right apartment price cluster for units and contributes to anonymised apartment-type tagging in future suburb reports |
| **Hashed session ID** | Yes | Your device-generated UUID is **one-way hashed** (SHA-256) before being stored. It is used solely to enforce the 5 free checks per day limit. The hash cannot be reversed to identify you |
| **Timestamp** | Yes | To support 6-month data retention and time-series trend analysis |

---

## 2. Data Aggregation & Suburb Demand Heat Maps

Search records are aggregated across all users to produce suburb-level demand heat maps showing which Sydney suburbs are receiving research interest in real time.

- Individual records are **never published or shared**. Only aggregated, suburb-level counts are surfaced in trend analysis.
- The hashed session ID cannot be linked to any personal profile and is never used outside of daily usage counting.
- Bedrooms input, where provided, is used to improve apartment-level price cluster accuracy in aggregate reporting only.

---

## 3. What We Do Not Collect

We do **not** collect, store, or have access to:

- Your name, email address, or any personally identifying information
- Your IP address (it is not logged or stored by our backend)
- Financial records, credit scores, bank details, or legal documents
- Browser history or activity on any website other than this Extension's popup
- Any data when you are not actively using the Extension

---

## 4. Data Retention

Stored search records (full address, suburb, bedrooms, budget, hashed session ID, and timestamp) are retained for **6 months** to maintain the relevance of market trend data, after which they are deleted from our systems.

Calculated results such as the Market Match Index score, market sentiment, and clearance rate are never persisted — they are computed fresh on each request and exist only in your browser session.

Your local usage counter (`chrome.storage.local`) remains only on your device and is never synced to our servers.

---

## 5. Local Storage

The Extension stores the following data locally on your device only:

| Stored value | Purpose |
|---|---|
| **Anonymous session ID** | Randomly generated UUID used to count your daily free checks. Transmitted to the backend as a one-way hash only |
| **Daily usage counter** | Number of checks used today |

Neither value is used to identify you personally.

---

## 6. Third-Party Services

We use the following services solely to provide the Extension's analytical functions:

| Service | Purpose |
|---|---|
| **Render** | Backend API hosting |
| **Supabase** | Property database storage |
| **Google Places API** *(via our backend proxy)* | Address autocomplete. Your address input passes through our backend — the API key is never exposed to the browser |

---

## 7. Contact & Support

If you have questions about this policy, please contact us through the Chrome Web Store support link.

---

*Disclaimer: This tool is for educational and research purposes only and does not constitute financial, legal, or real estate advice.*
