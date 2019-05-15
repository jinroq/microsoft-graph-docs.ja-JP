---
author: daspek
ms.author: dspektor
title: deleteAction リソースの種類
description: DeleteAction オブジェクトは、アイテムの削除に関する情報を提供します。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: ba5004c17f1cc71f66420a81b5eb66603df00eee
ms.sourcegitcommit: 52baf24d1d08096214b12f60e7c755291fe03ab5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/13/2019
ms.locfileid: "33970779"
---
# <a name="deleteaction-resource-type"></a><span data-ttu-id="ff6ee-103">deleteAction リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ff6ee-103">deleteAction resource type</span></span>

<span data-ttu-id="ff6ee-104">[**Itemactivity**] [ activity]に**deleteaction**リソースが存在することは、アクティビティがアイテムを削除したことを示します。</span><span class="sxs-lookup"><span data-stu-id="ff6ee-104">The presence of the **deleteAction** resource on an [**itemActivity**][activity] indicates that the activity deleted an item.</span></span>

><span data-ttu-id="ff6ee-105">**注:** 現時点では、アイテムアクティビティレコードは SharePoint および OneDrive for business でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="ff6ee-105">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="ff6ee-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ff6ee-106">Properties</span></span>

| <span data-ttu-id="ff6ee-107">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="ff6ee-107">Property name</span></span> | <span data-ttu-id="ff6ee-108">種類</span><span class="sxs-lookup"><span data-stu-id="ff6ee-108">Type</span></span>   | <span data-ttu-id="ff6ee-109">説明</span><span class="sxs-lookup"><span data-stu-id="ff6ee-109">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="ff6ee-110">name</span><span class="sxs-lookup"><span data-stu-id="ff6ee-110">name</span></span>          | <span data-ttu-id="ff6ee-111">string</span><span class="sxs-lookup"><span data-stu-id="ff6ee-111">string</span></span> | <span data-ttu-id="ff6ee-112">削除されたアイテムの名前。</span><span class="sxs-lookup"><span data-stu-id="ff6ee-112">The name of the item that was deleted.</span></span>
| <span data-ttu-id="ff6ee-113">objectType</span><span class="sxs-lookup"><span data-stu-id="ff6ee-113">objectType</span></span>    | <span data-ttu-id="ff6ee-114">string</span><span class="sxs-lookup"><span data-stu-id="ff6ee-114">string</span></span> | <span data-ttu-id="ff6ee-115">`File`また`Folder`は、削除されたアイテムの種類によって異なります。</span><span class="sxs-lookup"><span data-stu-id="ff6ee-115">`File` or `Folder`, depending on the type of the deleted item.</span></span>


## <a name="json-representation"></a><span data-ttu-id="ff6ee-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ff6ee-116">JSON representation</span></span>

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

<!--
{
  "type": "#page.annotation",
  "description": "The deleteAction object provides information about the deletion of an item.",
  "keywords": "activities,activity,action,delete,deletion",
  "section": "documentation",
  "tocPath": "Resources/DeleteAction",
  "suppressions": []
}
-->
