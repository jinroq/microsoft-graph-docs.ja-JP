---
title: networkIPv4ConfigurationManagementCondition リソースの種類
description: 構成ベースの管理条件を定義することも、デバイスが特定の IP を検出したときにトリガーとなる IPv4 ネットワークの設定です。 IP 構成の管理の条件だと考えてよい真のネットワーク接続がアクティブなときです。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 412f5de452e23eeb58f536655c4678526e996e07
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962108"
---
# <a name="networkipv4configurationmanagementcondition-resource-type"></a>networkIPv4ConfigurationManagementCondition リソースの種類

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでの、これらの API の使用はサポートされていません。

> **注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。

構成ベースの管理条件を定義することも、デバイスが特定の IP を検出したときにトリガーとなる IPv4 ネットワークの設定です。 IP 構成の管理の条件だと考えてよい真のネットワーク接続がアクティブなときです。

[NetworkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md)から継承します。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト networkIPv4ConfigurationManagementConditions](../api/intune-fencing-networkipv4configurationmanagementcondition-list.md)|[networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md)コレクション|[NetworkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md)オブジェクトのプロパティと関係を一覧表示します。|
|[NetworkIPv4ConfigurationManagementCondition を取得します。](../api/intune-fencing-networkipv4configurationmanagementcondition-get.md)|[networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md)|[NetworkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md)オブジェクトのプロパティと関係を参照してください。|
|[NetworkIPv4ConfigurationManagementCondition を作成します。](../api/intune-fencing-networkipv4configurationmanagementcondition-create.md)|[networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md)|新しい[networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md)オブジェクトを作成します。|
|[NetworkIPv4ConfigurationManagementCondition を削除します。](../api/intune-fencing-networkipv4configurationmanagementcondition-delete.md)|なし|の[networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md)を削除します。|
|[NetworkIPv4ConfigurationManagementCondition を更新します。](../api/intune-fencing-networkipv4configurationmanagementcondition-update.md)|[networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md)|[NetworkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
|:---|:---|:---|
|ID|String|管理条件の一意の識別子です。 システムでは、作成時に割り当てられた値が生成されます。 [ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。|
|一意な名前|String|管理条件の一意の名前です。 管理条件式で使用されます。 [ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。|
|displayName|String|管理者は、管理の条件の名前を定義します。 [ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。|
|説明|String|管理者は、管理状態の説明を定義します。 [ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。|
|createdDateTime|DateTimeOffset|管理条件が作成された時刻。 サービス側が生成されます。 [ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。|
|変更された日時|DateTimeOffset|管理条件が最後に修正された時間です。 サービス側を更新します。 [ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。|
|eTag|String|管理条件の ETag。 サービス側を更新します。 [ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。|
|applicablePlatforms|[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)コレクション|この管理条件に該当するプラットフォームです。 [ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。|
|ipV4Prefix|String|接続されている IPv4 サブネットです。 10.0.0.0/8 など|
|ipV4Gateway|String|ゲートウェイの IPv4 アドレス。 10.0.0.0 など|
|ipV4DHCPServer|String|アダプターの DHCP サーバーの IPv4 アドレスです。|
|ipV4DNSServerList|String コレクション|アダプターに対して構成されている IPv4 DNS サーバーです。|
|dnsSuffixList|String コレクション|現在のネットワークの有効な DNS サフィックスです。 例: seattle.contoso.com|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|managementConditionStatements|[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)コレクション|管理条件に関連付けられている管理の条件ステートメントです。 [ManagementCondition](../resources/intune-fencing-managementcondition.md)から継承されました。|

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





