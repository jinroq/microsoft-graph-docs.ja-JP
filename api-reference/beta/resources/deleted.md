---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: Deleted
localization_priority: Normal
ms.openlocfilehash: de832eb4ecdf36081b00b94679dcafe9b94fe007
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529440"
---
# <a name="deleted-facet"></a><span data-ttu-id="2994b-102">Deleted ファセット</span><span class="sxs-lookup"><span data-stu-id="2994b-102">Deleted facet</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2994b-p101">削除済みリソースは、アイテムが削除されたことを示します。このバージョンの API では、リソースの値が存在する (null 以外である) ことは、ファイルが削除されたことを示します。null (または存在しない) 値は、ファイルが削除されていないことを示します。</span><span class="sxs-lookup"><span data-stu-id="2994b-p101">The **Deleted** resource indicates that the item has been deleted. In this version of the API, the presence (non-null) of the resource value indicates that the file was deleted. A null (or missing) value indicates that the file is not deleted.</span></span>

<span data-ttu-id="2994b-106">変更の追跡と削除済みアイテムの検出の詳細については、「[アイテムの変更を表示する](../api/driveitem-delta.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2994b-106">See [view changes for an item](../api/driveitem-delta.md) for more information on tracking changes and finding deleted items.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2994b-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2994b-107">JSON representation</span></span>

<span data-ttu-id="2994b-108">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2994b-108">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="2994b-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2994b-109">Properties</span></span>

| <span data-ttu-id="2994b-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2994b-110">Property</span></span> | <span data-ttu-id="2994b-111">型</span><span class="sxs-lookup"><span data-stu-id="2994b-111">Type</span></span>   | <span data-ttu-id="2994b-112">説明</span><span class="sxs-lookup"><span data-stu-id="2994b-112">Description</span></span>                               |
|:---------|:-------|:------------------------------------------|
| <span data-ttu-id="2994b-113">state</span><span class="sxs-lookup"><span data-stu-id="2994b-113">state</span></span>    | <span data-ttu-id="2994b-114">String</span><span class="sxs-lookup"><span data-stu-id="2994b-114">String</span></span> | <span data-ttu-id="2994b-115">削除されたアイテムの状態を表します。</span><span class="sxs-lookup"><span data-stu-id="2994b-115">Represents the state of the deleted item.</span></span> |

## <a name="remarks"></a><span data-ttu-id="2994b-116">注釈</span><span class="sxs-lookup"><span data-stu-id="2994b-116">Remarks</span></span> 

<span data-ttu-id="2994b-117">DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2994b-117">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "The deleted facet providers properties about deleted items",
  "keywords": "deleted,delete,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Deleted",
  "suppressions": [
    "Error: /api-reference/beta/resources/deleted.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
