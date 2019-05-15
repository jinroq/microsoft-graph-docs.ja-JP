---
author: daspek
ms.author: dspektor
title: mentionAction リソースの種類
description: MentionAction オブジェクトは、活動中に説明されたユーザーに関する情報を提供します。
localization_priority: Normal
ms.prod: insights
ms.openlocfilehash: d8c09de2a36be2cd83d5e33cf2ed948c25819fe4
ms.sourcegitcommit: 52baf24d1d08096214b12f60e7c755291fe03ab5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/13/2019
ms.locfileid: "33970778"
---
# <a name="mentionaction-resource-type"></a><span data-ttu-id="f8b90-103">mentionAction リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f8b90-103">mentionAction resource type</span></span>

<span data-ttu-id="f8b90-104">**MentionAction** リソースは、ユーザーについて記載した[アクティビティ][]に関する情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="f8b90-104">The **MentionAction** resource provides information about an [activity][] that mentioned people.</span></span>

><span data-ttu-id="f8b90-105">**注:** 現時点では、アイテムアクティビティレコードは SharePoint および OneDrive for business でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="f8b90-105">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[アクティビティ]: itemactivity.md
[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="f8b90-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f8b90-107">Properties</span></span>

| <span data-ttu-id="f8b90-108">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="f8b90-108">Property name</span></span> | <span data-ttu-id="f8b90-109">種類</span><span class="sxs-lookup"><span data-stu-id="f8b90-109">Type</span></span>                       | <span data-ttu-id="f8b90-110">説明</span><span class="sxs-lookup"><span data-stu-id="f8b90-110">Description</span></span>
|:--------------|:---------------------------|:-----------------------------
| <span data-ttu-id="f8b90-111">mentionees</span><span class="sxs-lookup"><span data-stu-id="f8b90-111">mentionees</span></span>    | <span data-ttu-id="f8b90-112">[identitySet][] コレクション</span><span class="sxs-lookup"><span data-stu-id="f8b90-112">[identitySet][] collection</span></span> | <span data-ttu-id="f8b90-113">このアクションに記載されているユーザーの ID。</span><span class="sxs-lookup"><span data-stu-id="f8b90-113">The identities of the users mentioned in this action.</span></span>

[identitySet]: identityset.md

## <a name="json-representation"></a><span data-ttu-id="f8b90-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f8b90-115">JSON representation</span></span>

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

<!--
{
  "type": "#page.annotation",
  "description": "The MentionAction object provides information about who was mentioned during an activity.",
  "keywords": "activities,activity,action,mention",
  "section": "documentation",
  "tocPath": "Resources/MentionAction",
  "suppressions": []
}
-->
