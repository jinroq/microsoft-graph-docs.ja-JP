---
author: daspek
ms.author: dspektor
title: mentionAction リソースの種類
description: MentionAction オブジェクトは、活動中に説明されたユーザーに関する情報を提供します。
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 511519439f4079b2d7d618767855582f201c00f7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036184"
---
# <a name="mentionaction-resource-type"></a><span data-ttu-id="9dc38-103">mentionAction リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9dc38-103">mentionAction resource type</span></span>

<span data-ttu-id="9dc38-104">**MentionAction** リソースは、ユーザーについて記載した[アクティビティ][]に関する情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="9dc38-104">The **MentionAction** resource provides information about an [activity][] that mentioned people.</span></span>

><span data-ttu-id="9dc38-105">**注:** 現時点では、アイテムアクティビティレコードは SharePoint および OneDrive for business でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="9dc38-105">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[アクティビティ]: itemactivity.md
[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="9dc38-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9dc38-107">Properties</span></span>

| <span data-ttu-id="9dc38-108">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="9dc38-108">Property name</span></span> | <span data-ttu-id="9dc38-109">種類</span><span class="sxs-lookup"><span data-stu-id="9dc38-109">Type</span></span>                       | <span data-ttu-id="9dc38-110">説明</span><span class="sxs-lookup"><span data-stu-id="9dc38-110">Description</span></span>
|:--------------|:---------------------------|:-----------------------------
| <span data-ttu-id="9dc38-111">mentionees</span><span class="sxs-lookup"><span data-stu-id="9dc38-111">mentionees</span></span>    | <span data-ttu-id="9dc38-112">[identitySet][] コレクション</span><span class="sxs-lookup"><span data-stu-id="9dc38-112">[identitySet][] collection</span></span> | <span data-ttu-id="9dc38-113">このアクションに記載されているユーザーの ID。</span><span class="sxs-lookup"><span data-stu-id="9dc38-113">The identities of the users mentioned in this action.</span></span>

[identitySet]: identityset.md

## <a name="json-representation"></a><span data-ttu-id="9dc38-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9dc38-115">JSON representation</span></span>

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
