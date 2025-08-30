# Rollback Procedure — Website Hosting (Netlify)

**Owner:** Rachel (PM)  
**Doer:** Steve (Cloud)  

## Steps

1. **Netlify Console:**
   - Go to **Deploys** tab for the `securepath.uk` site.
   - Identify the last known good deploy.
   - Click **Rollback to this deploy**.

2. **Verify Rollback:**
   - Open `https://securepath.uk` in browser.
   - Confirm site content matches previous version.

3. **DNS Fallback (if Netlify issue persists):**
   - Log into domain registrar for `securepath.uk`.
   - Update DNS A/CNAME to point back to fallback provider (document reference: DNS_Fallback_Config.md).
   - Propagation check: use `dig securepath.uk` or online DNS checker.

4. **Record Keeping:**
   - Document rollback in Governance Log (date, reason, version).
   - Notify Rachel (PM) + Michelle (CEO).

---

## Test Condition
- A dummy deploy rollback was performed successfully before go-live.
- Evidence stored in Evidence Vault.
