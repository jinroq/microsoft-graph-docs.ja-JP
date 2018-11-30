---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Deleted
ms.openlocfilehash: 5a0dd4132f39574f0af04282bd3f39bfd303eef1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068128"
---
# <a name="deleted-facet"></a><span data-ttu-id="52df5-102">Deleted ファセット</span><span class="sxs-lookup"><span data-stu-id="52df5-102">Deleted facet</span></span>

> <span data-ttu-id="52df5-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="52df5-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="52df5-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="52df5-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="52df5-p102">**削除済み**リソースは、アイテムが削除されたことを示します。このバージョンの API では、リソースの値が存在する (null 以外である) ことは、ファイルが削除されたことを示します。null (または存在しない) 値は、ファイルが削除されていないことを示します。</span><span class="sxs-lookup"><span data-stu-id="52df5-p102">The **Deleted** resource indicates that the item has been deleted. In this version of the API, the presence (non-null) of the resource value indicates that the file was deleted. A null (or missing) value indicates that the file is not deleted.</span></span>

<span data-ttu-id="52df5-108">変更の追跡と削除済みアイテムの検出の詳細については、「[アイテムの変更を表示する](../api/driveitem-delta.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="52df5-108">See [view changes for an item](../api/driveitem-delta.md) for more information on tracking changes and finding deleted items.</span></span>

## <a name="json-representation"></a><span data-ttu-id="52df5-109">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="52df5-109">JSON representation</span></span>

<span data-ttu-id="52df5-110">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="52df5-110">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
  "state"
  ],
  "@odata.type": "microsoft.graph.deleted"
}-->
```json
{
  "state": "string"
}
```
## <a name="properties"></a><span data-ttu-id="52df5-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="52df5-111">Properties</span></span>

| <span data-ttu-id="52df5-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="52df5-112">Property</span></span> | <span data-ttu-id="52df5-113">型</span><span class="sxs-lookup"><span data-stu-id="52df5-113">Type</span></span>   | <span data-ttu-id="52df5-114">説明</span><span class="sxs-lookup"><span data-stu-id="52df5-114">Description</span></span>                               |
|:---------|:-------|:------------------------------------------|
| <span data-ttu-id="52df5-115">state</span><span class="sxs-lookup"><span data-stu-id="52df5-115">state</span></span>    | <span data-ttu-id="52df5-116">String</span><span class="sxs-lookup"><span data-stu-id="52df5-116">String</span></span> | <span data-ttu-id="52df5-117">削除されたアイテムの状態を表します。</span><span class="sxs-lookup"><span data-stu-id="52df5-117">Represents the state of the deleted item.</span></span> |

## <a name="remarks"></a><span data-ttu-id="52df5-118">注釈</span><span class="sxs-lookup"><span data-stu-id="52df5-118">Remarks</span></span> 

<span data-ttu-id="52df5-119">DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="52df5-119">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "The deleted facet providers properties about deleted items",
  "keywords": "deleted,delete,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Deleted"
} -->
