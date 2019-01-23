---
title: groupPolicyPresentationDropdownList リソースの種類
description: ADMX dropdownList 要素と ADMX 列挙型の要素を表します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 4c7f35a52e43598f09b3fccdce1ef1d869798e7b
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430490"
---
# <a name="grouppolicypresentationdropdownlist-resource-type"></a>groupPolicyPresentationDropdownList リソースの種類

> **重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。 実稼働アプリケーションでこれらの API を使用することは、サポートされていません。

> **注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

ADMX dropdownList 要素と ADMX 列挙型の要素を表します。


[GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[リスト groupPolicyPresentationDropdownLists](../api/intune-grouppolicy-grouppolicypresentationdropdownlist-list.md)|[groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md)コレクション|[GroupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md)オブジェクトのプロパティと関係を一覧表示します。|
|[GroupPolicyPresentationDropdownList を取得します。](../api/intune-grouppolicy-grouppolicypresentationdropdownlist-get.md)|[groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md)|[GroupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md)オブジェクトのプロパティと関係を参照してください。|
|[GroupPolicyPresentationDropdownList を作成します。](../api/intune-grouppolicy-grouppolicypresentationdropdownlist-create.md)|[groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md)|新しい[groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md)オブジェクトを作成します。|
|[GroupPolicyPresentationDropdownList を削除します。](../api/intune-grouppolicy-grouppolicypresentationdropdownlist-delete.md)|なし|の[groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md)を削除します。|
|[GroupPolicyPresentationDropdownList を更新します。](../api/intune-grouppolicy-grouppolicypresentationdropdownlist-update.md)|[groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md)|[GroupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|label|String|プレゼンテーションの任意のエンティティのローカライズされたテキスト ラベルです。 既定値は空です。 [GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承されました。|
|id|String|エンティティのキー。 [GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承されました。|
|lastModifiedDateTime|DateTimeOffset|日付と時刻、エンティティが最後に修正されました。 [GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承されました。|
|defaultItem|[groupPolicyPresentationDropdownListItem](../resources/intune-grouppolicy-grouppolicypresentationdropdownlistitem.md)|項目のリストの既定の選択肢を識別する文字列値をローカライズします。|
|items|[groupPolicyPresentationDropdownListItem](../resources/intune-grouppolicy-grouppolicypresentationdropdownlistitem.md)コレクション|一連のローカライズされた表示名とその値を表します。|
|必須|Boolean|パラメーター] ボックスに値を入力するための要件です。 既定値は、false を指定します。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|definition|[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|プレゼンテーションに関連付けられているグループ ポリシーの定義です。 [GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承されました。|

## <a name="json-representation"></a>JSON 表記
以下は、リソースの JSON 表記です。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyPresentationDropdownList"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationDropdownList",
  "label": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "defaultItem": {
    "@odata.type": "microsoft.graph.groupPolicyPresentationDropdownListItem",
    "displayName": "String",
    "value": "String"
  },
  "items": [
    {
      "@odata.type": "microsoft.graph.groupPolicyPresentationDropdownListItem",
      "displayName": "String",
      "value": "String"
    }
  ],
  "required": true
}
```




