---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: CommentAction
localization_priority: Normal
ms.openlocfilehash: c472a0b1b992c91b60174859e4900ffcee04c007
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33341482"
---
# <a name="commentaction-resource-type"></a><span data-ttu-id="fc9e9-102">CommentAction リソースの種類</span><span class="sxs-lookup"><span data-stu-id="fc9e9-102">CommentAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fc9e9-103">**CommentAction**リソースは、アイテムに対して行われたコメント [アクティビティ][]に関する情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="fc9e9-103">The **CommentAction** resource provides information about a comment [activity][] made on an item.</span></span>

[アクティビティ]: itemactivity.md
[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="fc9e9-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fc9e9-105">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [ ],
  "@type": "microsoft.graph.commentAction"
}-->

```json
{
  "isReply": false,
  "parentAuthor": {"@odata.type": "microsoft.graph.identitySet"},
  "participants": [{"@odata.type": "microsoft.graph.identitySet"}]
}
```

## <a name="properties"></a><span data-ttu-id="fc9e9-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fc9e9-106">Properties</span></span>

| <span data-ttu-id="fc9e9-107">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="fc9e9-107">Property name</span></span>    | <span data-ttu-id="fc9e9-108">種類</span><span class="sxs-lookup"><span data-stu-id="fc9e9-108">Type</span></span>                       | <span data-ttu-id="fc9e9-109">説明</span><span class="sxs-lookup"><span data-stu-id="fc9e9-109">Description</span></span>
|:-----------------|:---------------------------|:-----------------------------
| <span data-ttu-id="fc9e9-110">isReply</span><span class="sxs-lookup"><span data-stu-id="fc9e9-110">isReply</span></span>          | <span data-ttu-id="fc9e9-111">boolean</span><span class="sxs-lookup"><span data-stu-id="fc9e9-111">boolean</span></span>                    | <span data-ttu-id="fc9e9-112">true の場合、このアクティビティは既存のコメント スレッドへの返信だったことを示します。</span><span class="sxs-lookup"><span data-stu-id="fc9e9-112">If true, this activity was a reply to an existing comment thread.</span></span>
| <span data-ttu-id="fc9e9-113">parentAuthor</span><span class="sxs-lookup"><span data-stu-id="fc9e9-113">parentAuthor</span></span>     | <span data-ttu-id="fc9e9-114">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="fc9e9-114">[identitySet][]</span></span>            | <span data-ttu-id="fc9e9-115">コメント スレッドを開始したユーザーの ID。</span><span class="sxs-lookup"><span data-stu-id="fc9e9-115">The identity of the user who started the comment thread.</span></span>
| <span data-ttu-id="fc9e9-116">participants</span><span class="sxs-lookup"><span data-stu-id="fc9e9-116">participants</span></span>     | <span data-ttu-id="fc9e9-117">[identitySet][] コレクション</span><span class="sxs-lookup"><span data-stu-id="fc9e9-117">[identitySet][] collection</span></span> | <span data-ttu-id="fc9e9-118">該当のコメント スレッドに参加しているユーザーの ID。</span><span class="sxs-lookup"><span data-stu-id="fc9e9-118">The identities of the users participating in this comment thread.</span></span>

[identitySet]: identityset.md

## <a name="remarks"></a><span data-ttu-id="fc9e9-120">備考</span><span class="sxs-lookup"><span data-stu-id="fc9e9-120">Remarks</span></span>

<span data-ttu-id="fc9e9-121">アイテムのアクティビティの記録は、現在、SharePoint と OneDrive for Business でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="fc9e9-121">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The CommentAction object provides information about a comment that was made on an item.",
  "keywords": "activities,activity,action,comment",
  "section": "documentation",
  "tocPath": "Resources/CommentAction",
  "suppressions": []
}
-->
