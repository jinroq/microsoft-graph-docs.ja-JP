---
author: daspek
ms.author: dspektor
title: renameAction リソースの種類
description: RenameAction オブジェクトは、アイテムの名前を変更したアクティビティに関する情報を提供します。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 2949a3875d657dba3c64b6753855476c1d66bfb3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034721"
---
# <a name="renameaction-resource-type"></a><span data-ttu-id="c72ff-103">renameAction リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c72ff-103">renameAction resource type</span></span>

<span data-ttu-id="c72ff-104">[**Itemactivity**][activity]に**renameaction**リソースが存在することは、アクティビティがアイテムの名前を変更したことを示します。</span><span class="sxs-lookup"><span data-stu-id="c72ff-104">The presence of the **renameAction** resource on an [**itemActivity**][activity] indicates that the activity renamed an item.</span></span>

><span data-ttu-id="c72ff-105">**注:** 現時点では、アイテムアクティビティレコードは SharePoint および OneDrive for business でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="c72ff-105">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="c72ff-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c72ff-106">Properties</span></span>

| <span data-ttu-id="c72ff-107">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="c72ff-107">Property name</span></span> | <span data-ttu-id="c72ff-108">種類</span><span class="sxs-lookup"><span data-stu-id="c72ff-108">Type</span></span>   | <span data-ttu-id="c72ff-109">説明</span><span class="sxs-lookup"><span data-stu-id="c72ff-109">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="c72ff-110">oldName</span><span class="sxs-lookup"><span data-stu-id="c72ff-110">oldName</span></span>       | <span data-ttu-id="c72ff-111">string</span><span class="sxs-lookup"><span data-stu-id="c72ff-111">string</span></span> | <span data-ttu-id="c72ff-112">アイテムの変更前の名前。</span><span class="sxs-lookup"><span data-stu-id="c72ff-112">The previous name of the item.</span></span>
| <span data-ttu-id="c72ff-113">newName</span><span class="sxs-lookup"><span data-stu-id="c72ff-113">newName</span></span>       | <span data-ttu-id="c72ff-114">string</span><span class="sxs-lookup"><span data-stu-id="c72ff-114">string</span></span> | <span data-ttu-id="c72ff-115">アイテムの新しい名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="c72ff-115">The new name of the item.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c72ff-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c72ff-116">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.renameAction"
}-->

```json
{
  "oldName": "string",
  "newName": "string"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "The renameAction object provides information about an activity that renamed an item.",
  "keywords": "activities,activity,action,rename,renamed",
  "section": "documentation",
  "tocPath": "Resources/renameAction",
  "suppressions": []
}
-->
