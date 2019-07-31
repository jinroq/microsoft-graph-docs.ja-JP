---
title: messageRuleActions リソースの種類
description: ルールに使用可能なアクションのセットを表します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
doc_type: resourcePageType
ms.openlocfilehash: 74462319b2878d4f0915b3f03d70a6dae06534b7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009686"
---
# <a name="messageruleactions-resource-type"></a><span data-ttu-id="6ae32-103">messageRuleActions リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6ae32-103">messageRuleActions resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6ae32-104">ルールに使用可能なアクションのセットを表します。</span><span class="sxs-lookup"><span data-stu-id="6ae32-104">Represents the set of actions that are available to a rule.</span></span>

## <a name="properties"></a><span data-ttu-id="6ae32-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6ae32-105">Properties</span></span>
| <span data-ttu-id="6ae32-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6ae32-106">Property</span></span>     | <span data-ttu-id="6ae32-107">型</span><span class="sxs-lookup"><span data-stu-id="6ae32-107">Type</span></span>   |<span data-ttu-id="6ae32-108">説明</span><span class="sxs-lookup"><span data-stu-id="6ae32-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="6ae32-109">assignCategories</span><span class="sxs-lookup"><span data-stu-id="6ae32-109">assignCategories</span></span> | <span data-ttu-id="6ae32-110">String コレクション</span><span class="sxs-lookup"><span data-stu-id="6ae32-110">String collection</span></span> | <span data-ttu-id="6ae32-111">メッセージに割り当てられるカテゴリの一覧です。</span><span class="sxs-lookup"><span data-stu-id="6ae32-111">A list of categories to be assigned to a message.</span></span> |
| <span data-ttu-id="6ae32-112">copyToFolder</span><span class="sxs-lookup"><span data-stu-id="6ae32-112">copyToFolder</span></span> | <span data-ttu-id="6ae32-113">String</span><span class="sxs-lookup"><span data-stu-id="6ae32-113">String</span></span> | <span data-ttu-id="6ae32-114">メッセージのコピー先のフォルダーの ID です。</span><span class="sxs-lookup"><span data-stu-id="6ae32-114">The ID of a folder that a message is to be copied to.</span></span> |
| <span data-ttu-id="6ae32-115">delete</span><span class="sxs-lookup"><span data-stu-id="6ae32-115">delete</span></span> | <span data-ttu-id="6ae32-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ae32-116">Boolean</span></span> | <span data-ttu-id="6ae32-117">削除済みアイテム フォルダーにメッセージを移動する必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6ae32-117">Indicates whether a message should be moved to the Deleted Items folder.</span></span> |
| <span data-ttu-id="6ae32-118">forwardAsAttachmentTo</span><span class="sxs-lookup"><span data-stu-id="6ae32-118">forwardAsAttachmentTo</span></span> | <span data-ttu-id="6ae32-119">[recipient](recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="6ae32-119">[recipient](recipient.md) collection</span></span> | <span data-ttu-id="6ae32-120">添付ファイルとしてメッセージを転送する受信者の電子メール アドレスです。</span><span class="sxs-lookup"><span data-stu-id="6ae32-120">The email addresses of the recipients to which a message should be forwarded as an attachment.</span></span> |
| <span data-ttu-id="6ae32-121">forwardTo</span><span class="sxs-lookup"><span data-stu-id="6ae32-121">forwardTo</span></span> | <span data-ttu-id="6ae32-122">[recipient](recipient.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="6ae32-122">[recipient](recipient.md) collection</span></span> | <span data-ttu-id="6ae32-123">メッセージを転送する受信者の電子メール アドレスです。</span><span class="sxs-lookup"><span data-stu-id="6ae32-123">The email addresses of the recipients to which a message should be forwarded.</span></span> |
| <span data-ttu-id="6ae32-124">markAsRead</span><span class="sxs-lookup"><span data-stu-id="6ae32-124">markAsRead</span></span> | <span data-ttu-id="6ae32-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ae32-125">Boolean</span></span> | <span data-ttu-id="6ae32-126">メッセージを開封済みにする必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6ae32-126">Indicates whether a message should be marked as read.</span></span> |
| <span data-ttu-id="6ae32-127">markImportance</span><span class="sxs-lookup"><span data-stu-id="6ae32-127">markImportance</span></span> | <span data-ttu-id="6ae32-128">String</span><span class="sxs-lookup"><span data-stu-id="6ae32-128">String</span></span> | <span data-ttu-id="6ae32-129">メッセージの重要度を設定します。使用可能な値は、`low`、`normal`、`high` です。</span><span class="sxs-lookup"><span data-stu-id="6ae32-129">Sets the importance of the message, which can be: `low`, `normal`, `high`.</span></span> |
| <span data-ttu-id="6ae32-130">moveToFolder</span><span class="sxs-lookup"><span data-stu-id="6ae32-130">moveToFolder</span></span> |  <span data-ttu-id="6ae32-131">String</span><span class="sxs-lookup"><span data-stu-id="6ae32-131">String</span></span>| <span data-ttu-id="6ae32-132">メッセージ移動先のフォルダーの ID です。</span><span class="sxs-lookup"><span data-stu-id="6ae32-132">The ID of the folder that a message will be moved to.</span></span> |
| <span data-ttu-id="6ae32-133">permanentDelete</span><span class="sxs-lookup"><span data-stu-id="6ae32-133">permanentDelete</span></span> | <span data-ttu-id="6ae32-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ae32-134">Boolean</span></span> | <span data-ttu-id="6ae32-135">メッセージを完全に削除し、削除済みアイテム フォルダーにメッセージを保存しないようにするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6ae32-135">Indicates whether a message should be permanently deleted and not saved to the Deleted Items folder.</span></span> |
| <span data-ttu-id="6ae32-136">redirectTo</span><span class="sxs-lookup"><span data-stu-id="6ae32-136">redirectTo</span></span> | [<span data-ttu-id="6ae32-137">recipient</span><span class="sxs-lookup"><span data-stu-id="6ae32-137">recipient</span></span>](recipient.md) | <span data-ttu-id="6ae32-138">メッセージのリダイレクト先の電子メール アドレスです。</span><span class="sxs-lookup"><span data-stu-id="6ae32-138">The email address to which a message should be redirected.</span></span> |
| <span data-ttu-id="6ae32-139">stopProcessingRules</span><span class="sxs-lookup"><span data-stu-id="6ae32-139">stopProcessingRules</span></span> | <span data-ttu-id="6ae32-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="6ae32-140">Boolean</span></span> | <span data-ttu-id="6ae32-141">後続のルールを評価する必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6ae32-141">Indicates whether subsequent rules should be evaluated.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="6ae32-142">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6ae32-142">JSON representation</span></span>
<span data-ttu-id="6ae32-143">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6ae32-143">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
