---
title: messageRuleActions リソースの種類
description: ルールに使用可能なアクションのセットを表します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: a786a225bb9d439d60a29d2395b2d438975fc16c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32523421"
---
# <a name="messageruleactions-resource-type"></a><span data-ttu-id="5383f-103">messageRuleActions リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5383f-103">messageRuleActions resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5383f-104">ルールに使用可能なアクションのセットを表します。</span><span class="sxs-lookup"><span data-stu-id="5383f-104">Represents the set of actions that are available to a rule.</span></span>

## <a name="properties"></a><span data-ttu-id="5383f-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5383f-105">Properties</span></span>
| <span data-ttu-id="5383f-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5383f-106">Property</span></span>     | <span data-ttu-id="5383f-107">型</span><span class="sxs-lookup"><span data-stu-id="5383f-107">Type</span></span>   |<span data-ttu-id="5383f-108">説明</span><span class="sxs-lookup"><span data-stu-id="5383f-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5383f-109">assignCategories</span><span class="sxs-lookup"><span data-stu-id="5383f-109">assignCategories</span></span> | <span data-ttu-id="5383f-110">String コレクション</span><span class="sxs-lookup"><span data-stu-id="5383f-110">String collection</span></span> | <span data-ttu-id="5383f-111">メッセージに割り当てられるカテゴリの一覧です。</span><span class="sxs-lookup"><span data-stu-id="5383f-111">A list of categories to be assigned to a message.</span></span> |
| <span data-ttu-id="5383f-112">copyToFolder</span><span class="sxs-lookup"><span data-stu-id="5383f-112">copyToFolder</span></span> | <span data-ttu-id="5383f-113">String
</span><span class="sxs-lookup"><span data-stu-id="5383f-113">String</span></span> | <span data-ttu-id="5383f-114">メッセージのコピー先のフォルダーの ID です。</span><span class="sxs-lookup"><span data-stu-id="5383f-114">The ID of a folder that a message is to be copied to.</span></span> |
| <span data-ttu-id="5383f-115">delete</span><span class="sxs-lookup"><span data-stu-id="5383f-115">delete</span></span> | <span data-ttu-id="5383f-116">ブール型</span><span class="sxs-lookup"><span data-stu-id="5383f-116">Boolean</span></span> | <span data-ttu-id="5383f-117">削除済みアイテム フォルダーにメッセージを移動する必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="5383f-117">Indicates whether a message should be moved to the Deleted Items folder.</span></span> |
| <span data-ttu-id="5383f-118">forwardAsAttachmentTo</span><span class="sxs-lookup"><span data-stu-id="5383f-118">forwardAsAttachmentTo</span></span> | <span data-ttu-id="5383f-119">[recipient](recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="5383f-119">[recipient](recipient.md) collection</span></span> | <span data-ttu-id="5383f-120">添付ファイルとしてメッセージを転送する受信者の電子メール アドレスです。</span><span class="sxs-lookup"><span data-stu-id="5383f-120">The email addresses of the recipients to which a message should be forwarded as an attachment.</span></span> |
| <span data-ttu-id="5383f-121">forwardTo</span><span class="sxs-lookup"><span data-stu-id="5383f-121">forwardTo</span></span> | <span data-ttu-id="5383f-122">[recipient](recipient.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="5383f-122">[recipient](recipient.md) collection</span></span> | <span data-ttu-id="5383f-123">メッセージを転送する受信者の電子メール アドレスです。</span><span class="sxs-lookup"><span data-stu-id="5383f-123">The email addresses of the recipients to which a message should be forwarded.</span></span> |
| <span data-ttu-id="5383f-124">markAsRead</span><span class="sxs-lookup"><span data-stu-id="5383f-124">markAsRead</span></span> | <span data-ttu-id="5383f-125">ブール型</span><span class="sxs-lookup"><span data-stu-id="5383f-125">Boolean</span></span> | <span data-ttu-id="5383f-126">メッセージを開封済みにする必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="5383f-126">Indicates whether a message should be marked as read.</span></span> |
| <span data-ttu-id="5383f-127">markImportance</span><span class="sxs-lookup"><span data-stu-id="5383f-127">markImportance</span></span> | <span data-ttu-id="5383f-128">String
</span><span class="sxs-lookup"><span data-stu-id="5383f-128">String</span></span> | <span data-ttu-id="5383f-129">メッセージの重要度を設定します。使用可能な値は、`low`、`normal`、`high` です。</span><span class="sxs-lookup"><span data-stu-id="5383f-129">Sets the importance of the message, which can be: `low`, `normal`, `high`.</span></span> |
| <span data-ttu-id="5383f-130">moveToFolder</span><span class="sxs-lookup"><span data-stu-id="5383f-130">moveToFolder</span></span> |  <span data-ttu-id="5383f-131">String</span><span class="sxs-lookup"><span data-stu-id="5383f-131">String</span></span>| <span data-ttu-id="5383f-132">メッセージ移動先のフォルダーの ID です。</span><span class="sxs-lookup"><span data-stu-id="5383f-132">The ID of the folder that a message will be moved to.</span></span> |
| <span data-ttu-id="5383f-133">permanentDelete</span><span class="sxs-lookup"><span data-stu-id="5383f-133">permanentDelete</span></span> | <span data-ttu-id="5383f-134">ブール型</span><span class="sxs-lookup"><span data-stu-id="5383f-134">Boolean</span></span> | <span data-ttu-id="5383f-135">メッセージを完全に削除し、削除済みアイテム フォルダーにメッセージを保存しないようにするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="5383f-135">Indicates whether a message should be permanently deleted and not saved to the Deleted Items folder.</span></span> |
| <span data-ttu-id="5383f-136">redirectTo</span><span class="sxs-lookup"><span data-stu-id="5383f-136">redirectTo</span></span> | [<span data-ttu-id="5383f-137">recipient</span><span class="sxs-lookup"><span data-stu-id="5383f-137">recipient</span></span>](recipient.md) | <span data-ttu-id="5383f-138">メッセージのリダイレクト先の電子メール アドレスです。</span><span class="sxs-lookup"><span data-stu-id="5383f-138">The email address to which a message should be redirected.</span></span> |
| <span data-ttu-id="5383f-139">stopProcessingRules</span><span class="sxs-lookup"><span data-stu-id="5383f-139">stopProcessingRules</span></span> | <span data-ttu-id="5383f-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="5383f-140">Boolean</span></span> | <span data-ttu-id="5383f-141">後続のルールを評価する必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="5383f-141">Indicates whether subsequent rules should be evaluated.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="5383f-142">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5383f-142">JSON representation</span></span>
<span data-ttu-id="5383f-143">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="5383f-143">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [
   ],
  "@odata.type": "microsoft.graph.messageRuleActions"
}-->

```json
{
  "assignCategories": ["String"],
  "copyToFolder": "String",
  "delete": "Boolean",
  "forwardAsAttachmentTo": [{"@odata.type": "microsoft.graph.recipient"}],
  "forwardTo": [{"@odata.type": "microsoft.graph.recipient"}],
  "markAsRead": "Boolean",
  "markImportance": "String",
  "moveToFolder": "String",
  "permanentDelete": "Boolean",
  "redirectTo": {"@odata.type": "microsoft.graph.recipient"},
  "stopProcessingRules": "Boolean"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "messageRuleActions resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/messageruleactions.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
