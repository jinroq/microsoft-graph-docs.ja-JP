---
author: daspek
description: itemActivity に VersionAction リソースがある場合、アクティビティが新しいバージョンの作成を引き起こしたことを示します。
ms.date: 09/14/2017
title: VersionAction
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 8eeec313ac4ed901d7552e2ad65d02edcaa821cd
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36007397"
---
# <a name="versionaction-resource-type"></a><span data-ttu-id="0cda9-103">VersionAction リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0cda9-103">VersionAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0cda9-104">[**itemActivity**][activity] に **VersionAction** リソースがある場合、アクティビティが新しいバージョンの作成を引き起こしたことを示します。</span><span class="sxs-lookup"><span data-stu-id="0cda9-104">The presence of the **VersionAction** resource on an [**itemActivity**][activity] indicates that the activity caused a new version to be created.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="0cda9-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0cda9-105">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="0cda9-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0cda9-106">Properties</span></span>

| <span data-ttu-id="0cda9-107">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="0cda9-107">Property name</span></span> | <span data-ttu-id="0cda9-108">種類</span><span class="sxs-lookup"><span data-stu-id="0cda9-108">Type</span></span>   | <span data-ttu-id="0cda9-109">説明</span><span class="sxs-lookup"><span data-stu-id="0cda9-109">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="0cda9-110">newVersion</span><span class="sxs-lookup"><span data-stu-id="0cda9-110">newVersion</span></span>    | <span data-ttu-id="0cda9-111">string</span><span class="sxs-lookup"><span data-stu-id="0cda9-111">string</span></span> | <span data-ttu-id="0cda9-112">このアクションによって作成された新しいバージョンの名前。</span><span class="sxs-lookup"><span data-stu-id="0cda9-112">The name of the new version that was created by this action.</span></span>

## <a name="remarks"></a><span data-ttu-id="0cda9-113">備考</span><span class="sxs-lookup"><span data-stu-id="0cda9-113">Remarks</span></span>

<span data-ttu-id="0cda9-114">アイテムのアクティビティの記録は、現在、SharePoint と OneDrive for Business でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="0cda9-114">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

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
