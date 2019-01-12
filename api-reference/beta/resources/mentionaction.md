---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: MentionAction
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: 48ac49c80a39fd6bc51b048a8eb7dab6e62da810
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27974141"
---
# <a name="mentionaction-resource-type"></a><span data-ttu-id="02541-102">MentionAction リソースの種類</span><span class="sxs-lookup"><span data-stu-id="02541-102">MentionAction resource type</span></span>

> <span data-ttu-id="02541-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="02541-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="02541-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="02541-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="02541-105">**MentionAction** リソースは、ユーザーについて記載した[アクティビティ][]に関する情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="02541-105">The **MentionAction** resource provides information about an [activity][] that mentioned people.</span></span>

[アクティビティ]: itemactivity.md
[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="02541-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="02541-107">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="02541-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="02541-108">Properties</span></span>

| <span data-ttu-id="02541-109">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="02541-109">Property name</span></span> | <span data-ttu-id="02541-110">Type</span><span class="sxs-lookup"><span data-stu-id="02541-110">Type</span></span>                       | <span data-ttu-id="02541-111">説明</span><span class="sxs-lookup"><span data-stu-id="02541-111">Description</span></span>
|:--------------|:---------------------------|:-----------------------------
| <span data-ttu-id="02541-112">mentionees</span><span class="sxs-lookup"><span data-stu-id="02541-112">mentionees</span></span>    | <span data-ttu-id="02541-113">[identitySet][] コレクション</span><span class="sxs-lookup"><span data-stu-id="02541-113">[identitySet][] collection</span></span> | <span data-ttu-id="02541-114">このアクションに記載されているユーザーの ID。</span><span class="sxs-lookup"><span data-stu-id="02541-114">The identities of the users mentioned in this action.</span></span>

[identitySet]: identityset.md

## <a name="remarks"></a><span data-ttu-id="02541-116">備考</span><span class="sxs-lookup"><span data-stu-id="02541-116">Remarks</span></span>

<span data-ttu-id="02541-117">アイテムのアクティビティの記録は、現在、SharePoint と OneDrive for Business でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="02541-117">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The MentionAction object provides information about who was mentioned during an activity.",
  "keywords": "activities,activity,action,mention",
  "section": "documentation",
  "tocPath": "Resources/MentionAction"
} -->
