---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/10/2017
title: Deleted
localization_priority: Normal
description: Deleted リソースは、アイテムが削除されたことを示します。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: d1f5c07c60c8de4890a2a4ac334df04a59b7339c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029520"
---
# <a name="deleted-facet"></a><span data-ttu-id="c3594-103">Deleted ファセット</span><span class="sxs-lookup"><span data-stu-id="c3594-103">Deleted facet</span></span>

<span data-ttu-id="c3594-p101">**削除済み**リソースは、アイテムが削除されたことを示します。このバージョンの API では、リソースの値が存在する (null 以外である) ことは、ファイルが削除されたことを示します。null (または存在しない) 値は、ファイルが削除されていないことを示します。</span><span class="sxs-lookup"><span data-stu-id="c3594-p101">The **Deleted** resource indicates that the item has been deleted. In this version of the API, the presence (non-null) of the resource value indicates that the file was deleted. A null (or missing) value indicates that the file is not deleted.</span></span>

<span data-ttu-id="c3594-107">変更の追跡と削除済みアイテムの検出の詳細については、「[アイテムの変更を表示する](../api/driveitem-delta.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c3594-107">See [view changes for an item](../api/driveitem-delta.md) for more information on tracking changes and finding deleted items.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c3594-108">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c3594-108">JSON representation</span></span>

<span data-ttu-id="c3594-109">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c3594-109">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="c3594-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c3594-110">Properties</span></span>

| <span data-ttu-id="c3594-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c3594-111">Property</span></span> | <span data-ttu-id="c3594-112">型</span><span class="sxs-lookup"><span data-stu-id="c3594-112">Type</span></span>   | <span data-ttu-id="c3594-113">説明</span><span class="sxs-lookup"><span data-stu-id="c3594-113">Description</span></span>                               |
|:---------|:-------|:------------------------------------------|
| <span data-ttu-id="c3594-114">state</span><span class="sxs-lookup"><span data-stu-id="c3594-114">state</span></span>    | <span data-ttu-id="c3594-115">String</span><span class="sxs-lookup"><span data-stu-id="c3594-115">String</span></span> | <span data-ttu-id="c3594-116">削除されたアイテムの状態を表します。</span><span class="sxs-lookup"><span data-stu-id="c3594-116">Represents the state of the deleted item.</span></span> |

## <a name="remarks"></a><span data-ttu-id="c3594-117">注釈</span><span class="sxs-lookup"><span data-stu-id="c3594-117">Remarks</span></span> 

<span data-ttu-id="c3594-118">DriveItem のファセットの詳細については、「[DriveItem](driveitem.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c3594-118">For more information about the facets on a DriveItem, see [DriveItem](driveitem.md).</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The deleted facet providers properties about deleted items",
  "keywords": "deleted,delete,item,facet",
  "section": "documentation",
  "tocPath": "Facets/Deleted"
} -->
