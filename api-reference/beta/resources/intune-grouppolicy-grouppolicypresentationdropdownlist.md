---
title: grouppolicypresentationdropdownlist リソースの種類
description: admx の dropdownList 要素と admx enum 要素を表します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b70b9b5385203921151e4bc9f01c2e3a7d28cd8d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32575717"
---
# <a name="grouppolicypresentationdropdownlist-resource-type"></a>grouppolicypresentationdropdownlist リソースの種類

> **重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。

> **注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

admx の dropdownList 要素と admx enum 要素を表します。


[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。

## <a name="methods"></a>メソッド
|メソッド|戻り値の型|説明|
|:---|:---|:---|
|[grouppolicypresentationdropdownlists のリスト](../api/intune-grouppolicy-grouppolicypresentationdropdownlist-list.md)|[grouppolicypresentationdropdownlist](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md)コレクション|[grouppolicypresentationdropdownlist](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md)オブジェクトのプロパティとリレーションシップをリストします。|
|[grouppolicypresentationdropdownlist の取得](../api/intune-grouppolicy-grouppolicypresentationdropdownlist-get.md)|[grouppolicypresentationdropdownlist](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md)|[grouppolicypresentationdropdownlist](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md)オブジェクトのプロパティとリレーションシップを読み取ります。|
|[grouppolicypresentationdropdownlist の作成](../api/intune-grouppolicy-grouppolicypresentationdropdownlist-create.md)|[grouppolicypresentationdropdownlist](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md)|新しい[grouppolicypresentationdropdownlist](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md)オブジェクトを作成します。|
|[grouppolicypresentationdropdownlist の削除](../api/intune-grouppolicy-grouppolicypresentationdropdownlist-delete.md)|なし|[grouppolicypresentationdropdownlist](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md)を削除します。|
|[grouppolicypresentationdropdownlist の更新](../api/intune-grouppolicy-grouppolicypresentationdropdownlist-update.md)|[grouppolicypresentationdropdownlist](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md)|[grouppolicypresentationdropdownlist](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md)オブジェクトのプロパティを更新します。|

## <a name="properties"></a>プロパティ
|プロパティ|型|説明|
|:---|:---|:---|
|label|String|任意のプレゼンテーションエンティティのローカライズされたテキストラベル。 既定値は空白です。 [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。|
|id|String|エンティティのキー。 [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。|
|lastModifiedDateTime|DateTimeOffset|エンティティが最後に変更された日付と時刻。 [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。|
|defaultitem|[grouppolicypresentationdropdownlistitem](../resources/intune-grouppolicy-grouppolicypresentationdropdownlistitem.md)|アイテムのリストの既定の選択を示すローカライズされた文字列値。|
|items|[grouppolicypresentationdropdownlistitem](../resources/intune-grouppolicy-grouppolicypresentationdropdownlistitem.md)コレクション|ローカライズされた表示名とそれに関連する値のセットを表します。|
|必須|Boolean|[パラメーター] ボックスに値を入力する必要があります。 既定値は false です。|

## <a name="relationships"></a>リレーションシップ
|リレーションシップ|型|説明|
|:---|:---|:---|
|definition|[grouppolicydefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|プレゼンテーションに関連付けられたグループポリシーの定義。 [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承します。|

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





