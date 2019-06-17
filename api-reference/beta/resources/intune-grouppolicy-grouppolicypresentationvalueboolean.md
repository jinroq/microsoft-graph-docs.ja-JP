---
title: groupPolicyPresentationValueBoolean リソースの種類
description: エンティティは、ポリシー定義のチェックボックスプレゼンテーションのブール値を表します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9e7abc5ef2d4a9ef6af4cfbf49f24b92fa542778
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34996359"
---
# <a name="grouppolicypresentationvalueboolean-resource-type"></a>groupPolicyPresentationValueBoolean リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

エンティティは、ポリシー定義のチェックボックスプレゼンテーションのブール値を表します。


[Grouppolicypresentationvalue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)から継承します

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[GroupPolicyPresentationValueBooleans のリスト](../api/intune-grouppolicy-grouppolicypresentationvalueboolean-list.md)|[Grouppolicypresentationvalueboolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md)コレクション|[Grouppolicypresentationvalueboolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[GroupPolicyPresentationValueBoolean の取得](../api/intune-grouppolicy-grouppolicypresentationvalueboolean-get.md)|[groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md)|[Grouppolicypresentationvalueboolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[GroupPolicyPresentationValueBoolean の作成](../api/intune-grouppolicy-grouppolicypresentationvalueboolean-create.md)|[groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md)|新しい[Grouppolicypresentationvalueboolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md)オブジェクトを作成します。|
|[GroupPolicyPresentationValueBoolean の削除](../api/intune-grouppolicy-grouppolicypresentationvalueboolean-delete.md)|None|[Grouppolicypresentationvalueboolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md)を削除します。|
|[GroupPolicyPresentationValueBoolean の更新](../api/intune-grouppolicy-grouppolicypresentationvalueboolean-update.md)|[groupPolicyPresentationValueBoolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md)|[Grouppolicypresentationvalueboolean](../resources/intune-grouppolicy-grouppolicypresentationvalueboolean.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|lastModifiedDateTime|DateTimeOffset|オブジェクトが最後に変更された日付と時刻。 [Grouppolicypresentationvalue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)から継承します。|
|createdDateTime|DateTimeOffset|オブジェクトが作成された日付と時刻。 [Grouppolicypresentationvalue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)から継承します。|
|id|String|エンティティのキー。 [Grouppolicypresentationvalue](../resources/intune-grouppolicy-grouppolicypresentationvalue.md)から継承します。|
|value|ブール型 (Boolean)|関連付けられたプレゼンテーションのブール値。|

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
  "@odata.type": "microsoft.graph.groupPolicyPresentationValueBoolean"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationValueBoolean",
  "lastModifiedDateTime": "String (timestamp)",
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "value": true
}
```





