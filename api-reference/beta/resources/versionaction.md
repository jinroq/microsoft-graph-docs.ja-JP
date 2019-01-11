---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: VersionAction
localization_priority: Normal
ms.openlocfilehash: 1f315b26c45e337986784200fb6ec2c78612344b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27866711"
---
# <a name="versionaction-resource-type"></a><span data-ttu-id="2de48-102">VersionAction リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2de48-102">VersionAction resource type</span></span>

> <span data-ttu-id="2de48-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2de48-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2de48-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2de48-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2de48-105">[**itemActivity**][activity] に **VersionAction** リソースがある場合、アクティビティが新しいバージョンの作成を引き起こしたことを示します。</span><span class="sxs-lookup"><span data-stu-id="2de48-105">The presence of the **VersionAction** resource on an [**itemActivity**][activity] indicates that the activity caused a new version to be created.</span></span>

[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="2de48-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2de48-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="2de48-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2de48-107">Properties</span></span>

| <span data-ttu-id="2de48-108">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="2de48-108">Property name</span></span> | <span data-ttu-id="2de48-109">Type</span><span class="sxs-lookup"><span data-stu-id="2de48-109">Type</span></span>   | <span data-ttu-id="2de48-110">説明</span><span class="sxs-lookup"><span data-stu-id="2de48-110">Description</span></span>
|:--------------|:-------|:----------------------------------------------------
| <span data-ttu-id="2de48-111">newVersion</span><span class="sxs-lookup"><span data-stu-id="2de48-111">newVersion</span></span>    | <span data-ttu-id="2de48-112">文字列</span><span class="sxs-lookup"><span data-stu-id="2de48-112">string</span></span> | <span data-ttu-id="2de48-113">このアクションによって作成された新しいバージョンの名前。</span><span class="sxs-lookup"><span data-stu-id="2de48-113">The name of the new version that was created by this action.</span></span>

## <a name="remarks"></a><span data-ttu-id="2de48-114">備考</span><span class="sxs-lookup"><span data-stu-id="2de48-114">Remarks</span></span>

<span data-ttu-id="2de48-115">アイテムのアクティビティの記録は、現在、SharePoint と OneDrive for Business でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="2de48-115">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The VersionAction object provides information about an activity that resulted in a new item version.",
  "keywords": "activities,activity,action,version",
  "section": "documentation",
  "tocPath": "Resources/VersionAction"
} -->
