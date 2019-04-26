---
title: agreementFileData リソースの種類
description: azure Active Directory (azure AD) 利用規約ファイルの blob を表します。
localization_priority: Normal
ms.openlocfilehash: c6f4b6708493c0063928a81c95eeb60b7e7603b0
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33339142"
---
# <a name="agreementfiledata-resource-type"></a>agreementFileData リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

azure Active Directory (azure AD) 利用規約ファイルの blob を表します。

## <a name="properties"></a>プロパティ
| メソッド       | 戻り値の型 | 説明 |
|:-------------|:------------|:------------|
|data|Binary|使用条件を表すデータ。 PDF ドキュメント。 読み取り専用です。|

## <a name="json-representation"></a>JSON 表記

リソースの JSON 表記を次に示します。

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.agreementFileData"
}-->

```json
{
  "data": "Binary"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "agreementFileData resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
