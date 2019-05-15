---
author: daspek
ms.author: dspektor
title: コメントアクションリソースの種類
description: Comment アクションオブジェクトは、アイテムに対して行われたコメントについての情報を提供します。
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 12e6cd68d5809b8e4c1765234eeb77b40b30a78e
ms.sourcegitcommit: 52baf24d1d08096214b12f60e7c755291fe03ab5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/13/2019
ms.locfileid: "33970749"
---
# <a name="commentaction-resource-type"></a><span data-ttu-id="c0cfe-103">コメントアクションリソースの種類</span><span class="sxs-lookup"><span data-stu-id="c0cfe-103">commentAction resource type</span></span>

<span data-ttu-id="c0cfe-104">**Comment アクション**リソースは、アイテムに対して行われたコメント[アクティビティ][]に関する情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="c0cfe-104">The **commentAction** resource provides information about a comment [activity][] made on an item.</span></span>

><span data-ttu-id="c0cfe-105">**注:** 現時点では、アイテムアクティビティレコードは SharePoint および OneDrive for business でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="c0cfe-105">**Note:** Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

[アクティビティ]: itemactivity.md
[activity]: itemactivity.md

## <a name="properties"></a><span data-ttu-id="c0cfe-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c0cfe-107">Properties</span></span>

| <span data-ttu-id="c0cfe-108">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="c0cfe-108">Property name</span></span>    | <span data-ttu-id="c0cfe-109">種類</span><span class="sxs-lookup"><span data-stu-id="c0cfe-109">Type</span></span>                       | <span data-ttu-id="c0cfe-110">説明</span><span class="sxs-lookup"><span data-stu-id="c0cfe-110">Description</span></span>
|:-----------------|:---------------------------|:-----------------------------
| <span data-ttu-id="c0cfe-111">isReply</span><span class="sxs-lookup"><span data-stu-id="c0cfe-111">isReply</span></span>          | <span data-ttu-id="c0cfe-112">boolean</span><span class="sxs-lookup"><span data-stu-id="c0cfe-112">boolean</span></span>                    | <span data-ttu-id="c0cfe-113">true の場合、このアクティビティは既存のコメント スレッドへの返信だったことを示します。</span><span class="sxs-lookup"><span data-stu-id="c0cfe-113">If true, this activity was a reply to an existing comment thread.</span></span>
| <span data-ttu-id="c0cfe-114">parentAuthor</span><span class="sxs-lookup"><span data-stu-id="c0cfe-114">parentAuthor</span></span>     | <span data-ttu-id="c0cfe-115">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="c0cfe-115">[identitySet][]</span></span>            | <span data-ttu-id="c0cfe-116">コメント スレッドを開始したユーザーの ID。</span><span class="sxs-lookup"><span data-stu-id="c0cfe-116">The identity of the user who started the comment thread.</span></span>
| <span data-ttu-id="c0cfe-117">participants</span><span class="sxs-lookup"><span data-stu-id="c0cfe-117">participants</span></span>     | <span data-ttu-id="c0cfe-118">[identitySet][] コレクション</span><span class="sxs-lookup"><span data-stu-id="c0cfe-118">[identitySet][] collection</span></span> | <span data-ttu-id="c0cfe-119">該当のコメント スレッドに参加しているユーザーの ID。</span><span class="sxs-lookup"><span data-stu-id="c0cfe-119">The identities of the users participating in this comment thread.</span></span>

[identitySet]: identityset.md

## <a name="json-representation"></a><span data-ttu-id="c0cfe-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c0cfe-121">JSON representation</span></span>

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
