---
title: groupPolicyPresentationValueList リソースの種類
description: エンティティは、ポリシー定義のリストボックスプレゼンテーションの名前と値のペアのコレクションを表します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 43dc4ed5206e39292ba026f646ae57cac6377ef2
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36331239"
---
# <a name="grouppolicypresentationvaluelist-resource-type"></a>groupPolicyPresentationValueList リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

エンティティは、ポリシー定義のリストボックスプレゼンテーションの名前と値のペアのコレクションを表します。


[Grouppolicypresentationvalue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[GroupPolicyPresentationValueLists のリスト](../api/intune-grouppolicy-grouppolicypresentationvaluelist-list.md)|[Grouppolicypresentationvaluelist](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md)コレクション|[Grouppolicypresentationvaluelist](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[GroupPolicyPresentationValueList の取得](../api/intune-grouppolicy-grouppolicypresentationvaluelist-get.md)|[groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md)|[Grouppolicypresentationvaluelist](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[GroupPolicyPresentationValueList の作成](../api/intune-grouppolicy-grouppolicypresentationvaluelist-create.md)|[groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md)|新しい[Grouppolicypresentationvaluelist](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md)オブジェクトを作成します。|
|[GroupPolicyPresentationValueList の削除](../api/intune-grouppolicy-grouppolicypresentationvaluelist-delete.md)|None|[Grouppolicypresentationvaluelist](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md)を削除します。|
|[GroupPolicyPresentationValueList の更新](../api/intune-grouppolicy-grouppolicypresentationvaluelist-update.md)|[groupPolicyPresentationValueList](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md)|[Grouppolicypresentationvaluelist](../resources/intune-grouppolicy-grouppolicypresentationvaluelist.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|lastModifiedDateTime|DateTimeOffset|オブジェクトが最後に変更された日付と時刻。 [Grouppolicypresentationvalue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)から継承します。|
|createdDateTime|DateTimeOffset|オブジェクトが作成された日付と時刻。 [Grouppolicypresentationvalue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)から継承します。|
|id|String|エンティティのキー。 [Grouppolicypresentationvalue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)から継承します。|
|values|[keyValuePair](../resources/intune-shared-keyvaluepair.md) コレクション|関連付けられているプレゼンテーションのペアのリスト。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|definitionValue|[groupPolicyDefinitionValue](../resources/intune-grouppolicy-grouppolicydefinitionvalue.md)|プレゼンテーション値に関連付けられているグループポリシー定義の値。 [Grouppolicypresentationvalue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)から継承します。|
|プレゼンテーション|[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|プレゼンテーション値に関連付けられたグループポリシーのプレゼンテーション。 [Grouppolicypresentationvalue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)から継承します。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyPresentationValueList"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueList",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "values": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ]
}
```



