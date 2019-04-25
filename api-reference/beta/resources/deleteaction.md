---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: DeleteAction
localization_priority: Normal
ms.openlocfilehash: 5e3b7cbf752d3ddb2c4b7bde3981d2a443028b92
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543248"
---
# <a name="deleteaction-resource-type"></a><span data-ttu-id="6f83e-102">DeleteAction リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6f83e-102">DeleteAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6f83e-103">[**itemActivity**][activity] に **DeleteAction** リソースがある場合、アクティビティがアイテムを削除したことを示します。</span><span class="sxs-lookup"><span data-stu-id="6f83e-103">The presence of the **DeleteAction** resource on an [**itemActivity**][activity] indicates that the activity deleted an item.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="6f83e-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6f83e-104">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.deleteAction"
}-->

```json
{
  "name": "string",
  "objectType": "File | Folder"
}
```

## <a name="properties"></a><span data-ttu-id="6f83e-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6f83e-105">Properties</span></span>

| <span data-ttu-id="6f83e-106">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="6f83e-106">Property name</span></span> | <span data-ttu-id="6f83e-107">種類</span><span class="sxs-lookup"><span data-stu-id="6f83e-107">Type</span></span>   | <span data-ttu-id="6f83e-108">説明</span><span class="sxs-lookup"><span data-stu-id="6f83e-108">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="6f83e-109">name</span><span class="sxs-lookup"><span data-stu-id="6f83e-109">name</span></span>          | <span data-ttu-id="6f83e-110">string</span><span class="sxs-lookup"><span data-stu-id="6f83e-110">string</span></span> | <span data-ttu-id="6f83e-111">削除されたアイテムの名前。</span><span class="sxs-lookup"><span data-stu-id="6f83e-111">The name of the item that was deleted.</span></span>
| <span data-ttu-id="6f83e-112">objectType</span><span class="sxs-lookup"><span data-stu-id="6f83e-112">objectType</span></span>    | <span data-ttu-id="6f83e-113">string</span><span class="sxs-lookup"><span data-stu-id="6f83e-113">string</span></span> | <span data-ttu-id="6f83e-114">`File`また`Folder`は、削除されたアイテムの種類によって異なります。</span><span class="sxs-lookup"><span data-stu-id="6f83e-114">`File` or `Folder`, depending on the type of the deleted item.</span></span>

## <a name="remarks"></a><span data-ttu-id="6f83e-115">備考</span><span class="sxs-lookup"><span data-stu-id="6f83e-115">Remarks</span></span>

<span data-ttu-id="6f83e-116">アイテムのアクティビティの記録は、現在、SharePoint と OneDrive for Business でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="6f83e-116">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The DeleteAction object provides information about the deletion of an item.",
  "keywords": "activities,activity,action,delete,deletion",
  "section": "documentation",
  "tocPath": "Resources/DeleteAction",
  "suppressions": [
    "Error: /api-reference/beta/resources/deleteaction.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
