---
author: daspek
description: itemActivity に DeleteAction リソースがある場合、アクティビティがアイテムを削除したことを示します。
ms.date: 09/14/2017
title: DeleteAction
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: c5617c61f3221351930ab8d4bf940eaf1efa0629
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973848"
---
# <a name="deleteaction-resource-type"></a><span data-ttu-id="f2a55-103">DeleteAction リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f2a55-103">DeleteAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f2a55-104">[**itemActivity**][activity] に **DeleteAction** リソースがある場合、アクティビティがアイテムを削除したことを示します。</span><span class="sxs-lookup"><span data-stu-id="f2a55-104">The presence of the **DeleteAction** resource on an [**itemActivity**][activity] indicates that the activity deleted an item.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="f2a55-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f2a55-105">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="f2a55-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f2a55-106">Properties</span></span>

| <span data-ttu-id="f2a55-107">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="f2a55-107">Property name</span></span> | <span data-ttu-id="f2a55-108">種類</span><span class="sxs-lookup"><span data-stu-id="f2a55-108">Type</span></span>   | <span data-ttu-id="f2a55-109">説明</span><span class="sxs-lookup"><span data-stu-id="f2a55-109">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="f2a55-110">name</span><span class="sxs-lookup"><span data-stu-id="f2a55-110">name</span></span>          | <span data-ttu-id="f2a55-111">string</span><span class="sxs-lookup"><span data-stu-id="f2a55-111">string</span></span> | <span data-ttu-id="f2a55-112">削除されたアイテムの名前。</span><span class="sxs-lookup"><span data-stu-id="f2a55-112">The name of the item that was deleted.</span></span>
| <span data-ttu-id="f2a55-113">objectType</span><span class="sxs-lookup"><span data-stu-id="f2a55-113">objectType</span></span>    | <span data-ttu-id="f2a55-114">string</span><span class="sxs-lookup"><span data-stu-id="f2a55-114">string</span></span> | <span data-ttu-id="f2a55-115">`File`また`Folder`は、削除されたアイテムの種類によって異なります。</span><span class="sxs-lookup"><span data-stu-id="f2a55-115">`File` or `Folder`, depending on the type of the deleted item.</span></span>

## <a name="remarks"></a><span data-ttu-id="f2a55-116">備考</span><span class="sxs-lookup"><span data-stu-id="f2a55-116">Remarks</span></span>

<span data-ttu-id="f2a55-117">アイテムのアクティビティの記録は、現在、SharePoint と OneDrive for Business でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="f2a55-117">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

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
