---
title: grouppolicydefinition リソースの種類
description: エンティティは、1つのグループポリシーに関するすべての情報を記述します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7c5062fda984dbe1dda518e77ff271750d30adb8
ms.sourcegitcommit: cd4bdb2c6754b1d5658e68909ea6c219466da6df
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/16/2019
ms.locfileid: "30644287"
---
# <a name="grouppolicydefinition-resource-type"></a>grouppolicydefinition リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

エンティティは、1つのグループポリシーに関するすべての情報を記述します。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[grouppolicydefinition の取得](../api/intune-grouppolicy-grouppolicydefinition-get.md)|[grouppolicydefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|[grouppolicydefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[grouppolicydefinition の更新](../api/intune-grouppolicy-grouppolicydefinition-update.md)|[grouppolicydefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|[grouppolicydefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|classType|[grouppolicydefinitionclasstype](../resources/intune-grouppolicy-grouppolicydefinitionclasstype.md)|ポリシーを適用できるグループの種類を指定します。 可能な値は、`user`、`machine` です。|
|displayName|String|ローカライズされたポリシー名。|
|explainText|String|ポリシーに関連付けられたローカライズされた説明またはヘルプテキスト。 既定値は空白です。|
|categoryPath|String|ポリシーのローカライズされた完全なカテゴリのパス。|
|supportedOn|String|ポリシーによって影響を受けるオペレーティングシステムまたはアプリケーションのバージョンを指定するために使用されるローカライズされた文字列。|
|msrtcsip-policytype|[groupPolicyType](../resources/intune-grouppolicy-grouppolicytype.md)|グループポリシーの種類を指定します。 可能な値は、`admxBacked`、`admxIngested` です。|
|id|String|エンティティのキー。|
|lastModifiedDateTime|DateTimeOffset|エンティティが最後に変更された日付と時刻。|

## <a name="relationships"></a>関係
|リレーションシップ|型|説明|
|:---|:---|:---|
|definitionfile|[grouppolicydefinitionfile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|定義に関連付けられているグループポリシーファイル。|
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




