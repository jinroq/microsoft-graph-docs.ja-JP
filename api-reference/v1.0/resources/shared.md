---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: 共有
localization_priority: Normal
description: Shared リソースは、DriveItem が他のユーザーと共有されていることを示します。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 547d227aff5b62cf47f3f6c11219a2c55c3e8205
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034329"
---
# <a name="shared-resource-type"></a><span data-ttu-id="1389b-103">Shared リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1389b-103">Shared resource type</span></span>

<span data-ttu-id="1389b-p101">**Shared** リソースは、DriveItem が他のユーザーと共有されていることを示します。リソースは、項目がどのように共有されているかに関する情報を含んでいます。</span><span class="sxs-lookup"><span data-stu-id="1389b-p101">The **Shared** resource indicates a DriveItem has been shared with others. The resource includes information about how the item is shared.</span></span>

<span data-ttu-id="1389b-106">[**Driveitem**](driveitem.md) が null でない **shared** ファセットを持つ場合、項目は共有されています。</span><span class="sxs-lookup"><span data-stu-id="1389b-106">If a [**Driveitem**](driveitem.md) has a non-null **shared** facet, the item has been shared.</span></span>

## <a name="json-representation"></a><span data-ttu-id="1389b-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1389b-107">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="1389b-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1389b-108">Properties</span></span>

| <span data-ttu-id="1389b-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1389b-109">Property</span></span>       | <span data-ttu-id="1389b-110">型</span><span class="sxs-lookup"><span data-stu-id="1389b-110">Type</span></span>                          | <span data-ttu-id="1389b-111">説明</span><span class="sxs-lookup"><span data-stu-id="1389b-111">Description</span></span>
| :------------- |:------------------------------|:----------------------------
| <span data-ttu-id="1389b-112">owner</span><span class="sxs-lookup"><span data-stu-id="1389b-112">owner</span></span>          | [<span data-ttu-id="1389b-113">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="1389b-113">IdentitySet</span></span>](identityset.md) | <span data-ttu-id="1389b-p102">共有項目の所有者の ID。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="1389b-p102">The identity of the owner of the shared item. Read-only.</span></span>
| <span data-ttu-id="1389b-116">scope</span><span class="sxs-lookup"><span data-stu-id="1389b-116">scope</span></span>          | <span data-ttu-id="1389b-117">String</span><span class="sxs-lookup"><span data-stu-id="1389b-117">String</span></span>                        | <span data-ttu-id="1389b-p103">`anonymous`、`organization`、や `users` など、項目がどのように共有されているかのスコープを示します。 読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="1389b-p103">Indicates the scope of how the item is shared: `anonymous`, `organization`, or `users`. Read-only.</span></span>
| <span data-ttu-id="1389b-120">sharedBy</span><span class="sxs-lookup"><span data-stu-id="1389b-120">sharedBy</span></span>       | [<span data-ttu-id="1389b-121">identitySet</span><span class="sxs-lookup"><span data-stu-id="1389b-121">identitySet</span></span>](identityset.md) | <span data-ttu-id="1389b-p104">項目を共有するユーザーの ID。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="1389b-p104">The identity of the user who shared the item. Read-only.</span></span>
| <span data-ttu-id="1389b-124">sharedDateTime</span><span class="sxs-lookup"><span data-stu-id="1389b-124">sharedDateTime</span></span> | <span data-ttu-id="1389b-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1389b-125">DateTimeOffset</span></span>                | <span data-ttu-id="1389b-p105">項目が共有された UTC 日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="1389b-p105">The UTC date and time when the item was shared. Read-only.</span></span>

## <a name="scope-options"></a><span data-ttu-id="1389b-128">範囲オプション</span><span class="sxs-lookup"><span data-stu-id="1389b-128">Scope options</span></span>

| <span data-ttu-id="1389b-129">値</span><span class="sxs-lookup"><span data-stu-id="1389b-129">Value</span></span>          | <span data-ttu-id="1389b-130">説明</span><span class="sxs-lookup"><span data-stu-id="1389b-130">Description</span></span>                                                                           |
|:---------------|:--------------------------------------------------------------------------------------|
| `anonymous`    | <span data-ttu-id="1389b-131">項目は、リンクを持つすべてのユーザーに対して機能するリンクを使用して共有されます。</span><span class="sxs-lookup"><span data-stu-id="1389b-131">The item is shared by using a link that works for anyone with the link.</span></span>               |
| `organization` | <span data-ttu-id="1389b-132">項目は、所有者の組織内にいるすべてのユーザーに対して機能するリンクを使用して共有されます。</span><span class="sxs-lookup"><span data-stu-id="1389b-132">The item is shared by using a link that works for anyone in the owner's organization.</span></span> |
| `users`        | <span data-ttu-id="1389b-133">項目は、特定のユーザーのみと共有されます。</span><span class="sxs-lookup"><span data-stu-id="1389b-133">The item is shared with specific users only.</span></span>                                          |

## <a name="remarks"></a><span data-ttu-id="1389b-134">備考</span><span class="sxs-lookup"><span data-stu-id="1389b-134">Remarks</span></span>

<span data-ttu-id="1389b-135">**driveItem** のファセットに関する詳細については、「[**driveItem**](driveitem.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1389b-135">For more information about the facets on a **driveItem**, see [**driveItem**](driveitem.md).</span></span>

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
