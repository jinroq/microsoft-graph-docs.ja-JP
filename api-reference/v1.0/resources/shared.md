---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Shared
ms.openlocfilehash: 1d828310a226edd0443ff3b5f60156df1e7c98cb
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/28/2017
---
# <a name="shared-resource-type"></a>Shared リソース型

**Shared** リソースは、DriveItem が他のユーザーと共有されていることを示します。
リソースは、項目がどのように共有されているかに関する情報を含んでいます。

[**Driveitem**](driveitem.md) が null でない **shared** ファセットを持つ場合、項目は共有されています。

## <a name="json-representation"></a>JSON 表記

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.shared",
  "optionalProperties": [ "sharedBy", "sharedDateTime" ]
}-->

```json
{
  "owner": { "@odata.type": "microsoft.graph.identitySet" },
  "scope": "anonymous | organization | users",
  "sharedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "sharedDateTime": "datetime"
}
```

## <a name="properties"></a>プロパティ

| プロパティ       | 型                          | 説明
| :------------- |:------------------------------|:----------------------------
| owner          | [IdentitySet](identityset.md) | 共有項目の所有者の ID。読み取り専用。
| scope          | 文字列                        | `anonymous`、`organization`、や `users` など、項目がどのように共有されているかのスコープを示します。  読み取り専用です。
| sharedBy       | [identitySet](identityset.md) | 項目を共有するユーザーの ID。読み取り専用です。
| sharedDateTime | DateTimeOffset                | 項目が共有された UTC 日時。読み取り専用です。

## <a name="scope-values"></a>スコープの値

| 値          | 説明                                                                           |
|:---------------|:--------------------------------------------------------------------------------------|
| `anonymous`    | 項目は、リンクを持つすべてのユーザーに対して機能するリンクを使用して共有されます。               |
| `organization` | 項目は、所有者の組織内にいるすべてのユーザーに対して機能するリンクを使用して共有されます。 |
| `users`        | 項目は、特定のユーザーのみと共有されます。                                          |

## <a name="remarks"></a>備考

**driveItem** のファセットに関する詳細については、「[**driveItem**](driveitem.md)」を参照してください。

<!-- {
  "type": "#page.annotation",
  "description": "The shared facet provides info about shared items.",
  "keywords": "shared,share,item,facet,onedrive",
  "section": "documentation",
  "tocPath": "Facets/Shared"
} -->
