---
title: groupPolicyDefinition リソースの種類
description: エンティティでは、すべての単一のグループ ポリシーに関する情報について説明します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 502312f7a39dd5dc93fd8e39203f56d47a9ebf27
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430491"
---
# <a name="grouppolicydefinition-resource-type"></a>groupPolicyDefinition リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

エンティティでは、すべての単一のグループ ポリシーに関する情報について説明します。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[GroupPolicyDefinition を取得します。](../api/intune-grouppolicy-grouppolicydefinition-get.md)|[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|[GroupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)オブジェクトのプロパティと関係を参照してください。|
|[GroupPolicyDefinition を更新します。](../api/intune-grouppolicy-grouppolicydefinition-update.md)|[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|[GroupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|classType|[groupPolicyDefinitionClassType](../resources/intune-grouppolicy-grouppolicydefinitionclasstype.md)|ポリシーを適用できるグループの種類を識別します。 可能な値は、`user`、`machine`、`both` です。|
|displayName|String|ローカライズされたポリシーの名前です。|
|説明|String|ローカライズされた説明またはヘルプ テキスト、ポリシーに関連付けられています。 既定値は空です。|
|categoryPath|String|ポリシーのすべてのローカライズされたカテゴリのパスです。|
|supportedOn|String|どのようなオペレーティング システムまたはアプリケーションのバージョンを指定するために使用するローカライズされた文字列は、ポリシーの影響を受けます。|
|policyType|[groupPolicyType](../resources/intune-grouppolicy-grouppolicytype.md)|グループ ポリシーの種類を指定します。 使用可能な値は、`admxBacked`、`admxIngested` です。|
|id|String|エンティティのキー。|
|lastModifiedDateTime|DateTimeOffset|日付と時刻、エンティティが最後に修正されました。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|-definitionfile|[groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|定義に関連付けられているグループ ポリシー ファイルです。|
|プレゼンテーション|[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)コレクション|定義に関連付けられているグループ ポリシーのプレゼンテーションです。|

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




