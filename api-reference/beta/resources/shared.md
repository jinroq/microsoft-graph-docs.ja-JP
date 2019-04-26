---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 共有
localization_priority: Normal
ms.openlocfilehash: 143593615d34d069c8378f1cb068fc000d076192
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343177"
---
# <a name="shared-resource-type"></a>Shared リソースの種類

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

**Shared** リソースは、DriveItem が他のユーザーと共有されていることを示します。リソースは、項目がどのように共有されているかに関する情報を含んでいます。

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
| scope          | String                        | `anonymous`、`organization`、や `users` など、項目がどのように共有されているかのスコープを示します。 読み取り専用。
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

<!--
{
  "type": "#page.annotation",
  "description": "The shared facet provides info about shared items.",
  "keywords": "shared,share,item,facet,onedrive",
  "section": "documentation",
  "tocPath": "Facets/Shared",
  "suppressions": []
}
-->
