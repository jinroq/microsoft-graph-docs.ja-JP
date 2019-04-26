---
title: groupPolicyPresentationValueLongDecimal リソースの種類
description: エンティティは、ポリシー定義にある長い小数点のテキストボックスプレゼンテーションの符号なしの長い値を表します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1c4386084fff68d6db9be9106bd4da361ed1b933
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32556915"
---
# <a name="grouppolicypresentationvaluelongdecimal-resource-type"></a>groupPolicyPresentationValueLongDecimal リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

エンティティは、ポリシー定義にある長い小数点のテキストボックスプレゼンテーションの符号なしの長い値を表します。


[grouppolicypresentationvalue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト groupPolicyPresentationValueLongDecimals](../api/intune-grouppolicy-grouppolicypresentationvaluelongdecimal-list.md)|[groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md)コレクション|[groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[groupPolicyPresentationValueLongDecimal を取得する](../api/intune-grouppolicy-grouppolicypresentationvaluelongdecimal-get.md)|[groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md)|[groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[groupPolicyPresentationValueLongDecimal を作成する](../api/intune-grouppolicy-grouppolicypresentationvaluelongdecimal-create.md)|[groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md)|新しい[groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md)オブジェクトを作成します。|
|[groupPolicyPresentationValueLongDecimal の削除](../api/intune-grouppolicy-grouppolicypresentationvaluelongdecimal-delete.md)|なし|[groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md)を削除します。|
|[groupPolicyPresentationValueLongDecimal の更新](../api/intune-grouppolicy-grouppolicypresentationvaluelongdecimal-update.md)|[groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md)|[groupPolicyPresentationValueLongDecimal](../resources/intune-grouppolicy-grouppolicypresentationvaluelongdecimal.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|lastModifiedDateTime|DateTimeOffset|オブジェクトが最後に変更された日付と時刻。 [grouppolicypresentationvalue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)から継承します。|
|createdDateTime|DateTimeOffset|オブジェクトが作成された日付と時刻。 [grouppolicypresentationvalue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)から継承します。|
|id|String|エンティティのキー。 [grouppolicypresentationvalue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)から継承します。|
|value|Int64|関連付けられたプレゼンテーションの符号なしの長整数型 (long) の値を指定します。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|definitionvalue|[grouppolicydefinitionvalue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)|プレゼンテーション値に関連付けられているグループポリシー定義の値。 [grouppolicypresentationvalue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)から継承します。|
|プレゼンテーション|[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|プレゼンテーション値に関連付けられたグループポリシーのプレゼンテーション。 [grouppolicypresentationvalue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)から継承します。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyPresentationValueLongDecimal"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueLongDecimal",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "value": 1024
}
```





