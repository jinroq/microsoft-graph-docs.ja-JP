---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: MentionAction
localization_priority: Normal
ms.openlocfilehash: 7843feebd8ebca2022b276007d21a89b754217a0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27804971"
---
# <a name="mentionaction-resource-type"></a><span data-ttu-id="e8acc-102">MentionAction リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e8acc-102">MentionAction resource type</span></span>

> <span data-ttu-id="e8acc-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e8acc-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e8acc-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e8acc-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="e8acc-105">**MentionAction** リソースは、ユーザーについて記載した[アクティビティ][]に関する情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="e8acc-105">The **MentionAction** resource provides information about an [activity][] that mentioned people.</span></span>

[アクティビティ]: itemactivity.md
[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="e8acc-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e8acc-107">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.mentionAction"
}-->

```json
{
  "mentionees": [{"@odata.type": "microsoft.graph.identitySet"}]
}
```

## <a name="properties"></a><span data-ttu-id="e8acc-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e8acc-108">Properties</span></span>

| <span data-ttu-id="e8acc-109">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="e8acc-109">Property name</span></span> | <span data-ttu-id="e8acc-110">Type</span><span class="sxs-lookup"><span data-stu-id="e8acc-110">Type</span></span>                       | <span data-ttu-id="e8acc-111">説明</span><span class="sxs-lookup"><span data-stu-id="e8acc-111">Description</span></span>
|:--------------|:---------------------------|:-----------------------------
| <span data-ttu-id="e8acc-112">mentionees</span><span class="sxs-lookup"><span data-stu-id="e8acc-112">mentionees</span></span>    | <span data-ttu-id="e8acc-113">[identitySet][] コレクション</span><span class="sxs-lookup"><span data-stu-id="e8acc-113">[identitySet][] collection</span></span> | <span data-ttu-id="e8acc-114">このアクションに記載されているユーザーの ID。</span><span class="sxs-lookup"><span data-stu-id="e8acc-114">The identities of the users mentioned in this action.</span></span>

[identitySet]: identityset.md

## <a name="remarks"></a><span data-ttu-id="e8acc-116">備考</span><span class="sxs-lookup"><span data-stu-id="e8acc-116">Remarks</span></span>

<span data-ttu-id="e8acc-117">アイテムのアクティビティの記録は、現在、SharePoint と OneDrive for Business でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="e8acc-117">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The MentionAction object provides information about who was mentioned during an activity.",
  "keywords": "activities,activity,action,mention",
  "section": "documentation",
  "tocPath": "Resources/MentionAction"
} -->
