---
title: groupPolicyPresentationDropdownList リソースの種類
description: ADMX の dropdownList 要素と ADMX enum 要素を表します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: a12a210156727ed7dd00bd79e7c2f711aa518a8f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36010953"
---
# <a name="grouppolicypresentationdropdownlist-resource-type"></a>groupPolicyPresentationDropdownList リソースの種類

> **重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

ADMX の dropdownList 要素と ADMX enum 要素を表します。


[GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[GroupPolicyPresentationDropdownLists のリスト](../api/intune-grouppolicy-grouppolicypresentationdropdownlist-list.md)|[Grouppolicypresentationdropdownlist](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md)コレクション|[Grouppolicypresentationdropdownlist](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[GroupPolicyPresentationDropdownList の取得](../api/intune-grouppolicy-grouppolicypresentationdropdownlist-get.md)|[groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md)|[Grouppolicypresentationdropdownlist](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[GroupPolicyPresentationDropdownList の作成](../api/intune-grouppolicy-grouppolicypresentationdropdownlist-create.md)|[groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md)|新しい[Grouppolicypresentationdropdownlist](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md)オブジェクトを作成します。|
|[GroupPolicyPresentationDropdownList の削除](../api/intune-grouppolicy-grouppolicypresentationdropdownlist-delete.md)|None|[Grouppolicypresentationdropdownlist](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md)を削除します。|
|[GroupPolicyPresentationDropdownList の更新](../api/intune-grouppolicy-grouppolicypresentationdropdownlist-update.md)|[groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md)|[Grouppolicypresentationdropdownlist](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|label|String|任意のプレゼンテーションエンティティのローカライズされたテキストラベル。 既定値は空白です。 [GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。|
|id|String|エンティティのキー。 [GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。|
|lastModifiedDateTime|DateTimeOffset|エンティティが最後に変更された日付と時刻。 [GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。|
|defaultItem|[groupPolicyPresentationDropdownListItem](../resources/intune-grouppolicy-grouppolicypresentationdropdownlistitem.md)|アイテムのリストの既定の選択を示すローカライズされた文字列値。|
|items|[Grouppolicypresentationdropdownlistitem](../resources/intune-grouppolicy-grouppolicypresentationdropdownlistitem.md)コレクション|ローカライズされた表示名とそれに関連する値のセットを表します。|
|必須|Boolean|[パラメーター] ボックスに値を入力する必要があります。 既定値は false です。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|definition|[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|プレゼンテーションに関連付けられたグループポリシーの定義。 [GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。|

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





