---
title: groupPolicyPresentation リソースの種類
description: グループ ポリシーの定義の他のオプションのいずれかの表示のプレゼンテーションの基本エンティティです。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 736b599eaf310bc63530daa45ffa1aee7ede4c3f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430543"
---
# <a name="grouppolicypresentation-resource-type"></a>groupPolicyPresentation リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

グループ ポリシーの定義の他のオプションのいずれかの表示のプレゼンテーションの基本エンティティです。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[GroupPolicyPresentation を取得します。](../api/intune-grouppolicy-grouppolicypresentation-get.md)|[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|[GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)オブジェクトのプロパティと関係を参照してください。|
|[GroupPolicyPresentation を更新します。](../api/intune-grouppolicy-grouppolicypresentation-update.md)|[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|[GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|label|String|プレゼンテーションの任意のエンティティのローカライズされたテキスト ラベルです。 既定値は空です。|
|id|String|エンティティのキー。|
|lastModifiedDateTime|DateTimeOffset|日付と時刻、エンティティが最後に修正されました。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|definition|[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|プレゼンテーションに関連付けられているグループ ポリシーの定義です。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyPresentation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentation",
  "label": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```




