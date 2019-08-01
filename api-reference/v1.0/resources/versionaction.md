---
author: daspek
ms.author: dspektor
title: versionAction リソースの種類
description: VersionAction オブジェクトは、新しいアイテムバージョンが発生したアクティビティに関する情報を提供します。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 22f06691824d2ffa5b773a796b4c456cb2fcaecc
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033447"
---
# <a name="versionaction-resource-type"></a><span data-ttu-id="23849-103">versionAction リソースの種類</span><span class="sxs-lookup"><span data-stu-id="23849-103">versionAction resource type</span></span>

<span data-ttu-id="23849-104">[**Itemactivity**][activity]に**versionaction**リソースがある場合、アクティビティが新しいバージョンの作成を引き起こしたことを示します。</span><span class="sxs-lookup"><span data-stu-id="23849-104">The presence of the **versionAction** resource on an [**itemActivity**][activity] indicates that the activity caused a new version to be created.</span></span>

><span data-ttu-id="23849-105">**注:** 現時点では、アイテムアクティビティレコードは SharePoint および OneDrive for business でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="23849-105">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="23849-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="23849-106">Properties</span></span>

| <span data-ttu-id="23849-107">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="23849-107">Property name</span></span> | <span data-ttu-id="23849-108">種類</span><span class="sxs-lookup"><span data-stu-id="23849-108">Type</span></span>   | <span data-ttu-id="23849-109">説明</span><span class="sxs-lookup"><span data-stu-id="23849-109">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="23849-110">newVersion</span><span class="sxs-lookup"><span data-stu-id="23849-110">newVersion</span></span>    | <span data-ttu-id="23849-111">string</span><span class="sxs-lookup"><span data-stu-id="23849-111">string</span></span> | <span data-ttu-id="23849-112">このアクションによって作成された新しいバージョンの名前。</span><span class="sxs-lookup"><span data-stu-id="23849-112">The name of the new version that was created by this action.</span></span>

## <a name="json-representation"></a><span data-ttu-id="23849-113">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="23849-113">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.versionAction"
}-->

```json
{
  "newVersion": "string"
}
```

<!--
{
  "type": "#page.annotation",
  "description": "The VersionAction object provides information about an activity that resulted in a new item version.",
  "keywords": "activities,activity,action,version",
  "section": "documentation",
  "tocPath": "Resources/VersionAction",
  "suppressions": []
}
-->
