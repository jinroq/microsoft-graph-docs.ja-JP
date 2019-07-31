---
title: networkIPv6ConfigurationManagementCondition リソースの種類
description: デバイスが特定の IP ネットワーク設定を検出したときにトリガーされる IPv6 構成ベースの管理条件が定義されている場合があります。 IP 構成管理条件は、ネットワーク接続がアクティブな場合にのみ TRUE と見なされます。 IPv6 DHCP サーバーのアドレスが一致しない可能性があります。 これは、Windows (circa Redstone) がこの情報を自然な認証サービスに公開しないためです。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: fead4345c94e9a48682b6d9584ba9897e1ad78e9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35998696"
---
# <a name="networkipv6configurationmanagementcondition-resource-type"></a>networkIPv6ConfigurationManagementCondition リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

デバイスが特定の IP ネットワーク設定を検出したときにトリガーされる IPv6 構成ベースの管理条件が定義されている場合があります。 IP 構成管理条件は、ネットワーク接続がアクティブな場合にのみ TRUE と見なされます。
IPv6 DHCP サーバーのアドレスが一致しない可能性があります。 これは、Windows (circa Redstone) がこの情報を自然な認証サービスに公開しないためです。


[Networkmanagementcondition](../resources/intune-fencing-networkmanagementcondition.md)から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト networkIPv6ConfigurationManagementConditions](../api/intune-fencing-networkipv6configurationmanagementcondition-list.md)|[networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md)コレクション|[NetworkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[NetworkIPv6ConfigurationManagementCondition を取得する](../api/intune-fencing-networkipv6configurationmanagementcondition-get.md)|[networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md)|[NetworkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[NetworkIPv6ConfigurationManagementCondition を作成する](../api/intune-fencing-networkipv6configurationmanagementcondition-create.md)|[networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md)|新しい[networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md)オブジェクトを作成します。|
|[NetworkIPv6ConfigurationManagementCondition の削除](../api/intune-fencing-networkipv6configurationmanagementcondition-delete.md)|None|[NetworkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md)を削除します。|
|[NetworkIPv6ConfigurationManagementCondition の更新](../api/intune-fencing-networkipv6configurationmanagementcondition-update.md)|[networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md)|[NetworkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列|管理条件の一意識別子。 作成時に割り当てられたシステム生成値。 [Managementcondition](../resources/intune-fencing-managementcondition.md)から継承します|
|uniqueName|String|管理条件の一意の名前。 管理条件式で使用されます。 [Managementcondition](../resources/intune-fencing-managementcondition.md)から継承します|
|displayName|String|管理条件の管理者定義の名前。 [Managementcondition](../resources/intune-fencing-managementcondition.md)から継承します|
|description|String|管理条件の管理者定義の説明。 [Managementcondition](../resources/intune-fencing-managementcondition.md)から継承します|
|createdDateTime|DateTimeOffset|管理条件が作成された時刻。 サービス側を生成しました。 [Managementcondition](../resources/intune-fencing-managementcondition.md)から継承します|
|modifiedDateTime|DateTimeOffset|管理条件が最後に変更された時刻。 サービス側を更新しました。 [Managementcondition](../resources/intune-fencing-managementcondition.md)から継承します|
|eTag|String|管理条件の ETag。 サービス側を更新しました。 [Managementcondition](../resources/intune-fencing-managementcondition.md)から継承します|
|アプリケーションのプラットフォーム|[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)コレクション|この管理条件の適用可能なプラットフォーム。 [Managementcondition](../resources/intune-fencing-managementcondition.md)から継承します|
|ipV6Prefix|String|接続先の IPv6 サブネット。 例: 2001 年: db8::/32|
|ipV6Gateway|String|IPv6 ゲートウェイアドレス。 例: 2001 年: db8:: 1|
|ipV6DNSServerList|文字列コレクション|アダプターに対して構成された IPv6 DNS サーバー。|
|dnsSuffixList|文字列コレクション|現在のネットワークの有効な DNS サフィックス。 例: seattle.contoso.com|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|managementConditionStatements|[Managementconditionstatement](../resources/intune-fencing-managementconditionstatement.md)コレクション|管理条件に関連付けられている管理条件ステートメント。 [Managementcondition](../resources/intune-fencing-managementcondition.md)から継承します|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.networkIPv6ConfigurationManagementCondition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.networkIPv6ConfigurationManagementCondition",
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
  "ipV6Prefix": "String",
  "ipV6Gateway": "String",
  "ipV6DNSServerList": [
    "String"
  ],
  "dnsSuffixList": [
    "String"
  ]
}
```





