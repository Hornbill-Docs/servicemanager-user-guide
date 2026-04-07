---
layout: article-toc
---
# Asset management overview

Use asset management to capture and detail information for your organization's assets. This process includes tracking ownership, costs, relationships, and the life cycle of assets to support strategic decision-making for your IT environment.

Hornbill Service Manager Asset Management records hardware and software inventory information. This data helps IT teams support asset users and make informed decisions about hardware and software purchases and redistribution.

Assets form the foundation of a Configuration Management Database (CMDB). You can use assets within Incident, Problem, and Change processes to assist with incident classification, impact analysis, and change planning.

<!-- [Visual Suggestion: A diagram showing how assets connect to Incident, Problem, and Change records to form a CMDB.] -->

## Access requirements

To use the Asset Management capabilities in Hornbill Service Manager, your user account must have one of the following roles.

| Role | Description |
| :--- | :--- |
| Asset Management User | Provides rights to define and edit assets and add detailed asset information. |
| Asset Management Admin | Provides all capabilities of the Asset Management User role and adds rights to access asset configuration where asset types, categories, partitions, custom fields, and other settings can be managed. |

## Key features

* **Manage assets**: Access and update your organization's assets in one central location.
* **Bulk update assets**: Update a field across multiple assets simultaneously.
* **Assets under warranty**: View assets based on their warranty status.

## Integration options

If you use an asset-discovery tool or a separate asset database, you can set up automated imports and updates. Use the [Hornbill Asset Import utility](/data-imports-guide/assets/overview) to connect to a local database within your network and move information to your Hornbill instance.

<!--
Database Asset Import

:::note
If Assets are added using data::entityAddRecord API, the Asset URN must be set against each individual Asset record. This can be achieved using data::entityUpdateRecord API. Please remember to replace [Asset Id] with the generated value in h_pk_asset_id column in h_cmdb_assets table.

 <params>
   <application>com.hornbill.servicemanager</application>
   <entity>Asset</entity>
   <primaryEntityData>
     <record>
       <h_pk_asset_id>[Asset Id]</h_pk_asset_id>
       <h_asset_urn>urn:sys:entity:com.hornbill.servicemanager:Asset:" + [Asset Id]</h_asset_urn>
     </record>
   </primaryEntityData>
 </params>

 :::
 -->