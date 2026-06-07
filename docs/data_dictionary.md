# Data Dictionary

## Source Dataset

Current development source:

`data/raw/MSD Projects Sheet 2025.xlsx`

Future production source:

`Google Sheets → PostgreSQL → Superset`

## Column Definitions

| Raw Column | Clean Column Name | Category | Description |
|---|---|---|---|
| Sr | project_sr | Project | Unique project serial number from the source sheet |
| Projects | project_name | Project | Name/title of the project or customer engagement |
| Project Sector | project_sector | Customer/Market | Sector or industry of the customer |
| Description | project_description | Project | Description of solution, service, or requirement |
| Requirement Type | requirement_type | Sales | Lead/commercial source such as own lead, tender, RFQ/RFP |
| Preffered Partner | preferred_partner | Partner | Preferred partner/vendor, spelling corrected in clean layer |
| Progress Status | progress_status | Operations | Current project status |
| Dollar Rate ($) | dollar_rate | Finance | Exchange rate used for costing or pricing |
| Landing Factor for DDP | landing_factor_ddp | Finance | Cost factor used for DDP/import calculations |
| Revenue | revenue | Finance | Customer-facing project value |
| NTL Cost | ntl_cost | Finance | Internal Nayatel cost for the project |
| Profit | profit | Finance | Revenue minus NTL cost |
| Margin (%) | markup_pct_raw | Finance | Existing sheet margin; likely markup, not true gross margin |
| Sales Person | salesperson_name | Sales | Commercial owner of the project |
| Project Engineer | engineer_name | Operations | Delivery/technical owner |
| BOQ in Progress Date | boq_in_progress_date | Timeline | Date when BOQ work started |
| Approval in Process Date | approval_in_process_date | Timeline | Date when approval process started |
| Work in Progress Date | work_in_progress_date | Timeline | Date when delivery/work started |
| Halt Date | halt_date | Timeline | Date when project was halted/closed/stalled |
| Project Completion Date | completion_date | Timeline | Date when project was completed |
| Expected Man Hours | expected_man_hours | Effort | Planned effort hours |
| Actual Man Hours (After Project Completion) | actual_man_hours | Effort | Actual effort captured after completion |
| Mode of Payment | payment_mode | Finance | Customer payment terms/mode |
| Special Discounts (Amount) | special_discount_amount | Finance | Discount amount applied to project |
| Project Timeline Provided to Customer (Weeks) | timeline_committed_weeks | Timeline | Timeline committed to customer |
| Project Completion Timeline (Weeks) | completion_timeline_weeks | Timeline | Actual or recorded completion timeline |
| Passive Work | passive_work | Delivery | Whether passive work is involved |
| Equipment Provided | equipment_provided | Delivery | Equipment or solution provided |
| OEM 1 | oem_1 | Vendor | First OEM/manufacturer |
| Distributor 1 | distributor_1 | Vendor | First distributor |
| Distributor 1 (NTL Cost) | distributor_1_ntl_cost | Vendor/Finance | Cost from first distributor |
| OEM 2 | oem_2 | Vendor | Second OEM/manufacturer |
| Distributor 2 | distributor_2 | Vendor | Second distributor |
| Distributor 2 (NTL Cost) | distributor_2_ntl_cost | Vendor/Finance | Cost from second distributor |
| OEM 3 | oem_3 | Vendor | Third OEM/manufacturer |
| Distributor 3 | distributor_3 | Vendor | Third distributor |
| Distributor 3 (NTL Cost) | distributor_3_ntl_cost | Vendor/Finance | Cost from third distributor |
