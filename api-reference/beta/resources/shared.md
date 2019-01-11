---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Shared
localization_priority: Normal
ms.openlocfilehash: cae69a60691d388570d29176fc20aac429907f8a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27838991"
---
# <a name="shared-resource-type"></a><span data-ttu-id="31f37-102">Shared リソースの種類</span><span class="sxs-lookup"><span data-stu-id="31f37-102">Shared resource type</span></span>

> <span data-ttu-id="31f37-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="31f37-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="31f37-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="31f37-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="31f37-p102">**Shared** リソースは、DriveItem が他のユーザーと共有されていることを示します。リソースは、項目がどのように共有されているかに関する情報を含んでいます。</span><span class="sxs-lookup"><span data-stu-id="31f37-p102">The **Shared** resource indicates a DriveItem has been shared with others. The resource includes information about how the item is shared.</span></span>

<span data-ttu-id="31f37-107">[**Driveitem**](driveitem.md) が null でない **shared** ファセットを持つ場合、項目は共有されています。</span><span class="sxs-lookup"><span data-stu-id="31f37-107">If a [**Driveitem**](driveitem.md) has a non-null **shared** facet, the item has been shared.</span></span>

## <a name="json-representation"></a><span data-ttu-id="31f37-108">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="31f37-108">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="31f37-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="31f37-109">Properties</span></span>

| <span data-ttu-id="31f37-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="31f37-110">Property</span></span>       | <span data-ttu-id="31f37-111">種類</span><span class="sxs-lookup"><span data-stu-id="31f37-111">Type</span></span>                          | <span data-ttu-id="31f37-112">説明</span><span class="sxs-lookup"><span data-stu-id="31f37-112">Description</span></span>
| :------------- |:------------------------------|:----------------------------
| <span data-ttu-id="31f37-113">owner</span><span class="sxs-lookup"><span data-stu-id="31f37-113">owner</span></span>          | [<span data-ttu-id="31f37-114">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="31f37-114">IdentitySet</span></span>](identityset.md) | <span data-ttu-id="31f37-p103">共有項目の所有者の ID。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="31f37-p103">The identity of the owner of the shared item. Read-only.</span></span>
| <span data-ttu-id="31f37-117">scope</span><span class="sxs-lookup"><span data-stu-id="31f37-117">scope</span></span>          | <span data-ttu-id="31f37-118">String</span><span class="sxs-lookup"><span data-stu-id="31f37-118">String</span></span>                        | <span data-ttu-id="31f37-p104">`anonymous`、`organization`、や `users` など、項目がどのように共有されているかのスコープを示します。 読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="31f37-p104">Indicates the scope of how the item is shared: `anonymous`, `organization`, or `users`. Read-only.</span></span>
| <span data-ttu-id="31f37-121">sharedBy</span><span class="sxs-lookup"><span data-stu-id="31f37-121">sharedBy</span></span>       | [<span data-ttu-id="31f37-122">identitySet</span><span class="sxs-lookup"><span data-stu-id="31f37-122">identitySet</span></span>](identityset.md) | <span data-ttu-id="31f37-p105">項目を共有するユーザーの ID。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="31f37-p105">The identity of the user who shared the item. Read-only.</span></span>
| <span data-ttu-id="31f37-125">sharedDateTime</span><span class="sxs-lookup"><span data-stu-id="31f37-125">sharedDateTime</span></span> | <span data-ttu-id="31f37-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="31f37-126">DateTimeOffset</span></span>                | <span data-ttu-id="31f37-p106">項目が共有された UTC 日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="31f37-p106">The UTC date and time when the item was shared. Read-only.</span></span>

## <a name="scope-values"></a><span data-ttu-id="31f37-129">スコープの値</span><span class="sxs-lookup"><span data-stu-id="31f37-129">Scope values</span></span>

| <span data-ttu-id="31f37-130">値</span><span class="sxs-lookup"><span data-stu-id="31f37-130">Value</span></span>          | <span data-ttu-id="31f37-131">説明</span><span class="sxs-lookup"><span data-stu-id="31f37-131">Description</span></span>                                                                           |
|:---------------|:--------------------------------------------------------------------------------------|
| `anonymous`    | <span data-ttu-id="31f37-132">項目は、リンクを持つすべてのユーザーに対して機能するリンクを使用して共有されます。</span><span class="sxs-lookup"><span data-stu-id="31f37-132">The item is shared by using a link that works for anyone with the link.</span></span>               |
| `organization` | <span data-ttu-id="31f37-133">項目は、所有者の組織内にいるすべてのユーザーに対して機能するリンクを使用して共有されます。</span><span class="sxs-lookup"><span data-stu-id="31f37-133">The item is shared by using a link that works for anyone in the owner's organization.</span></span> |
| `users`        | <span data-ttu-id="31f37-134">項目は、特定のユーザーのみと共有されます。</span><span class="sxs-lookup"><span data-stu-id="31f37-134">The item is shared with specific users only.</span></span>                                          |

## <a name="remarks"></a><span data-ttu-id="31f37-135">備考</span><span class="sxs-lookup"><span data-stu-id="31f37-135">Remarks</span></span>

<span data-ttu-id="31f37-136">**driveItem** のファセットに関する詳細については、「[**driveItem**](driveitem.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="31f37-136">For more information about the facets on a **driveItem**, see [**driveItem**](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The shared facet provides info about shared items.",
  "keywords": "shared,share,item,facet,onedrive",
  "section": "documentation",
  "tocPath": "Facets/Shared"
} -->
