---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Shared
localization_priority: Normal
ms.openlocfilehash: 33b12ea8e530fd862619c9c20e77a76989efb619
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29507699"
---
# <a name="shared-resource-type"></a><span data-ttu-id="12cab-102">Shared リソースの種類</span><span class="sxs-lookup"><span data-stu-id="12cab-102">Shared resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="12cab-p101">Shared リソースは、DriveItem が他のユーザーと共有されていることを示します。リソースは、項目がどのように共有されているかに関する情報を含んでいます。</span><span class="sxs-lookup"><span data-stu-id="12cab-p101">The **Shared** resource indicates a DriveItem has been shared with others. The resource includes information about how the item is shared.</span></span>

<span data-ttu-id="12cab-105">[**Driveitem**](driveitem.md) が null でない **shared** ファセットを持つ場合、項目は共有されています。</span><span class="sxs-lookup"><span data-stu-id="12cab-105">If a [**Driveitem**](driveitem.md) has a non-null **shared** facet, the item has been shared.</span></span>

## <a name="json-representation"></a><span data-ttu-id="12cab-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="12cab-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="12cab-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="12cab-107">Properties</span></span>

| <span data-ttu-id="12cab-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="12cab-108">Property</span></span>       | <span data-ttu-id="12cab-109">型</span><span class="sxs-lookup"><span data-stu-id="12cab-109">Type</span></span>                          | <span data-ttu-id="12cab-110">説明</span><span class="sxs-lookup"><span data-stu-id="12cab-110">Description</span></span>
| :------------- |:------------------------------|:----------------------------
| <span data-ttu-id="12cab-111">owner</span><span class="sxs-lookup"><span data-stu-id="12cab-111">owner</span></span>          | [<span data-ttu-id="12cab-112">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="12cab-112">IdentitySet</span></span>](identityset.md) | <span data-ttu-id="12cab-p102">共有項目の所有者の ID。読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="12cab-p102">The identity of the owner of the shared item. Read-only.</span></span>
| <span data-ttu-id="12cab-115">scope</span><span class="sxs-lookup"><span data-stu-id="12cab-115">scope</span></span>          | <span data-ttu-id="12cab-116">文字列</span><span class="sxs-lookup"><span data-stu-id="12cab-116">String</span></span>                        | <span data-ttu-id="12cab-p103">`anonymous`、`organization`、や `users` など、項目がどのように共有されているかのスコープを示します。 読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="12cab-p103">Indicates the scope of how the item is shared: `anonymous`, `organization`, or `users`. Read-only.</span></span>
| <span data-ttu-id="12cab-119">sharedBy</span><span class="sxs-lookup"><span data-stu-id="12cab-119">sharedBy</span></span>       | [<span data-ttu-id="12cab-120">identitySet</span><span class="sxs-lookup"><span data-stu-id="12cab-120">identitySet</span></span>](identityset.md) | <span data-ttu-id="12cab-p104">項目を共有するユーザーの ID。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="12cab-p104">The identity of the user who shared the item. Read-only.</span></span>
| <span data-ttu-id="12cab-123">sharedDateTime</span><span class="sxs-lookup"><span data-stu-id="12cab-123">sharedDateTime</span></span> | <span data-ttu-id="12cab-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="12cab-124">DateTimeOffset</span></span>                | <span data-ttu-id="12cab-p105">項目が共有された UTC 日時。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="12cab-p105">The UTC date and time when the item was shared. Read-only.</span></span>

## <a name="scope-values"></a><span data-ttu-id="12cab-127">スコープの値</span><span class="sxs-lookup"><span data-stu-id="12cab-127">Scope values</span></span>

| <span data-ttu-id="12cab-128">値</span><span class="sxs-lookup"><span data-stu-id="12cab-128">Value</span></span>          | <span data-ttu-id="12cab-129">説明</span><span class="sxs-lookup"><span data-stu-id="12cab-129">Description</span></span>                                                                           |
|:---------------|:--------------------------------------------------------------------------------------|
| `anonymous`    | <span data-ttu-id="12cab-130">項目は、リンクを持つすべてのユーザーに対して機能するリンクを使用して共有されます。</span><span class="sxs-lookup"><span data-stu-id="12cab-130">The item is shared by using a link that works for anyone with the link.</span></span>               |
| `organization` | <span data-ttu-id="12cab-131">項目は、所有者の組織内にいるすべてのユーザーに対して機能するリンクを使用して共有されます。</span><span class="sxs-lookup"><span data-stu-id="12cab-131">The item is shared by using a link that works for anyone in the owner's organization.</span></span> |
| `users`        | <span data-ttu-id="12cab-132">項目は、特定のユーザーのみと共有されます。</span><span class="sxs-lookup"><span data-stu-id="12cab-132">The item is shared with specific users only.</span></span>                                          |

## <a name="remarks"></a><span data-ttu-id="12cab-133">備考</span><span class="sxs-lookup"><span data-stu-id="12cab-133">Remarks</span></span>

<span data-ttu-id="12cab-134">**driveItem** のファセットに関する詳細については、「[**driveItem**](driveitem.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="12cab-134">For more information about the facets on a **driveItem**, see [**driveItem**](driveitem.md).</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The shared facet provides info about shared items.",
  "keywords": "shared,share,item,facet,onedrive",
  "section": "documentation",
  "tocPath": "Facets/Shared",
  "suppressions": [
    "Error: /api-reference/beta/resources/shared.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
