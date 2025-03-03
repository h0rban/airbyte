# Zoho Billing
Zoho Billing is a billing software used by countless organizations across the globe.
Using this connector we can extract data from various streams such as products , invoices , transactions and quotes.
Docs : https://www.zoho.com/billing/api/v1/introduction/#overview

## Configuration

| Input | Type | Description | Default Value |
|-------|------|-------------|---------------|
| `region` | `string` | Region.  |  |
| `client_id` | `string` | OAuth Client ID.  |  |
| `client_secret` | `string` | OAuth Client Secret.  |  |
| `refresh_token` | `string` | OAuth Refresh Token.  |  |

## Streams
| Stream Name | Primary Key | Pagination | Supports Full Sync | Supports Incremental |
|-------------|-------------|------------|---------------------|----------------------|
| Products | product_id | DefaultPaginator | ✅ |  ❌  |
| plans | plan_code | DefaultPaginator | ✅ |  ❌  |
| addons | addon_code | DefaultPaginator | ✅ |  ❌  |
| coupons | coupon_code | DefaultPaginator | ✅ |  ❌  |
| customers | customer_id | DefaultPaginator | ✅ |  ❌  |
| Quotes | estimate_id | DefaultPaginator | ✅ |  ❌  |
| invoices | invoice_id | DefaultPaginator | ✅ |  ❌  |
| expenses | expense_id | DefaultPaginator | ✅ |  ❌  |
| subscriptions | customer_id | DefaultPaginator | ✅ |  ❌  |
| taxes | tax_id | DefaultPaginator | ✅ |  ❌  |
| transactions | transaction_id | DefaultPaginator | ✅ |  ❌  |
| recurring expenses | recurring_expense_id | DefaultPaginator | ✅ |  ❌  |

## Changelog

<details>
  <summary>Expand to review</summary>

| Version          | Date              | Pull Request | Subject        |
|------------------|-------------------|--------------|----------------|
| 0.0.5 | 2025-01-11 | [51468](https://github.com/airbytehq/airbyte/pull/51468) | Update dependencies |
| 0.0.4 | 2024-12-28 | [50836](https://github.com/airbytehq/airbyte/pull/50836) | Update dependencies |
| 0.0.3 | 2024-12-21 | [50392](https://github.com/airbytehq/airbyte/pull/50392) | Update dependencies |
| 0.0.2 | 2024-12-14 | [49451](https://github.com/airbytehq/airbyte/pull/49451) | Update dependencies |
| 0.0.1 | 2024-11-05 | | Initial release by [@ombhardwajj](https://github.com/ombhardwajj) via Connector Builder |

</details>
