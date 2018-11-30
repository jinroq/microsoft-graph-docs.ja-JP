---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: MentionAction
ms.openlocfilehash: be873ba2b5f9bc1fdd387407c1036435dc6f1fc7
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069596"
---
# <a name="mentionaction-resource-type"></a><span data-ttu-id="fd620-102">MentionAction リソースの種類</span><span class="sxs-lookup"><span data-stu-id="fd620-102">MentionAction resource type</span></span>

> <span data-ttu-id="fd620-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="fd620-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fd620-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fd620-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fd620-105">**MentionAction** リソースは、ユーザーについて記載した[アクティビティ][]に関する情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="fd620-105">The **MentionAction** resource provides information about an [activity][] that mentioned people.</span></span>

[アクティビティ]: itemactivity.md
[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="fd620-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fd620-107">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="fd620-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fd620-108">Properties</span></span>

| <span data-ttu-id="fd620-109">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="fd620-109">Property name</span></span> | <span data-ttu-id="fd620-110">型</span><span class="sxs-lookup"><span data-stu-id="fd620-110">Type</span></span>                       | <span data-ttu-id="fd620-111">説明</span><span class="sxs-lookup"><span data-stu-id="fd620-111">Description</span></span>
|:--------------|:---------------------------|:-----------------------------
| <span data-ttu-id="fd620-112">mentionees</span><span class="sxs-lookup"><span data-stu-id="fd620-112">mentionees</span></span>    | <span data-ttu-id="fd620-113">[identitySet][] コレクション</span><span class="sxs-lookup"><span data-stu-id="fd620-113">[identitySet][] collection</span></span> | <span data-ttu-id="fd620-114">このアクションに記載されているユーザーの ID。</span><span class="sxs-lookup"><span data-stu-id="fd620-114">The identities of the users mentioned in this action.</span></span>

[identitySet]: identityset.md

## <a name="remarks"></a><span data-ttu-id="fd620-116">備考</span><span class="sxs-lookup"><span data-stu-id="fd620-116">Remarks</span></span>

<span data-ttu-id="fd620-117">アイテムのアクティビティの記録は、現在、SharePoint と OneDrive for Business でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="fd620-117">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The MentionAction object provides information about who was mentioned during an activity.",
  "keywords": "activities,activity,action,mention",
  "section": "documentation",
  "tocPath": "Resources/MentionAction"
} -->
