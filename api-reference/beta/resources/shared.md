---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Shared
ms.openlocfilehash: 38bc8604ba2528a24e2193a2fb521428b2b5c2d3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072222"
---
# <a name="shared-resource-type"></a><span data-ttu-id="373bc-102">Shared リソースの種類</span><span class="sxs-lookup"><span data-stu-id="373bc-102">Shared resource type</span></span>

> <span data-ttu-id="373bc-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="373bc-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="373bc-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="373bc-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="373bc-p102">**Shared** リソースは、DriveItem が他のユーザーと共有されていることを示します。リソースは、項目がどのように共有されているかに関する情報を含んでいます。</span><span class="sxs-lookup"><span data-stu-id="373bc-p102">The **Shared** resource indicates a DriveItem has been shared with others. The resource includes information about how the item is shared.</span></span>

<span data-ttu-id="373bc-107">[**Driveitem**](driveitem.md) が null でない **shared** ファセットを持つ場合、項目は共有されています。</span><span class="sxs-lookup"><span data-stu-id="373bc-107">If a [**Driveitem**](driveitem.md) has a non-null **shared** facet, the item has been shared.</span></span>

## <a name="json-representation"></a><span data-ttu-id="373bc-108">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="373bc-108">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="373bc-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="373bc-109">Properties</span></span>

| <span data-ttu-id="373bc-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="373bc-110">Property</span></span>       | <span data-ttu-id="373bc-111">型</span><span class="sxs-lookup"><span data-stu-id="373bc-111">Type</span></span>                          | <span data-ttu-id="373bc-112">説明</span><span class="sxs-lookup"><span data-stu-id="373bc-112">Description</span></span>
| :------------- |:------------------------------|:----------------------------
| <span data-ttu-id="373bc-113">owner</span><span class="sxs-lookup"><span data-stu-id="373bc-113">owner</span></span>          | [<span data-ttu-id="373bc-114">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="373bc-114">IdentitySet</span></span>](identityset.md) | <span data-ttu-id="373bc-p103">共有項目の所有者の ID。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="373bc-p103">The identity of the owner of the shared item. Read-only.</span></span>
| <span data-ttu-id="373bc-117">scope</span><span class="sxs-lookup"><span data-stu-id="373bc-117">scope</span></span>          | <span data-ttu-id="373bc-118">String</span><span class="sxs-lookup"><span data-stu-id="373bc-118">String</span></span>                        | <span data-ttu-id="373bc-p104">`anonymous`、`organization`、や `users` など、項目がどのように共有されているかのスコープを示します。 読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="373bc-p104">Indicates the scope of how the item is shared: `anonymous`, `organization`, or `users`. Read-only.</span></span>
| <span data-ttu-id="373bc-121">sharedBy</span><span class="sxs-lookup"><span data-stu-id="373bc-121">sharedBy</span></span>       | [<span data-ttu-id="373bc-122">identitySet</span><span class="sxs-lookup"><span data-stu-id="373bc-122">identitySet</span></span>](identityset.md) | <span data-ttu-id="373bc-p105">項目を共有するユーザーの ID。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="373bc-p105">The identity of the user who shared the item. Read-only.</span></span>
| <span data-ttu-id="373bc-125">sharedDateTime</span><span class="sxs-lookup"><span data-stu-id="373bc-125">sharedDateTime</span></span> | <span data-ttu-id="373bc-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="373bc-126">DateTimeOffset</span></span>                | <span data-ttu-id="373bc-p106">項目が共有された UTC 日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="373bc-p106">The UTC date and time when the item was shared. Read-only.</span></span>

## <a name="scope-values"></a><span data-ttu-id="373bc-129">スコープの値</span><span class="sxs-lookup"><span data-stu-id="373bc-129">Scope values</span></span>

| <span data-ttu-id="373bc-130">値</span><span class="sxs-lookup"><span data-stu-id="373bc-130">Value</span></span>          | <span data-ttu-id="373bc-131">説明</span><span class="sxs-lookup"><span data-stu-id="373bc-131">Description</span></span>                                                                           |
|:---------------|:--------------------------------------------------------------------------------------|
| `anonymous`    | <span data-ttu-id="373bc-132">項目は、リンクを持つすべてのユーザーに対して機能するリンクを使用して共有されます。</span><span class="sxs-lookup"><span data-stu-id="373bc-132">The item is shared by using a link that works for anyone with the link.</span></span>               |
| `organization` | <span data-ttu-id="373bc-133">項目は、所有者の組織内にいるすべてのユーザーに対して機能するリンクを使用して共有されます。</span><span class="sxs-lookup"><span data-stu-id="373bc-133">The item is shared by using a link that works for anyone in the owner's organization.</span></span> |
| `users`        | <span data-ttu-id="373bc-134">項目は、特定のユーザーのみと共有されます。</span><span class="sxs-lookup"><span data-stu-id="373bc-134">The item is shared with specific users only.</span></span>                                          |

## <a name="remarks"></a><span data-ttu-id="373bc-135">備考</span><span class="sxs-lookup"><span data-stu-id="373bc-135">Remarks</span></span>

<span data-ttu-id="373bc-136">**driveItem** のファセットに関する詳細については、「[**driveItem**](driveitem.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="373bc-136">For more information about the facets on a **driveItem**, see [**driveItem**](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The shared facet provides info about shared items.",
  "keywords": "shared,share,item,facet,onedrive",
  "section": "documentation",
  "tocPath": "Facets/Shared"
} -->
