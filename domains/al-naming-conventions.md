---
topic_id: company-naming-conventions
title: Company AL Naming Conventions
category: standards
bc_version: "14.0+"
priority: high
tags: [naming, standards, conventions]
---

# Company AL Naming Conventions

## Language
Always use English as the naming language.

## Casing
Always use CamelCase when naming object.

## General naming
- Naming of files, objects, procedures etc. should be descriptive, precise and intuitive.
- Names should be easy for a developer to understand without too many abbreviation.

## File naming
- All .al filenames should be prefixed with `OSB` without any `_` or whitespaces.
- For example `OSBSalesHeaderTemplate.Table.al`.

## Object naming
- Objects should have the same name as the file they are in.
- All objects should be prefixed with `OBS_` including an underscore. For example Object `OSB_SalesHeaderTemplate` is written in the file `OSBSalesHeaderTemplate.Table.al`.
- Objects shall never have any whitespaces in their name.

## Field naming
- Fields that are extenting existing AL Objects such as a `TableExtension` or `PageExtension` should always have `OSB_` as a prefix.
Example:
```
tableExtension 50000 OSB_ItemLedgerEntry extends "Item Ledger Entry"
{
  field(50000; OSB_Ext1_EntryNo; Integer)
  {
  }
}
```
- Fields that are within a new OSB AL Object have no prefix.
Example:
```
table 50000 OSB_MyTable
{
  field(10; EntryNo; Integer)
  {
  }
}
```
