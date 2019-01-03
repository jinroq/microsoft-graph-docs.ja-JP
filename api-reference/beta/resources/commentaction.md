---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: CommentAction
ms.openlocfilehash: 92dc26945cd591de2ba107907a593159f1e128c9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27074163"
---
# <a name="commentaction-resource-type"></a><span data-ttu-id="08905-102">CommentAction リソースの種類</span><span class="sxs-lookup"><span data-stu-id="08905-102">CommentAction resource type</span></span>

> <span data-ttu-id="08905-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="08905-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="08905-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="08905-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="08905-105">**CommentAction**リソースは、アイテムに対して行われたコメント [アクティビティ][]に関する情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="08905-105">The **CommentAction** resource provides information about a comment [activity][] made on an item.</span></span>

[アクティビティ]: itemactivity.md
[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="08905-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="08905-107">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="08905-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="08905-108">Properties</span></span>

| <span data-ttu-id="08905-109">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="08905-109">Property name</span></span>    | <span data-ttu-id="08905-110">型</span><span class="sxs-lookup"><span data-stu-id="08905-110">Type</span></span>                       | <span data-ttu-id="08905-111">説明</span><span class="sxs-lookup"><span data-stu-id="08905-111">Description</span></span>
|:-----------------|:---------------------------|:-----------------------------
| <span data-ttu-id="08905-112">isReply</span><span class="sxs-lookup"><span data-stu-id="08905-112">isReply</span></span>          | <span data-ttu-id="08905-113">boolean</span><span class="sxs-lookup"><span data-stu-id="08905-113">boolean</span></span>                    | <span data-ttu-id="08905-114">true の場合、このアクティビティは既存のコメント スレッドへの返信だったことを示します。</span><span class="sxs-lookup"><span data-stu-id="08905-114">If true, this activity was a reply to an existing comment thread.</span></span>
| <span data-ttu-id="08905-115">parentAuthor</span><span class="sxs-lookup"><span data-stu-id="08905-115">parentAuthor</span></span>     | <span data-ttu-id="08905-116">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="08905-116">[identitySet][]</span></span>            | <span data-ttu-id="08905-117">コメント スレッドを開始したユーザーの ID。</span><span class="sxs-lookup"><span data-stu-id="08905-117">The identity of the user who started the comment thread.</span></span>
| <span data-ttu-id="08905-118">participants</span><span class="sxs-lookup"><span data-stu-id="08905-118">participants</span></span>     | <span data-ttu-id="08905-119">[identitySet][] コレクション</span><span class="sxs-lookup"><span data-stu-id="08905-119">[identitySet][] collection</span></span> | <span data-ttu-id="08905-120">該当のコメント スレッドに参加しているユーザーの ID。</span><span class="sxs-lookup"><span data-stu-id="08905-120">The identities of the users participating in this comment thread.</span></span>

[identitySet]: identityset.md

## <a name="remarks"></a><span data-ttu-id="08905-122">備考</span><span class="sxs-lookup"><span data-stu-id="08905-122">Remarks</span></span>

<span data-ttu-id="08905-123">アイテムのアクティビティの記録は、現在、SharePoint と OneDrive for Business でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="08905-123">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!-- {
  "type": "#page.annotation",
  "description": "The CommentAction object provides information about a comment that was made on an item.",
  "keywords": "activities,activity,action,comment",
  "section": "documentation",
  "tocPath": "Resources/CommentAction"
} -->