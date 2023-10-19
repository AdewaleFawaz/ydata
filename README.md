# Importing Existing DNS Records with Terraform and Cloudflare

This guide explains how to import existing DNS records into Terraform when Terraform attempts to recreate resources that already exist in your Cloudflare account.

## Prerequisites

- [Terraform](https://www.terraform.io/downloads.html)
- A Cloudflare account
- Terraform Cloudflare provider correctly configured

## Importing DNS Records

When Terraform encounters an issue where it's trying to recreate existing resources, follow these steps to import the existing DNS records:

1. **Identify Existing DNS Records:**

   - Log in to your Cloudflare account.
   - Confirm the presence of the DNS records that Terraform is trying to manage.

2. **Retrieve Cloudflare Zone ID:**

   - Find the Cloudflare Zone ID for your domain in the Cloudflare dashboard.

3. **Import Existing DNS Records:**

   - Use the following `terraform import` commands to import the DNS records into Terraform, utilizing the "zoneID/recordID" format:

   ```bash
   terraform import module.nextresearch-mail-record.cloudflare_record.record ZONE_ID/DNS_RECORD_ID
   terraform import module.nextresearch-record.cloudflare_record.record ZONE_ID/DNS_RECORD_ID
   terraform import module.nextresearch-www-record.cloudflare_record.record ZONE_ID/DNS_RECORD_ID
