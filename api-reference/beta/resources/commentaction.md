---
author: daspek
ms.author: dspektor
ms.date: 09/14/2017
title: CommentAction
localization_priority: Normal
ms.openlocfilehash: e674c996002b3a54c92886dd1c5dca7a76c56b51
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32543463"
---
# <a name="commentaction-resource-type"></a><span data-ttu-id="b35ae-102">CommentAction リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b35ae-102">CommentAction resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b35ae-103">**CommentAction**リソースは、アイテムに対して行われたコメント [アクティビティ][]に関する情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="b35ae-103">The **CommentAction** resource provides information about a comment [activity][] made on an item.</span></span>

[アクティビティ]: itemactivity.md
[activity]: itemactivity.md

## <a name="json-representation"></a><span data-ttu-id="b35ae-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b35ae-105">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="b35ae-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b35ae-106">Properties</span></span>

| <span data-ttu-id="b35ae-107">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="b35ae-107">Property name</span></span>    | <span data-ttu-id="b35ae-108">種類</span><span class="sxs-lookup"><span data-stu-id="b35ae-108">Type</span></span>                       | <span data-ttu-id="b35ae-109">説明</span><span class="sxs-lookup"><span data-stu-id="b35ae-109">Description</span></span>
|:-----------------|:---------------------------|:-----------------------------
| <span data-ttu-id="b35ae-110">isReply</span><span class="sxs-lookup"><span data-stu-id="b35ae-110">isReply</span></span>          | <span data-ttu-id="b35ae-111">boolean</span><span class="sxs-lookup"><span data-stu-id="b35ae-111">boolean</span></span>                    | <span data-ttu-id="b35ae-112">true の場合、このアクティビティは既存のコメント スレッドへの返信だったことを示します。</span><span class="sxs-lookup"><span data-stu-id="b35ae-112">If true, this activity was a reply to an existing comment thread.</span></span>
| <span data-ttu-id="b35ae-113">parentAuthor</span><span class="sxs-lookup"><span data-stu-id="b35ae-113">parentAuthor</span></span>     | <span data-ttu-id="b35ae-114">[identitySet][]</span><span class="sxs-lookup"><span data-stu-id="b35ae-114">[identitySet][]</span></span>            | <span data-ttu-id="b35ae-115">コメント スレッドを開始したユーザーの ID。</span><span class="sxs-lookup"><span data-stu-id="b35ae-115">The identity of the user who started the comment thread.</span></span>
| <span data-ttu-id="b35ae-116">participants</span><span class="sxs-lookup"><span data-stu-id="b35ae-116">participants</span></span>     | <span data-ttu-id="b35ae-117">[identitySet][] コレクション</span><span class="sxs-lookup"><span data-stu-id="b35ae-117">[identitySet][] collection</span></span> | <span data-ttu-id="b35ae-118">該当のコメント スレッドに参加しているユーザーの ID。</span><span class="sxs-lookup"><span data-stu-id="b35ae-118">The identities of the users participating in this comment thread.</span></span>

[identitySet]: identityset.md

## <a name="remarks"></a><span data-ttu-id="b35ae-120">備考</span><span class="sxs-lookup"><span data-stu-id="b35ae-120">Remarks</span></span>

<span data-ttu-id="b35ae-121">アイテムのアクティビティの記録は、現在、SharePoint と OneDrive for Business でのみ使用できます。</span><span class="sxs-lookup"><span data-stu-id="b35ae-121">Item activity records are currently only available on SharePoint and OneDrive for Business.</span></span>

<!--
{
  "type": "#page.annotation",
  "description": "The CommentAction object provides information about a comment that was made on an item.",
  "keywords": "activities,activity,action,comment",
  "section": "documentation",
  "tocPath": "Resources/CommentAction",
  "suppressions": [
    "Error: /api-reference/beta/resources/commentaction.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
