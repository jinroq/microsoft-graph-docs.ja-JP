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
# <a name="shared-resource-type"></a><span data-ttu-id="0e5b3-102">Shared リソース型</span><span class="sxs-lookup"><span data-stu-id="0e5b3-102">Shared resource type</span></span>

<span data-ttu-id="0e5b3-103">**Shared** リソースは、DriveItem が他のユーザーと共有されていることを示します。</span><span class="sxs-lookup"><span data-stu-id="0e5b3-103">The **Shared** resource indicates a DriveItem has been shared with others. The resource includes information about how the item is shared.</span></span>
<span data-ttu-id="0e5b3-104">リソースは、項目がどのように共有されているかに関する情報を含んでいます。</span><span class="sxs-lookup"><span data-stu-id="0e5b3-104">The Shared resource indicates a DriveItem has been shared with others. The resource includes information about how the item is shared.</span></span>

<span data-ttu-id="0e5b3-105">[**Driveitem**](driveitem.md) が null でない **shared** ファセットを持つ場合、項目は共有されています。</span><span class="sxs-lookup"><span data-stu-id="0e5b3-105">If a [**Driveitem**](driveitem.md) has a non-null **shared** facet, the item has been shared.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0e5b3-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0e5b3-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="0e5b3-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0e5b3-107">Properties</span></span>

| <span data-ttu-id="0e5b3-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0e5b3-108">Property</span></span>       | <span data-ttu-id="0e5b3-109">型</span><span class="sxs-lookup"><span data-stu-id="0e5b3-109">Type</span></span>                          | <span data-ttu-id="0e5b3-110">説明</span><span class="sxs-lookup"><span data-stu-id="0e5b3-110">Description</span></span>
| :------------- |:------------------------------|:----------------------------
| <span data-ttu-id="0e5b3-111">owner</span><span class="sxs-lookup"><span data-stu-id="0e5b3-111">owner</span></span>          | [<span data-ttu-id="0e5b3-112">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="0e5b3-112">IdentitySet</span></span>](identityset.md) | <span data-ttu-id="0e5b3-p102">共有項目の所有者の ID。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="0e5b3-p102">The identity of the owner of the shared item. Read-only.</span></span>
| <span data-ttu-id="0e5b3-115">scope</span><span class="sxs-lookup"><span data-stu-id="0e5b3-115">scope</span></span>          | <span data-ttu-id="0e5b3-116">文字列</span><span class="sxs-lookup"><span data-stu-id="0e5b3-116">String</span></span>                        | <span data-ttu-id="0e5b3-117">`anonymous`、`organization`、や `users` など、項目がどのように共有されているかのスコープを示します。 </span><span class="sxs-lookup"><span data-stu-id="0e5b3-117">Indicates the scope of how the item is shared: `anonymous`, `organization`, or `users`.</span></span> <span data-ttu-id="0e5b3-118">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="0e5b3-118">Read-only.</span></span>
| <span data-ttu-id="0e5b3-119">sharedBy</span><span class="sxs-lookup"><span data-stu-id="0e5b3-119">sharedBy</span></span>       | [<span data-ttu-id="0e5b3-120">identitySet</span><span class="sxs-lookup"><span data-stu-id="0e5b3-120">identitySet</span></span>](identityset.md) | <span data-ttu-id="0e5b3-p104">項目を共有するユーザーの ID。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="0e5b3-p104">The identity of the user who shared the item. Read-only.</span></span>
| <span data-ttu-id="0e5b3-123">sharedDateTime</span><span class="sxs-lookup"><span data-stu-id="0e5b3-123">sharedDateTime</span></span> | <span data-ttu-id="0e5b3-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0e5b3-124">DateTimeOffset</span></span>                | <span data-ttu-id="0e5b3-p105">項目が共有された UTC 日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="0e5b3-p105">The UTC date and time when the item was shared. Read-only.</span></span>

## <a name="scope-values"></a><span data-ttu-id="0e5b3-127">スコープの値</span><span class="sxs-lookup"><span data-stu-id="0e5b3-127">Scope values</span></span>

| <span data-ttu-id="0e5b3-128">値</span><span class="sxs-lookup"><span data-stu-id="0e5b3-128">Value</span></span>          | <span data-ttu-id="0e5b3-129">説明</span><span class="sxs-lookup"><span data-stu-id="0e5b3-129">Description</span></span>                                                                           |
|:---------------|:--------------------------------------------------------------------------------------|
| `anonymous`    | <span data-ttu-id="0e5b3-130">項目は、リンクを持つすべてのユーザーに対して機能するリンクを使用して共有されます。</span><span class="sxs-lookup"><span data-stu-id="0e5b3-130">The item is shared by using a link that works for anyone with the link.</span></span>               |
| `organization` | <span data-ttu-id="0e5b3-131">項目は、所有者の組織内にいるすべてのユーザーに対して機能するリンクを使用して共有されます。</span><span class="sxs-lookup"><span data-stu-id="0e5b3-131">The item is shared by using a link that works for anyone in the owner's organization.</span></span> |
| `users`        | <span data-ttu-id="0e5b3-132">項目は、特定のユーザーのみと共有されます。</span><span class="sxs-lookup"><span data-stu-id="0e5b3-132">The item is shared with specific users only.</span></span>                                          |

## <a name="remarks"></a><span data-ttu-id="0e5b3-133">備考</span><span class="sxs-lookup"><span data-stu-id="0e5b3-133">Remarks</span></span>

<span data-ttu-id="0e5b3-134">**driveItem** のファセットに関する詳細については、「[**driveItem**](driveitem.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0e5b3-134">For more information about the facets on a **driveItem**, see [**driveItem**](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The shared facet provides info about shared items.",
  "keywords": "shared,share,item,facet,onedrive",
  "section": "documentation",
  "tocPath": "Facets/Shared"
} -->
