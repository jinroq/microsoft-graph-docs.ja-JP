---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: VersionAction
localization_priority: Normal
ms.openlocfilehash: 59977b4ad84615f72dc008d671d64c62a2f4960f
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345058"
---
# <a name="versionaction-resource-type"></a><span data-ttu-id="8fb6b-102">VersionAction リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8fb6b-102">VersionAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8fb6b-103">[**itemActivity**][activity] に **VersionAction** リソースがある場合、アクティビティが新しいバージョンの作成を引き起こしたことを示します。</span><span class="sxs-lookup"><span data-stu-id="8fb6b-103">The presence of the **VersionAction** resource on an [**itemActivity**][activity] indicates that the activity caused a new version to be created.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="8fb6b-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8fb6b-104">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="8fb6b-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8fb6b-105">Properties</span></span>

| <span data-ttu-id="8fb6b-106">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="8fb6b-106">Property name</span></span> | <span data-ttu-id="8fb6b-107">種類</span><span class="sxs-lookup"><span data-stu-id="8fb6b-107">Type</span></span>   | <span data-ttu-id="8fb6b-108">説明</span><span class="sxs-lookup"><span data-stu-id="8fb6b-108">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="8fb6b-109">newVersion</span><span class="sxs-lookup"><span data-stu-id="8fb6b-109">newVersion</span></span>    | <span data-ttu-id="8fb6b-110">string</span><span class="sxs-lookup"><span data-stu-id="8fb6b-110">string</span></span> | <span data-ttu-id="8fb6b-111">このアクションによって作成された新しいバージョンの名前。</span><span class="sxs-lookup"><span data-stu-id="8fb6b-111">The name of the new version that was created by this action.</span></span>

## <a name="remarks"></a><span data-ttu-id="8fb6b-112">備考</span><span class="sxs-lookup"><span data-stu-id="8fb6b-112">Remarks</span></span>

<span data-ttu-id="8fb6b-113">アイテムのアクティビティの記録は、現在、SharePoint と OneDrive for Business でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="8fb6b-113">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

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
