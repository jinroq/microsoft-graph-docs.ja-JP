---
author: daspek
description: MentionAction リソースは、ユーザーについて記載したアクティビティに関する情報を提供します。
ms.date: 09/14/2017
title: MentionAction
localization_priority: Normal
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 1b08233569fe655b5a8f0e878c4e14d178be279f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966819"
---
# <a name="mentionaction-resource-type"></a><span data-ttu-id="63d71-103">MentionAction リソースの種類</span><span class="sxs-lookup"><span data-stu-id="63d71-103">MentionAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="63d71-104">**MentionAction** リソースは、ユーザーについて記載した[アクティビティ][]に関する情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="63d71-104">The **MentionAction** resource provides information about an [activity][] that mentioned people.</span></span>

[アクティビティ]: itemactivity.md
[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="63d71-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="63d71-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="63d71-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="63d71-107">Properties</span></span>

| <span data-ttu-id="63d71-108">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="63d71-108">Property name</span></span> | <span data-ttu-id="63d71-109">種類</span><span class="sxs-lookup"><span data-stu-id="63d71-109">Type</span></span>                       | <span data-ttu-id="63d71-110">説明</span><span class="sxs-lookup"><span data-stu-id="63d71-110">Description</span></span>
|:--------------|:---------------------------|:-----------------------------
| <span data-ttu-id="63d71-111">mentionees</span><span class="sxs-lookup"><span data-stu-id="63d71-111">mentionees</span></span>    | <span data-ttu-id="63d71-112">[identitySet][] コレクション</span><span class="sxs-lookup"><span data-stu-id="63d71-112">[identitySet][] collection</span></span> | <span data-ttu-id="63d71-113">このアクションに記載されているユーザーの ID。</span><span class="sxs-lookup"><span data-stu-id="63d71-113">The identities of the users mentioned in this action.</span></span>

[identitySet]: identityset.md

## <a name="remarks"></a><span data-ttu-id="63d71-115">備考</span><span class="sxs-lookup"><span data-stu-id="63d71-115">Remarks</span></span>

<span data-ttu-id="63d71-116">アイテムのアクティビティの記録は、現在、SharePoint と OneDrive for Business でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="63d71-116">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

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
