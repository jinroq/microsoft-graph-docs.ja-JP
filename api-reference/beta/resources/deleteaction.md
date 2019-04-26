---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: DeleteAction
localization_priority: Normal
ms.openlocfilehash: a380376a813df5f519464978851049e020ded8b8
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340954"
---
# <a name="deleteaction-resource-type"></a><span data-ttu-id="7be21-102">DeleteAction リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7be21-102">DeleteAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7be21-103">[**itemActivity**][activity] に **DeleteAction** リソースがある場合、アクティビティがアイテムを削除したことを示します。</span><span class="sxs-lookup"><span data-stu-id="7be21-103">The presence of the **DeleteAction** resource on an [**itemActivity**][activity] indicates that the activity deleted an item.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="7be21-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7be21-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="7be21-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7be21-105">Properties</span></span>

| <span data-ttu-id="7be21-106">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="7be21-106">Property name</span></span> | <span data-ttu-id="7be21-107">種類</span><span class="sxs-lookup"><span data-stu-id="7be21-107">Type</span></span>   | <span data-ttu-id="7be21-108">説明</span><span class="sxs-lookup"><span data-stu-id="7be21-108">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="7be21-109">name</span><span class="sxs-lookup"><span data-stu-id="7be21-109">name</span></span>          | <span data-ttu-id="7be21-110">string</span><span class="sxs-lookup"><span data-stu-id="7be21-110">string</span></span> | <span data-ttu-id="7be21-111">削除されたアイテムの名前。</span><span class="sxs-lookup"><span data-stu-id="7be21-111">The name of the item that was deleted.</span></span>
| <span data-ttu-id="7be21-112">objectType</span><span class="sxs-lookup"><span data-stu-id="7be21-112">objectType</span></span>    | <span data-ttu-id="7be21-113">string</span><span class="sxs-lookup"><span data-stu-id="7be21-113">string</span></span> | <span data-ttu-id="7be21-114">`File`また`Folder`は、削除されたアイテムの種類によって異なります。</span><span class="sxs-lookup"><span data-stu-id="7be21-114">`File` or `Folder`, depending on the type of the deleted item.</span></span>

## <a name="remarks"></a><span data-ttu-id="7be21-115">備考</span><span class="sxs-lookup"><span data-stu-id="7be21-115">Remarks</span></span>

<span data-ttu-id="7be21-116">アイテムのアクティビティの記録は、現在、SharePoint と OneDrive for Business でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="7be21-116">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The DeleteAction object provides information about the deletion of an item.",
  "keywords": "activities,activity,action,delete,deletion",
  "section": "documentation",
  "tocPath": "Resources/DeleteAction",
  "suppressions": []
}
-->
