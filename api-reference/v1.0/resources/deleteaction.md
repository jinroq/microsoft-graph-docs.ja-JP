---
author: daspek
ms.author: dspektor
title: deleteAction リソースの種類
description: DeleteAction オブジェクトは、アイテムの削除に関する情報を提供します。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 93f605e74a0a483a94593a9aaa40d6fd30efe914
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36032733"
---
# <a name="deleteaction-resource-type"></a><span data-ttu-id="1791a-103">deleteAction リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1791a-103">deleteAction resource type</span></span>

<span data-ttu-id="1791a-104">[**Itemactivity**][activity]に**deleteaction**リソースが存在することは、アクティビティがアイテムを削除したことを示します。</span><span class="sxs-lookup"><span data-stu-id="1791a-104">The presence of the **deleteAction** resource on an [**itemActivity**][activity] indicates that the activity deleted an item.</span></span>

><span data-ttu-id="1791a-105">**注:** 現時点では、アイテムアクティビティレコードは SharePoint および OneDrive for business でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="1791a-105">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="1791a-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1791a-106">Properties</span></span>

| <span data-ttu-id="1791a-107">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="1791a-107">Property name</span></span> | <span data-ttu-id="1791a-108">種類</span><span class="sxs-lookup"><span data-stu-id="1791a-108">Type</span></span>   | <span data-ttu-id="1791a-109">説明</span><span class="sxs-lookup"><span data-stu-id="1791a-109">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="1791a-110">name</span><span class="sxs-lookup"><span data-stu-id="1791a-110">name</span></span>          | <span data-ttu-id="1791a-111">string</span><span class="sxs-lookup"><span data-stu-id="1791a-111">string</span></span> | <span data-ttu-id="1791a-112">削除されたアイテムの名前。</span><span class="sxs-lookup"><span data-stu-id="1791a-112">The name of the item that was deleted.</span></span>
| <span data-ttu-id="1791a-113">objectType</span><span class="sxs-lookup"><span data-stu-id="1791a-113">objectType</span></span>    | <span data-ttu-id="1791a-114">string</span><span class="sxs-lookup"><span data-stu-id="1791a-114">string</span></span> | <span data-ttu-id="1791a-115">`File`また`Folder`は、削除されたアイテムの種類によって異なります。</span><span class="sxs-lookup"><span data-stu-id="1791a-115">`File` or `Folder`, depending on the type of the deleted item.</span></span>


## <a name="json-representation"></a><span data-ttu-id="1791a-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1791a-116">JSON representation</span></span>

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
