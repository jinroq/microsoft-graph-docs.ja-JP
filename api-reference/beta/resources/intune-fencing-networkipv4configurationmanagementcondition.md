---
title: networkIPv4ConfigurationManagementCondition リソースの種類
description: デバイスが特定の IP ネットワーク設定を検出したときにトリガーされる IPv4 構成ベースの管理条件が定義されている場合があります。 IP 構成管理条件は、ネットワーク接続がアクティブな場合にのみ TRUE と見なされます。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2ace9a053b82118ff5e6bfdb3a14c628a5c488af
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30150478"
---
# <a name="networkipv4configurationmanagementcondition-resource-type"></a>networkIPv4ConfigurationManagementCondition リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

デバイスが特定の IP ネットワーク設定を検出したときにトリガーされる IPv4 構成ベースの管理条件が定義されている場合があります。 IP 構成管理条件は、ネットワーク接続がアクティブな場合にのみ TRUE と見なされます。


[networkmanagementcondition](../resources/intune-fencing-networkmanagementcondition.md)から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト networkIPv4ConfigurationManagementConditions](../api/intune-fencing-networkipv4configurationmanagementcondition-list.md)|[networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md)コレクション|[networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[networkIPv4ConfigurationManagementCondition を取得する](../api/intune-fencing-networkipv4configurationmanagementcondition-get.md)|[networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md)|[networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[networkIPv4ConfigurationManagementCondition を作成する](../api/intune-fencing-networkipv4configurationmanagementcondition-create.md)|[networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md)|新しい[networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md)オブジェクトを作成します。|
|[networkIPv4ConfigurationManagementCondition の削除](../api/intune-fencing-networkipv4configurationmanagementcondition-delete.md)|なし|[networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md)を削除します。|
|[networkIPv4ConfigurationManagementCondition の更新](../api/intune-fencing-networkipv4configurationmanagementcondition-update.md)|[networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md)|[networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列|管理条件の一意識別子。 作成時に割り当てられたシステム生成値。 [managementcondition](../resources/intune-fencing-managementcondition.md)から継承します|
|uniqueName|String|管理条件の一意の名前。 管理条件式で使用されます。 [managementcondition](../resources/intune-fencing-managementcondition.md)から継承します|
|displayName|String|管理条件の管理者定義の名前。 [managementcondition](../resources/intune-fencing-managementcondition.md)から継承します|
|説明|String|管理条件の管理者定義の説明。 [managementcondition](../resources/intune-fencing-managementcondition.md)から継承します|
|createdDateTime|DateTimeOffset|管理条件が作成された時刻。 サービス側を生成しました。 [managementcondition](../resources/intune-fencing-managementcondition.md)から継承します|
|変更された日時|DateTimeOffset|管理条件が最後に変更された時刻。 サービス側を更新しました。 [managementcondition](../resources/intune-fencing-managementcondition.md)から継承します|
|eTag|String|管理条件の ETag。 サービス側を更新しました。 [managementcondition](../resources/intune-fencing-managementcondition.md)から継承します|
|アプリケーションのプラットフォーム|[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)コレクション|この管理条件の適用可能なプラットフォーム。 [managementcondition](../resources/intune-fencing-managementcondition.md)から継承します|
|ipV4Prefix|String|接続先の IPv4 サブネット。 例: 10.0.0.0/8|
|ipV4Gateway|String|IPv4 ゲートウェイアドレス。 例: 10.0.0.0|
|ipV4DHCPServer|String|アダプターの DHCP サーバーの IPv4 アドレス。|
|ipV4DNSServerList|String コレクション|アダプターに対して構成されている IPv4 DNS サーバー。|
|dnsSuffixList|String コレクション|現在のネットワークの有効な DNS サフィックス。 例: seattle.contoso.com|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|managementconditionstatements|[managementconditionstatement](../resources/intune-fencing-managementconditionstatement.md)コレクション|管理条件に関連付けられている管理条件ステートメント。 [managementcondition](../resources/intune-fencing-managementcondition.md)から継承します|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.networkIPv4ConfigurationManagementCondition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.networkIPv4ConfigurationManagementCondition",
  "id": "String (identifier)",
  "uniqueName": "String",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "modifiedDateTime": "String (timestamp)",
  "eTag": "String",
  "applicablePlatforms": [
    "String"
  ],
  "ipV4Prefix": "String",
  "ipV4Gateway": "String",
  "ipV4DHCPServer": "String",
  "ipV4DNSServerList": [
    "String"
  ],
  "dnsSuffixList": [
    "String"
  ]
}
```




