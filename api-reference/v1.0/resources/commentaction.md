---
author: daspek
ms.author: dspektor
title: コメントアクションリソースの種類
description: Comment アクションオブジェクトは、アイテムに対して行われたコメントについての情報を提供します。
localization_priority: Normal
ms.prod: sharepoint
doc_type: resourcePageType
ms.openlocfilehash: 72502e466ff90ec0a299eb993346968c9038e2d1
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029681"
---
# <a name="commentaction-resource-type"></a><span data-ttu-id="6fb7b-103">コメントアクションリソースの種類</span><span class="sxs-lookup"><span data-stu-id="6fb7b-103">commentAction resource type</span></span>

<span data-ttu-id="6fb7b-104">**Comment アクション**リソースは、アイテムに対して行われたコメント[アクティビティ][]に関する情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="6fb7b-104">The **commentAction** resource provides information about a comment [activity][] made on an item.</span></span>

><span data-ttu-id="6fb7b-105">**注:** 現時点では、アイテムアクティビティレコードは SharePoint および OneDrive for business でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="6fb7b-105">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[アクティビティ]: itemactivity.md
[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="6fb7b-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6fb7b-107">Properties</span></span>

| <span data-ttu-id="6fb7b-108">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="6fb7b-108">Property name</span></span>    | <span data-ttu-id="6fb7b-109">種類</span><span class="sxs-lookup"><span data-stu-id="6fb7b-109">Type</span></span>                       | <span data-ttu-id="6fb7b-110">説明</span><span class="sxs-lookup"><span data-stu-id="6fb7b-110">Description</span></span>
|:-----------------|:---------------------------|:-----------------------------
| <span data-ttu-id="6fb7b-111">isReply</span><span class="sxs-lookup"><span data-stu-id="6fb7b-111">isReply</span></span>          | <span data-ttu-id="6fb7b-112">boolean</span><span class="sxs-lookup"><span data-stu-id="6fb7b-112">boolean</span></span>                    | <span data-ttu-id="6fb7b-113">true の場合、このアクティビティは既存のコメント スレッドへの返信だったことを示します。</span><span class="sxs-lookup"><span data-stu-id="6fb7b-113">If true, this activity was a reply to an existing comment thread.</span></span>
| <span data-ttu-id="6fb7b-114">parentAuthor</span><span class="sxs-lookup"><span data-stu-id="6fb7b-114">parentAuthor</span></span>     | <span data-ttu-id="6fb7b-115">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="6fb7b-115">[identitySet][]</span></span>            | <span data-ttu-id="6fb7b-116">コメント スレッドを開始したユーザーの ID。</span><span class="sxs-lookup"><span data-stu-id="6fb7b-116">The identity of the user who started the comment thread.</span></span>
| <span data-ttu-id="6fb7b-117">participants</span><span class="sxs-lookup"><span data-stu-id="6fb7b-117">participants</span></span>     | <span data-ttu-id="6fb7b-118">[identitySet][] コレクション</span><span class="sxs-lookup"><span data-stu-id="6fb7b-118">[identitySet][] collection</span></span> | <span data-ttu-id="6fb7b-119">該当のコメント スレッドに参加しているユーザーの ID。</span><span class="sxs-lookup"><span data-stu-id="6fb7b-119">The identities of the users participating in this comment thread.</span></span>

[identitySet]: identityset.md

## <a name="json-representation"></a><span data-ttu-id="6fb7b-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6fb7b-121">JSON representation</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "The commentAction object provides information about a comment that was made on an item.",
  "keywords": "activities,activity,action,comment",
  "section": "documentation",
  "tocPath": "Resources/commentAction",
  "suppressions": []
}
-->
