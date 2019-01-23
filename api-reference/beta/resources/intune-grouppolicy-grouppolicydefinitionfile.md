---
title: groupPolicyDefinitionFile リソースの種類
description: エンティティでは、ADMX (管理テンプレート) の XML ファイルを表します。 ADMX ファイルには、カテゴリへのパスでのグループ ポリシーの定義のコレクションとその場所が含まれています。 グループ ポリシー定義ファイルには、言語依存の ADML (管理テンプレート) の言語ファイルでサポートされる言語も含まれています。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 9ac5206321047dd4cd54732103e4adb70221e860
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431621"
---
# <a name="grouppolicydefinitionfile-resource-type"></a>groupPolicyDefinitionFile リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

エンティティでは、ADMX (管理テンプレート) の XML ファイルを表します。 ADMX ファイルには、カテゴリへのパスでのグループ ポリシーの定義のコレクションとその場所が含まれています。 グループ ポリシー定義ファイルには、言語依存の ADML (管理テンプレート) の言語ファイルでサポートされる言語も含まれています。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[GroupPolicyDefinitionFile を取得します。](../api/intune-grouppolicy-grouppolicydefinitionfile-get.md)|[groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|[GroupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)オブジェクトのプロパティと関係を参照してください。|
|[GroupPolicyDefinitionFile を更新します。](../api/intune-grouppolicy-grouppolicydefinitionfile-update.md)|[groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|[GroupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|displayName|String|ADMX ファイルのローカライズされた表示名です。|
|説明|String|ADMX ファイル内のポリシー設定のローカライズされた説明。 既定値は空です。|
|languageCodes|String コレクション|ADMX ファイルのサポートされている言語コードです。|
|targetPrefix|String|ADMX ファイル内で名前空間を参照する論理名を指定します。|
|targetNamespace|String|ADMX ファイル内で名前空間を識別するために使用する URI を指定します。|
|policyType|[groupPolicyType](../resources/intune-grouppolicy-grouppolicytype.md)|グループ ポリシーの種類を指定します。 使用可能な値は、`admxBacked`、`admxIngested` です。|
|id|String|エンティティのキー。|
|lastModifiedDateTime|DateTimeOffset|日付と時刻、エンティティが最後に修正されました。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|定義|[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)コレクション|ファイルに関連付けられているグループ ポリシーの定義です。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyDefinitionFile"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyDefinitionFile",
  "displayName": "String",
  "description": "String",
  "languageCodes": [
    "String"
  ],
  "targetPrefix": "String",
  "targetNamespace": "String",
  "policyType": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```




