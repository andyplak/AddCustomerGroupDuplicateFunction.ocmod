# Customer Group Duplicate Function OCMOD

An OpenCart 3.x OCMOD that adds customer group duplication functionality to the admin panel.

## Features

- **Complete Duplication**: Copies all customer group settings and related data
- **One-Click Operation**: Simple duplicate button in the customer group list
- **Comprehensive Entity Copying**: Duplicates all associated records including:
  - Product discounts
  - Category discounts
  - Custom fields
  - Tax rates
  - Product restrictions (hierarchical)
  - Form associations (TMD)
  - Shipping settings

## Installation

1. Download the `install.xml` file
2. Upload via OpenCart Admin → Extensions → Extension Installer
3. Go to Extensions → Modifications and click "Refresh"
4. Navigate to Customers → Customer Groups to see the duplicate functionality

## Usage

1. Go to **Customers → Customer Groups** in your admin panel
2. Find the customer group you want to duplicate
3. Click the **Duplicate** button (blue copy icon) next to the Edit button
4. The system will create a copy with "(Copy)" appended to the name
5. Edit the duplicated group as needed

## What Gets Duplicated

### Core Settings
- Customer group name (with "(Copy)" suffix)
- Description
- Approval requirements
- Sort order
- Parent group relationship (if using hierarchy)

### Associated Data
- **Product Discounts**: All product-specific pricing rules
- **Category Discounts**: Percentage-based category discounts
- **Custom Fields**: Required and optional custom field associations
- **Tax Rates**: Tax rate assignments for the group
- **Product Restrictions**: Category restrictions with inheritance settings
- **TMD Forms**: Associated form access permissions
- **Shipping Rules**: Multi-flat shipping rate configurations

## Product Restrictions Support

This OCMOD includes support for the product restrictions system, duplicating:
- Restricted product categories
- Inheritance settings (`apply_to_children`)
- Hierarchical restriction rules

## Compatibility

- **OpenCart Version**: 3.x
- **Dependencies**: None (standalone OCMOD)
- **Conflicts**: Should not conflict with other extensions

## Version History

- **v1.2**: Added product restrictions duplication support
- **v1.1**: Initial release with core duplication functionality

## Support

For issues or feature requests, please visit the [GitHub repository](https://github.com/andyplak/AddCustomerGroupDuplicateFunction.ocmod).

