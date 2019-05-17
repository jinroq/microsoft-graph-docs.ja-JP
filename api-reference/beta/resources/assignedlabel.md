---
title: assignedLabel リソースの種類
description: Office 365 グループに割り当てられた機密ラベルを表します。 機密ラベルを使用すると、管理者はグループに分類を割り当てることにより、グループに特定のグループ設定を適用することができます (機密、高機密、一般)。
localization_priority: Normal
author: krbain
ms.prod: groups
ms.openlocfilehash: 430387f228bf632a7f9f9b4a046537bbe5ff4953
ms.sourcegitcommit: b18ccb24fc79f3abb470cd759e25cdd266fc77c7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/17/2019
ms.locfileid: "34117621"
---
# <a name="assignedlabel-resource-type"></a>assignedLabel リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

Office 365 グループに割り当てられた機密ラベルを表します。 機密ラベルを使用すると、管理者はグループに分類を割り当てることにより、グループに特定のグループ設定を適用することができます (機密、高機密、一般)。 機密ラベルは microsoft 365 Security & コンプライアンスセンターの管理者によって、Microsoft Information Protection 機能の一部として公開されています。 機密ラベルの詳細については、「[感度ラベルの概要](https://docs.microsoft.com/en-us/Office365/SecurityCompliance/sensitivity-labels)」を参照してください。

## <a name="properties"></a>プロパティ
| プロパティ     | 型   |説明|
|:---------------|:--------|:----------|
|Lab_ d|String|ラベルの一意識別子。|
|displayName|String|ラベルの表示名を指定します。 読み取り専用です。|

## <a name="json-representation"></a>JSON 表記

以下は、リソースの JSON 表記です。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.assignedLabel"
}-->

```json
{
  "labelId": "String",
  "displayName": "String"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "assignedLabel resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
