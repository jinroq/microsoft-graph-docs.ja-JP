---
title: securityBaselineTemplate リソースの種類
description: アカウントのセキュリティベースラインテンプレート
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 8af050df4b90314ad823535860e08557075966df
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36319314"
---
# <a name="securitybaselinetemplate-resource-type"></a>securityBaselineTemplate リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

アカウントのセキュリティベースラインテンプレート


[Devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト securityBaselineTemplates](../api/intune-deviceintent-securitybaselinetemplate-list.md)|[securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md)コレクション|[SecurityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[SecurityBaselineTemplate を取得する](../api/intune-deviceintent-securitybaselinetemplate-get.md)|[securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md)|[SecurityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[SecurityBaselineTemplate を作成する](../api/intune-deviceintent-securitybaselinetemplate-create.md)|[securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md)|新しい[securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md)オブジェクトを作成します。|
|[SecurityBaselineTemplate の削除](../api/intune-deviceintent-securitybaselinetemplate-delete.md)|None|[SecurityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md)を削除します。|
|[SecurityBaselineTemplate の更新](../api/intune-deviceintent-securitybaselinetemplate-update.md)|[securityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md)|[SecurityBaselineTemplate](../resources/intune-deviceintent-securitybaselinetemplate.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|id|文字列|[Devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)から継承されたテンプレート ID|
|displayName|String|[Devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)から継承されたテンプレートの表示名|
|description|String|[Devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)から継承されるテンプレートの説明|
|versionInfo|String|[Devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)から継承されたテンプレートのバージョン情報|
|isDeprecated|Boolean|テンプレートが非推奨になっているか、使用されていません。 推奨されていないテンプレートからは、インテントを作成できません。 [Devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)から継承します|
|intentCount|Int32|このテンプレートから作成されたインテントの数。 [Devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)から継承します|
|templateType|[deviceManagementTemplateType](../resources/intune-deviceintent-devicemanagementtemplatetype.md)|テンプレートの種類を示します。 [Devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)から継承されます。 可能な値は、`securityBaseline`、`specializedDevices`、`advancedThreatProtectionSecurityBaseline`、`deviceConfiguration`、`custom` です。|
|publishedDateTime|DateTimeOffset|テンプレートが公開された場合 ( [Devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)から継承)|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|settings|[Devicemanagementsettinginstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)コレクション|このテンプレートが[Devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)から継承したすべての設定のコレクション|
|categories|[Devicemanagementtemplatesettingcategory](../resources/intune-deviceintent-devicemanagementtemplatesettingcategory.md)コレクション|[Devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)から継承されるテンプレート内のカテゴリ設定のコレクション|
|migratableTo|[Devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)コレクション|テンプレートのコレクションこのテンプレートは、 [Devicemanagementtemplate](../resources/intune-deviceintent-devicemanagementtemplate.md)から継承されるように移行できます。|
|deviceStateSummary|[securityBaselineStateSummary](../resources/intune-deviceintent-securitybaselinestatesummary.md)|セキュリティベースラインデバイスの状態の概要|
|deviceStates|[securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md)コレクション|セキュリティベースラインデバイスの状態|
|categoryDeviceStateSummaries|[securityBaselineCategoryStateSummary](../resources/intune-deviceintent-securitybaselinecategorystatesummary.md)コレクション|カテゴリ別のセキュリティベースラインデバイス状態の概要|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.securityBaselineTemplate"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.securityBaselineTemplate",
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



