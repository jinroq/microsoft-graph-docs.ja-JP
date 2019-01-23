---
title: groupPolicyPresentationValue リソースの種類
description: 1 つのグループ ポリシーのプレゼンテーションの値が格納されているプレゼンテーションの基本値のエンティティです。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: ec299eccc29ddcb39ece0d1f6c0e063a02192909
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430259"
---
# <a name="grouppolicypresentationvalue-resource-type"></a>groupPolicyPresentationValue リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

1 つのグループ ポリシーのプレゼンテーションの値が格納されているプレゼンテーションの基本値のエンティティです。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト groupPolicyPresentationValues](../api/intune-grouppolicy-grouppolicypresentationvalue-list.md)|[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)コレクション|[GroupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)オブジェクトのプロパティと関係を一覧表示します。|
|[GroupPolicyPresentationValue を取得します。](../api/intune-grouppolicy-grouppolicypresentationvalue-get.md)|[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|[GroupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)オブジェクトのプロパティと関係を参照してください。|
|[GroupPolicyPresentationValue を作成します。](../api/intune-grouppolicy-grouppolicypresentationvalue-create.md)|[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|新しい[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)オブジェクトを作成します。|
|[GroupPolicyPresentationValue を削除します。](../api/intune-grouppolicy-grouppolicypresentationvalue-delete.md)|なし|の[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)を削除します。|
|[GroupPolicyPresentationValue を更新します。](../api/intune-grouppolicy-grouppolicypresentationvalue-update.md)|[groupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)|[GroupPolicyPresentationValue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|lastModifiedDateTime|DateTimeOffset|日付と時刻オブジェクトが最後に修正されました。|
|createdDateTime|DateTimeOffset|日付と時刻オブジェクトを作成します。|
|id|String|エンティティのキー。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|definitionValue|[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)|プレゼンテーションの値に関連付けられているグループ ポリシーの定義の値です。|
|プレゼンテーション|[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|プレゼンテーションの値に関連付けられているグループ ポリシーのプレゼンテーションです。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyPresentationValue"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValue",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)"
}
```




