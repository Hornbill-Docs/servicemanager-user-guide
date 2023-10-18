---
layout: article-toc
---
# Asset Management
Asset Management involves the capturing and detailing of information for the assets within your Organization. This includes tracking the ownership, costs, relationships, and life cycle of assets to support the strategic decision making for the IT environment.

Asset Management facilitates the recording of detailed hardware and software inventory information which can be used to assist IT with supporting the users of the assets and for making decisions about hardware and software purchases and redistribution.

The Assets in the Asset Management forms the foundation of a Configuration Management Database (CMDB). Assets can be used as part of Incident, Problem, and Change processes to assist in incident classification, impact analysts and change planning.

## Access
To access the Asset Management capability of Hornbill Service Manager, your User Account must have one of the following roles associated.

|Role|Description|
|-|-|
|Asset Management User|This role is for an Asset Management User. It includes rights to define new and edit individual Assets as well as being able to add detailed Asset information.|
|Asset Management Admin|This role is for an Asset Management Administrator and as well as providing all the capability of the Asset Management User role, it includes additional rights to define new and edit existing Asset Types.|

## Features
* **Manage Assets**<br>Access to your organization's assets
* **Manage Asset Types**<br>Define the types of assets that are used by your organization. Control the available fields and information used on each asset type.
* **Upload Assets**<br>For small batch imports of assets, use our simple CSV import.
* **Asset Tags**<br>Create and managed tags that can be used on individual assets. This includes an option to enable or disable the ability for a user to add their own tags, or force them to use a defined set of tags.

## Integration
If you already have an asset discovery tool or a second asset database, Hornbill gives you the ability to set up automated imports and updates using the Hornbill Asset Import Tool. The Hornbill Database Asset Import lets you connect to local database within your network and push the information up to your Hornbill instance.

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