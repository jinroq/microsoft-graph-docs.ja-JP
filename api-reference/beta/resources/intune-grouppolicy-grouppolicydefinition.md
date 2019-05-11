---
title: groupPolicyDefinition リソースの種類
description: エンティティは、1つのグループポリシーに関するすべての情報を記述します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 17fef49d7d08f94f5ebafd02636d9536a05b87f9
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33941171"
---
# <a name="grouppolicydefinition-resource-type"></a>groupPolicyDefinition リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

エンティティは、1つのグループポリシーに関するすべての情報を記述します。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[GroupPolicyDefinition の取得](../api/intune-grouppolicy-grouppolicydefinition-get.md)|[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|[Grouppolicydefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[GroupPolicyDefinition の更新](../api/intune-grouppolicy-grouppolicydefinition-update.md)|[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|[Grouppolicydefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|種類|説明|
|:---|:---|:---|
|classType|[groupPolicyDefinitionClassType](../resources/intune-grouppolicy-grouppolicydefinitionclasstype.md)|ポリシーを適用できるグループの種類を指定します。 可能な値は、`user`、`machine` です。|
|displayName|String|ローカライズされたポリシー名。|
|explainText|String|ポリシーに関連付けられたローカライズされた説明またはヘルプテキスト。 既定値は空白です。|
|categoryPath|String|ポリシーのローカライズされた完全なカテゴリのパス。|
|supportedOn|String|ポリシーによって影響を受けるオペレーティングシステムまたはアプリケーションのバージョンを指定するために使用されるローカライズされた文字列。|
|Msrtcsip-policytype|[groupPolicyType](../resources/intune-grouppolicy-grouppolicytype.md)|グループポリシーの種類を指定します。 可能な値は、`admxBacked`、`admxIngested` です。|
|id|文字列|エンティティのキー。|
|lastModifiedDateTime|DateTimeOffset|エンティティが最後に変更された日付と時刻。|

## <a name="relationships"></a>関係
|リレーションシップ|型|説明|
|:---|:---|:---|
|definitionFile|[groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|定義に関連付けられているグループポリシーファイル。|
|プレゼンテーション|[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)コレクション|定義に関連付けられたグループポリシーのプレゼンテーション。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyDefinition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyDefinition",
  "classType": "String",
  "displayName": "String",
  "explainText": "String",
  "categoryPath": "String",
  "supportedOn": "String",
  "policyType": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```




