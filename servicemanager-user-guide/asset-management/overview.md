---
layout: article-toc
---
# Asset Management
Asset management involves the capturing and detailing of information for the assets within your organization. This includes tracking the ownership, costs, relationships, and life cycle of assets to support strategic decision-making for the IT environment.

Hornbill Service Manager Asset Management facilitates the recording of detailed hardware and software inventory information that can be used to assist IT with supporting the users of the assets and for making decisions about hardware and software purchases and redistribution.

The assets in Asset Management form the foundation of a Configuration Management Database (CMDB). Assets can be used as part of Incident, Problem, and Change processes to assist in incident classification, impact analysis, and change planning.

## Access
To access the Asset Management capabilities of Hornbill Service Manager, your user account must have one of the following roles associated.

|Role|Description|
|-|-|
|Asset Management User|This role includes rights to define  and edit assets as well as to add detailed asset information.|
|Asset Management Admin|This role provides all the capabilities of the Asset Management User role, with additional rights to define and edit asset types.|

## Features
* **Manage Assets.** Access to your organization's assets
* **Manage Asset Types.** Define the types of assets that are used by your organization. Control the available fields and information used on each asset type.
* **Upload Assets.** For small batch imports of assets, use our simple CSV import.
* **Asset Tags.** Create and managed tags that can be used on individual assets. This includes an option to enable or disable the ability for a user to add their own tags, or force them to use a defined set of tags.

## Integration
If you already have an asset-discovery tool or a second asset database, you can set up automated imports and updates using the [Hornbill Asset Import utility](/data-imports-guide/assets/overview). This utility lets you connect to a local database within your network and push the information up to your Hornbill instance.

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