---
author: daspek
description: CommentActionリソースは、アイテムに対して行われたコメント アクティビティに関する情報を提供します。
ms.date: 09/14/2017
title: CommentAction
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: b7782c6e4dd30b503a9be88737ef6bd2dbad109b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35973259"
---
# <a name="commentaction-resource-type"></a><span data-ttu-id="4334c-103">CommentAction リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4334c-103">CommentAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4334c-104">**CommentAction**リソースは、アイテムに対して行われたコメント [アクティビティ][]に関する情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="4334c-104">The **CommentAction** resource provides information about a comment [activity][] made on an item.</span></span>

[アクティビティ]: itemactivity.md
[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="4334c-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4334c-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="4334c-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4334c-107">Properties</span></span>

| <span data-ttu-id="4334c-108">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="4334c-108">Property name</span></span>    | <span data-ttu-id="4334c-109">種類</span><span class="sxs-lookup"><span data-stu-id="4334c-109">Type</span></span>                       | <span data-ttu-id="4334c-110">説明</span><span class="sxs-lookup"><span data-stu-id="4334c-110">Description</span></span>
|:-----------------|:---------------------------|:-----------------------------
| <span data-ttu-id="4334c-111">isReply</span><span class="sxs-lookup"><span data-stu-id="4334c-111">isReply</span></span>          | <span data-ttu-id="4334c-112">boolean</span><span class="sxs-lookup"><span data-stu-id="4334c-112">boolean</span></span>                    | <span data-ttu-id="4334c-113">true の場合、このアクティビティは既存のコメント スレッドへの返信だったことを示します。</span><span class="sxs-lookup"><span data-stu-id="4334c-113">If true, this activity was a reply to an existing comment thread.</span></span>
| <span data-ttu-id="4334c-114">parentAuthor</span><span class="sxs-lookup"><span data-stu-id="4334c-114">parentAuthor</span></span>     | <span data-ttu-id="4334c-115">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="4334c-115">[identitySet][]</span></span>            | <span data-ttu-id="4334c-116">コメント スレッドを開始したユーザーの ID。</span><span class="sxs-lookup"><span data-stu-id="4334c-116">The identity of the user who started the comment thread.</span></span>
| <span data-ttu-id="4334c-117">participants</span><span class="sxs-lookup"><span data-stu-id="4334c-117">participants</span></span>     | <span data-ttu-id="4334c-118">[identitySet][] コレクション</span><span class="sxs-lookup"><span data-stu-id="4334c-118">[identitySet][] collection</span></span> | <span data-ttu-id="4334c-119">該当のコメント スレッドに参加しているユーザーの ID。</span><span class="sxs-lookup"><span data-stu-id="4334c-119">The identities of the users participating in this comment thread.</span></span>

[identitySet]: identityset.md

## <a name="remarks"></a><span data-ttu-id="4334c-121">備考</span><span class="sxs-lookup"><span data-stu-id="4334c-121">Remarks</span></span>

<span data-ttu-id="4334c-122">アイテムのアクティビティの記録は、現在、SharePoint と OneDrive for Business でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="4334c-122">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

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
