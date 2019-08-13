---
title: deviceManagementTemplate リソースの種類
description: デバイス設定の定義済みコレクションを表すエンティティ
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 3e2c7536c61bfaf8287a0a2428e0b861e09f3a5f
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36337623"
---
# <a name="devicemanagementtemplate-resource-type"></a>deviceManagementTemplate リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

デバイス設定の定義済みコレクションを表すエンティティ

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[DeviceManagementTemplates を一覧表示する](../api/intune-deviceintent-devicemanagementtemplate-list.md)|[Devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)コレクション|[Devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[DeviceManagementTemplate の取得](../api/intune-deviceintent-devicemanagementtemplate-get.md)|[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)|[Devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[DeviceManagementTemplate の作成](../api/intune-deviceintent-devicemanagementtemplate-create.md)|[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)|新しい[Devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)オブジェクトを作成します。|
|[DeviceManagementTemplate の削除](../api/intune-deviceintent-devicemanagementtemplate-delete.md)|None|[Devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)を削除します。|
|[DeviceManagementTemplate の更新](../api/intune-deviceintent-devicemanagementtemplate-update.md)|[deviceManagementTemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)|[Devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)オブジェクトのプロパティを更新します。|
|[createInstance アクション](../api/intune-deviceintent-devicemanagementtemplate-createinstance.md)|[deviceManagementIntent](../resources/intune-deviceintent-devicemanagementintent.md)|まだ文書化されていません|
|[compare 関数](../api/intune-deviceintent-devicemanagementtemplate-compare.md)|[Devicemanagementsettingcomparison](../resources/intune-deviceintent-devicemanagementsettingcomparison.md)コレクション|まだ文書化されていません|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列|テンプレート ID|
|displayName|String|テンプレートの表示名|
|description|String|テンプレートの説明|
|versionInfo|String|テンプレートのバージョン情報|
|isDeprecated|Boolean|テンプレートが非推奨になっているか、使用されていません。 推奨されていないテンプレートからは、インテントを作成できません。|
|intentCount|Int32|このテンプレートから作成されたインテントの数。|
|templateType|[deviceManagementTemplateType](../resources/intune-deviceintent-devicemanagementtemplatetype.md)|テンプレートの種類を示します。 可能な値は、`securityBaseline`、`specializedDevices`、`advancedThreatProtectionSecurityBaseline`、`deviceConfiguration`、`custom` です。|
|publishedDateTime|DateTimeOffset|テンプレートが発行されたとき|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|settings|[Devicemanagementsettinginstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)コレクション|このテンプレートに含まれるすべての設定のコレクション|
|categories|[Devicemanagementtemplatesettingcategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md)コレクション|テンプレート内のカテゴリ設定のコレクション|
|migratableTo|[Devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)コレクション|このテンプレートが移行できるテンプレートのコレクション|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementTemplate",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String",
  "versionInfo": "String",
  "isDeprecated": true,
  "intentCount": 1024,
  "templateType": "String",
  "publishedDateTime": "String (timestamp)"
}
```



