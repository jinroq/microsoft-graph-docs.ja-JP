---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Deleted
ms.openlocfilehash: 1d45219b2ef26bdc96c46e386d66d91874f9bc0b
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/28/2017
---
# <a name="deleted-facet"></a><span data-ttu-id="e9b46-102">Deleted ファセット</span><span class="sxs-lookup"><span data-stu-id="e9b46-102">Deleted facet</span></span>

<span data-ttu-id="e9b46-103">**Deleted** リソースは、アイテムが削除されたことを示します。</span><span class="sxs-lookup"><span data-stu-id="e9b46-103">The **Deleted** resource indicates that the item has been deleted.</span></span>
<span data-ttu-id="e9b46-104">このバージョンの API では、リソースの値が存在する (null 以外である) ことは、ファイルが削除されたことを示します。</span><span class="sxs-lookup"><span data-stu-id="e9b46-104">The Deleted resource indicates that the item has been deleted. In this version of the API, the presence (non-null) of the resource value indicates that the file was deleted. A null (or missing) value indicates that the file is not deleted.</span></span>
<span data-ttu-id="e9b46-105">null (または存在しない) 値は、ファイルが削除されていないことを示します。</span><span class="sxs-lookup"><span data-stu-id="e9b46-105">A null (or missing) value indicates the driveItem is not the root..</span></span>

<span data-ttu-id="e9b46-106">変更の追跡と削除済みアイテムの検出の詳細については、「[アイテムの変更を表示する](../api/driveitem_delta.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e9b46-106">See [view changes for an item](../api/driveitem_delta.md) for more information on tracking changes and finding deleted items.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e9b46-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e9b46-107">JSON representation</span></span>

<span data-ttu-id="e9b46-108">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e9b46-108">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="e9b46-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e9b46-109">Properties</span></span>

| <span data-ttu-id="e9b46-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e9b46-110">Property</span></span> | <span data-ttu-id="e9b46-111">型</span><span class="sxs-lookup"><span data-stu-id="e9b46-111">Type</span></span>   | <span data-ttu-id="e9b46-112">説明</span><span class="sxs-lookup"><span data-stu-id="e9b46-112">Description</span></span>                               |
|:---------|:-------|:------------------------------------------|
| <span data-ttu-id="e9b46-113">state</span><span class="sxs-lookup"><span data-stu-id="e9b46-113">state</span></span>    | <span data-ttu-id="e9b46-114">String</span><span class="sxs-lookup"><span data-stu-id="e9b46-114">String</span></span> | <span data-ttu-id="e9b46-115">削除されたアイテムの状態を表します。</span><span class="sxs-lookup"><span data-stu-id="e9b46-115">Represents the state of the deleted item.</span></span> |

## <a name="remarks"></a><span data-ttu-id="e9b46-116">注釈</span><span class="sxs-lookup"><span data-stu-id="e9b46-116">Remarks</span></span> 

<span data-ttu-id="e9b46-117">DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e9b46-117">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The deleted facet providers properties about deleted items",
  "keywords": "deleted,delete,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Deleted"
} -->
