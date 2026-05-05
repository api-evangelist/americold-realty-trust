# Americold Realty Trust (americold-realty-trust)

Americold Realty Trust is a global leader in temperature-controlled logistics, real estate, and value-added services, owning and operating one of the largest networks of cold storage warehouses in the world. The company serves food producers, retailers, and distributors with integrated logistics solutions, offering technology platforms such as i-3PL for customer-facing inventory and order visibility and EDI for system-to-system supply chain integration. While Americold provides customer-facing technology and integration capabilities, it does not currently publish a public developer-facing API portal with open OpenAPI documentation; integrations are established project-by-project through the Americold service desk and EDI onboarding process. Fortune 2024 (rank 955).

**URL:** [Visit APIs.json](https://raw.githubusercontent.com/api-evangelist/americold-realty-trust/refs/heads/main/apis.yml)

## Tags:

 - Cold Storage, Logistics, Supply Chain, Warehousing, Real Estate, Temperature-Controlled, Cold Chain, EDI, 3PL

## Timestamps

- **Created:** 2026-05-04
- **Modified:** 2026-05-05

## APIs

### Americold i-3PL Platform
i-3PL is Americold's customer-facing digital supply chain platform offering real-time inventory tracking, order management, dock appointment scheduling, customizable alerts, and 40+ reporting tools across the Americold network. The platform supports integration with customer ERP systems for seamless data exchange but does not publish open public API documentation; programmatic integration is coordinated with the Americold Service Desk.

**Human URL:** [https://www.americold.com/technology-automation/i-3pl/](https://www.americold.com/technology-automation/i-3pl/)

#### Tags:

 - Logistics, Supply Chain, Cold Storage, 3PL, Inventory, Reporting

#### Properties

- [Portal](https://www.i-3pl.com/login)
- [Documentation](https://www.americold.com/technology-automation/i-3pl/)
- [Support](https://www.americold.com/contact-us/)
- [i-3PL Inventory Snapshot Schema](json-schema/americold-i-3pl-inventory-snapshot-schema.json)
- [i-3PL Inventory Snapshot Structure](json-structure/americold-i-3pl-inventory-snapshot-structure.json)
- [i-3PL Inventory Snapshot Example](examples/americold-i-3pl-inventory-snapshot-example.json)

### Americold EDI
Americold provides Electronic Data Interchange (EDI) capabilities for automated data exchange between Americold and depositor (customer) systems, supporting orders, inventory, shipments, and other supply chain transactions. The integration uses the X12 warehousing 900-series transaction sets common across third-party logistics providers (940, 943, 944, 945, 947, 856, 846).

**Human URL:** [https://www.americold.com/technology-automation/edi-electronic-data-interchange/](https://www.americold.com/technology-automation/edi-electronic-data-interchange/)

#### Tags:

 - EDI, Integration, Supply Chain, X12, 3PL, AS2

#### Properties

- [Documentation](https://www.americold.com/technology-automation/edi-electronic-data-interchange/)
- [Support](https://www.americold.com/contact-us/)
- [EDI Warehouse Shipping Order (940) Schema](json-schema/americold-edi-warehouse-shipping-order-schema.json)
- [EDI Warehouse Shipping Advice (945) Schema](json-schema/americold-edi-warehouse-shipping-advice-schema.json)
- [EDI Warehouse Shipping Order (940) Structure](json-structure/americold-edi-warehouse-shipping-order-structure.json)
- [EDI Warehouse Shipping Advice (945) Structure](json-structure/americold-edi-warehouse-shipping-advice-structure.json)
- [EDI Warehouse Shipping Order (940) Example](examples/americold-edi-warehouse-shipping-order-example.json)
- [EDI Warehouse Shipping Advice (945) Example](examples/americold-edi-warehouse-shipping-advice-example.json)

## Common Properties

- [Website](https://www.americold.com)
- [Portal](https://www.i-3pl.com/login)
- [Technology & Automation](https://www.americold.com/technology-automation/)
- [Customer Resources](https://www.americold.com/customer-resources/)
- [Contact](https://www.americold.com/contact-us/)
- [Careers](https://www.americold.com/careers/)
- [Investor Relations](https://ir.americold.com)
- [Privacy Policy](https://www.americold.com/privacy-policy/)
- [Terms of Service](https://www.americold.com/terms-of-use/)
- [Americold Realty Trust JSON-LD Context](json-ld/americold-realty-trust-context.jsonld)
- [Americold Realty Trust Vocabulary](vocabulary/americold-realty-trust-vocabulary.yaml)

## Features

| Name | Description |
|------|-------------|
| Global Cold Storage Network | Americold owns and operates one of the largest networks of temperature-controlled warehouses worldwide, with facilities across North America, Europe, Australia, New Zealand, and South America serving food producers, processors, distributors, and retailers. |
| i-3PL Customer Platform | Customer-facing digital platform delivering real-time inventory tracking, order management, dock appointment scheduling, customizable alerts, and over 40 reporting tools across the Americold network from phone, tablet, or desktop. |
| EDI Supply Chain Integration | Standards-based X12 EDI exchange of warehousing transactions (940/943/944/945/947) and shipping/inventory transactions (856, 846) between Americold's WMS/TMS/LMS/WES and depositor ERP systems for real-time supply chain visibility. |
| Lot-Level Traceability | Item-lot granularity for receipts, holds, releases, and shipments enables food-safety traceability, recall readiness, and FSMA / HACCP compliance across the cold chain. |
| Multi-Temperature Zones | Storage and handling across deep-frozen, frozen, refrigerated, cooler, and ambient temperature zones with documented temperature requirements and load-temperature recording on outbound shipments. |
| Value-Added Services | Blast freezing, pick and pack, labeling and relabeling, repacking, kitting, staging, cross-dock, sloughing/tempering, plus light assembly and food processing services provided alongside storage. |

## Use Cases

| Name | Description |
|------|-------------|
| Cold Chain Outbound Fulfillment | A depositor sends a 940 Warehouse Shipping Order to an Americold facility; Americold picks, stages, and ships product; a 945 Warehouse Shipping Advice returns to the depositor for ERP reconciliation. |
| Inventory Visibility for Food Manufacturers | Frozen and refrigerated food manufacturers monitor on-hand, available, committed, and held inventory across Americold facilities using i-3PL snapshots, dashboards, and reports. |
| Dock Appointment Scheduling | Carriers and depositor logistics teams book, modify, and cancel dock appointments at Americold facilities through i-3PL to optimize throughput and reduce dwell time. |
| Lot Traceability and Recall | Quality assurance and food safety teams trace a lot from receipt through every shipment to support recalls and regulatory holds. |
| Stock Transfer Between Facilities | Move inventory between Americold facilities using 943/944 transfer transactions to balance network inventory and meet regional demand. |
| ERP-to-WMS Integration | Connect SAP, Oracle, NetSuite, Microsoft Dynamics, and other ERP systems to Americold's WMS through EDI and managed integration partners. |

## Integrations

| Name | Description |
|------|-------------|
| SPS Commerce | SPS Commerce provides pre-built EDI connections used by depositors and 3PL trading partners to exchange warehousing transaction sets with Americold over a managed network. |
| Stedi | Stedi's API-first EDI platform is used by modern engineering teams to translate, validate, and exchange X12 warehouse transactions with Americold programmatically. |
| Cleo Integration Cloud | Cleo provides AS2, SFTP, and API integration tooling commonly used to connect depositor ERP systems to 3PL warehouse partners like Americold. |
| SAP and Oracle ERP | Americold integrates with leading enterprise ERP systems via EDI for orders, inventory, and shipping reconciliation across the depositor's order-to-cash and procure-to-pay processes. |
| Customer ERP Systems | Americold can integrate its supply chain management systems (WMS, LMS, TMS, WES) with a customer's ERP system for seamless information flow. |

## Artifacts

Machine-readable specifications organized by format. Note: Americold does not publish a public OpenAPI specification; the artifacts below model the EDI and i-3PL data domain that customers integrate with.

### JSON Schema

- [EDI Warehouse Shipping Order (940) Schema](json-schema/americold-edi-warehouse-shipping-order-schema.json)
- [EDI Warehouse Shipping Advice (945) Schema](json-schema/americold-edi-warehouse-shipping-advice-schema.json)
- [i-3PL Inventory Snapshot Schema](json-schema/americold-i-3pl-inventory-snapshot-schema.json)

### JSON Structure

- [EDI Warehouse Shipping Order (940) Structure](json-structure/americold-edi-warehouse-shipping-order-structure.json)
- [EDI Warehouse Shipping Advice (945) Structure](json-structure/americold-edi-warehouse-shipping-advice-structure.json)
- [i-3PL Inventory Snapshot Structure](json-structure/americold-i-3pl-inventory-snapshot-structure.json)

### JSON-LD

- [Americold Realty Trust Context](json-ld/americold-realty-trust-context.jsonld)

### Examples

- [EDI Warehouse Shipping Order (940) Example](examples/americold-edi-warehouse-shipping-order-example.json)
- [EDI Warehouse Shipping Advice (945) Example](examples/americold-edi-warehouse-shipping-advice-example.json)
- [i-3PL Inventory Snapshot Example](examples/americold-i-3pl-inventory-snapshot-example.json)

## Vocabulary

- [Americold Realty Trust Vocabulary](vocabulary/americold-realty-trust-vocabulary.yaml) — Unified taxonomy mapping 11 resources, 9 actions, 5 workflows, and 9 personas across Americold's cold-chain logistics, EDI integration, and i-3PL platform landscape.

## Maintainers

**FN:** API Evangelist

**URL:** [https://apievangelist.com](https://apievangelist.com)
