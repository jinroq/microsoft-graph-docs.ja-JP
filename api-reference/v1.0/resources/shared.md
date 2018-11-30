---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Shared
ms.openlocfilehash: 0a94a1d5ddf671151cf786d9ff93ae4f9e012a7b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022307"
---
# <a name="shared-resource-type"></a><span data-ttu-id="b8f70-102">Shared リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b8f70-102">Shared resource type</span></span>

<span data-ttu-id="b8f70-p101">**Shared** リソースは、DriveItem が他のユーザーと共有されていることを示します。リソースは、項目がどのように共有されているかに関する情報を含んでいます。</span><span class="sxs-lookup"><span data-stu-id="b8f70-p101">The **Shared** resource indicates a DriveItem has been shared with others. The resource includes information about how the item is shared.</span></span>

<span data-ttu-id="b8f70-105">[**Driveitem**](driveitem.md) が null でない **shared** ファセットを持つ場合、項目は共有されています。</span><span class="sxs-lookup"><span data-stu-id="b8f70-105">If a [**Driveitem**](driveitem.md) has a non-null **shared** facet, the item has been shared.</span></span>

## <a name="json-representation"></a><span data-ttu-id="b8f70-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b8f70-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="b8f70-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b8f70-107">Properties</span></span>

| <span data-ttu-id="b8f70-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b8f70-108">Property</span></span>       | <span data-ttu-id="b8f70-109">型</span><span class="sxs-lookup"><span data-stu-id="b8f70-109">Type</span></span>                          | <span data-ttu-id="b8f70-110">説明</span><span class="sxs-lookup"><span data-stu-id="b8f70-110">Description</span></span>
| :------------- |:------------------------------|:----------------------------
| <span data-ttu-id="b8f70-111">owner</span><span class="sxs-lookup"><span data-stu-id="b8f70-111">owner</span></span>          | [<span data-ttu-id="b8f70-112">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="b8f70-112">IdentitySet</span></span>](identityset.md) | <span data-ttu-id="b8f70-p102">共有項目の所有者の ID。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="b8f70-p102">The identity of the owner of the shared item. Read-only.</span></span>
| <span data-ttu-id="b8f70-115">scope</span><span class="sxs-lookup"><span data-stu-id="b8f70-115">scope</span></span>          | <span data-ttu-id="b8f70-116">文字列</span><span class="sxs-lookup"><span data-stu-id="b8f70-116">String</span></span>                        | <span data-ttu-id="b8f70-p103">`anonymous`、`organization`、や `users` など、項目がどのように共有されているかのスコープを示します。 読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b8f70-p103">Indicates the scope of how the item is shared: `anonymous`, `organization`, or `users`. Read-only.</span></span>
| <span data-ttu-id="b8f70-119">sharedBy</span><span class="sxs-lookup"><span data-stu-id="b8f70-119">sharedBy</span></span>       | [<span data-ttu-id="b8f70-120">identitySet</span><span class="sxs-lookup"><span data-stu-id="b8f70-120">identitySet</span></span>](identityset.md) | <span data-ttu-id="b8f70-p104">項目を共有するユーザーの ID。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b8f70-p104">The identity of the user who shared the item. Read-only.</span></span>
| <span data-ttu-id="b8f70-123">sharedDateTime</span><span class="sxs-lookup"><span data-stu-id="b8f70-123">sharedDateTime</span></span> | <span data-ttu-id="b8f70-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b8f70-124">DateTimeOffset</span></span>                | <span data-ttu-id="b8f70-p105">項目が共有された UTC 日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b8f70-p105">The UTC date and time when the item was shared. Read-only.</span></span>

## <a name="scope-options"></a><span data-ttu-id="b8f70-127">スコープ オプション</span><span class="sxs-lookup"><span data-stu-id="b8f70-127">Scope options</span></span>

| <span data-ttu-id="b8f70-128">値</span><span class="sxs-lookup"><span data-stu-id="b8f70-128">Value</span></span>          | <span data-ttu-id="b8f70-129">説明</span><span class="sxs-lookup"><span data-stu-id="b8f70-129">Description</span></span>                                                                           |
|:---------------|:--------------------------------------------------------------------------------------|
| `anonymous`    | <span data-ttu-id="b8f70-130">項目は、リンクを持つすべてのユーザーに対して機能するリンクを使用して共有されます。</span><span class="sxs-lookup"><span data-stu-id="b8f70-130">The item is shared by using a link that works for anyone with the link.</span></span>               |
| `organization` | <span data-ttu-id="b8f70-131">項目は、所有者の組織内にいるすべてのユーザーに対して機能するリンクを使用して共有されます。</span><span class="sxs-lookup"><span data-stu-id="b8f70-131">The item is shared by using a link that works for anyone in the owner's organization.</span></span> |
| `users`        | <span data-ttu-id="b8f70-132">項目は、特定のユーザーのみと共有されます。</span><span class="sxs-lookup"><span data-stu-id="b8f70-132">The item is shared with specific users only.</span></span>                                          |

## <a name="remarks"></a><span data-ttu-id="b8f70-133">備考</span><span class="sxs-lookup"><span data-stu-id="b8f70-133">Remarks</span></span>

<span data-ttu-id="b8f70-134">**driveItem** のファセットに関する詳細については、「[**driveItem**](driveitem.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b8f70-134">For more information about the facets on a **driveItem**, see [**driveItem**](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The shared facet provides info about shared items.",
  "keywords": "shared,share,item,facet,onedrive",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/shared.md:
      Found potential enums in resource example that weren't defined in a table:(anonymous,organization,users) are in resource, but () are in table"
  ],
  "tocPath": "Facets/Shared"
} -->
