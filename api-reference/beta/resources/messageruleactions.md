---
title: messageRuleActions リソースの種類
description: ルールに使用可能なアクションのセットを表します。
ms.openlocfilehash: fbd189d8a43dc47e139f69cd345b4c14744d94f5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067273"
---
# <a name="messageruleactions-resource-type"></a><span data-ttu-id="1d5d8-103">messageRuleActions リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1d5d8-103">messageRuleActions resource type</span></span>

> <span data-ttu-id="1d5d8-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1d5d8-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1d5d8-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1d5d8-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1d5d8-106">ルールに使用可能なアクションのセットを表します。</span><span class="sxs-lookup"><span data-stu-id="1d5d8-106">Represents the set of actions that are available to a rule.</span></span>

## <a name="properties"></a><span data-ttu-id="1d5d8-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1d5d8-107">Properties</span></span>
| <span data-ttu-id="1d5d8-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1d5d8-108">Property</span></span>     | <span data-ttu-id="1d5d8-109">型</span><span class="sxs-lookup"><span data-stu-id="1d5d8-109">Type</span></span>   |<span data-ttu-id="1d5d8-110">説明</span><span class="sxs-lookup"><span data-stu-id="1d5d8-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="1d5d8-111">assignCategories</span><span class="sxs-lookup"><span data-stu-id="1d5d8-111">assignCategories</span></span> | <span data-ttu-id="1d5d8-112">String コレクション</span><span class="sxs-lookup"><span data-stu-id="1d5d8-112">String collection</span></span> | <span data-ttu-id="1d5d8-113">メッセージに割り当てられるカテゴリの一覧です。</span><span class="sxs-lookup"><span data-stu-id="1d5d8-113">A list of categories to be assigned to a message.</span></span> |
| <span data-ttu-id="1d5d8-114">copyToFolder</span><span class="sxs-lookup"><span data-stu-id="1d5d8-114">copyToFolder</span></span> | <span data-ttu-id="1d5d8-115">String</span><span class="sxs-lookup"><span data-stu-id="1d5d8-115">String</span></span> | <span data-ttu-id="1d5d8-116">メッセージのコピー先のフォルダーの ID です。</span><span class="sxs-lookup"><span data-stu-id="1d5d8-116">The ID of a folder that a message is to be copied to.</span></span> |
| <span data-ttu-id="1d5d8-117">delete</span><span class="sxs-lookup"><span data-stu-id="1d5d8-117">delete</span></span> | <span data-ttu-id="1d5d8-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="1d5d8-118">Boolean</span></span> | <span data-ttu-id="1d5d8-119">削除済みアイテム フォルダーにメッセージを移動する必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1d5d8-119">Indicates whether a message should be moved to the Deleted Items folder.</span></span> |
| <span data-ttu-id="1d5d8-120">forwardAsAttachmentTo</span><span class="sxs-lookup"><span data-stu-id="1d5d8-120">forwardAsAttachmentTo</span></span> | <span data-ttu-id="1d5d8-121">[recipient](recipient.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="1d5d8-121">[recipient](recipient.md) collection</span></span> | <span data-ttu-id="1d5d8-122">添付ファイルとしてメッセージを転送する受信者の電子メール アドレスです。</span><span class="sxs-lookup"><span data-stu-id="1d5d8-122">The email addresses of the recipients to which a message should be forwarded as an attachment.</span></span> |
| <span data-ttu-id="1d5d8-123">forwardTo</span><span class="sxs-lookup"><span data-stu-id="1d5d8-123">forwardTo</span></span> | <span data-ttu-id="1d5d8-124">[recipient](recipient.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="1d5d8-124">[recipient](recipient.md) collection</span></span> | <span data-ttu-id="1d5d8-125">メッセージを転送する受信者の電子メール アドレスです。</span><span class="sxs-lookup"><span data-stu-id="1d5d8-125">The email addresses of the recipients to which a message should be forwarded.</span></span> |
| <span data-ttu-id="1d5d8-126">markAsRead</span><span class="sxs-lookup"><span data-stu-id="1d5d8-126">markAsRead</span></span> | <span data-ttu-id="1d5d8-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="1d5d8-127">Boolean</span></span> | <span data-ttu-id="1d5d8-128">メッセージを開封済みにする必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1d5d8-128">Indicates whether a message should be marked as read.</span></span> |
| <span data-ttu-id="1d5d8-129">markImportance</span><span class="sxs-lookup"><span data-stu-id="1d5d8-129">markImportance</span></span> | <span data-ttu-id="1d5d8-130">String</span><span class="sxs-lookup"><span data-stu-id="1d5d8-130">String</span></span> | <span data-ttu-id="1d5d8-131">メッセージの重要度を設定します。使用可能な値は、`low`、`normal`、`high` です。</span><span class="sxs-lookup"><span data-stu-id="1d5d8-131">Sets the importance of the message, which can be: `low`, `normal`, `high`.</span></span> |
| <span data-ttu-id="1d5d8-132">moveToFolder</span><span class="sxs-lookup"><span data-stu-id="1d5d8-132">moveToFolder</span></span> |  <span data-ttu-id="1d5d8-133">String</span><span class="sxs-lookup"><span data-stu-id="1d5d8-133">String</span></span>| <span data-ttu-id="1d5d8-134">メッセージ移動先のフォルダーの ID です。</span><span class="sxs-lookup"><span data-stu-id="1d5d8-134">The ID of the folder that a message will be moved to.</span></span> |
| <span data-ttu-id="1d5d8-135">permanentDelete</span><span class="sxs-lookup"><span data-stu-id="1d5d8-135">permanentDelete</span></span> | <span data-ttu-id="1d5d8-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="1d5d8-136">Boolean</span></span> | <span data-ttu-id="1d5d8-137">メッセージを完全に削除し、削除済みアイテム フォルダーにメッセージを保存しないようにするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1d5d8-137">Indicates whether a message should be permanently deleted and not saved to the Deleted Items folder.</span></span> |
| <span data-ttu-id="1d5d8-138">redirectTo</span><span class="sxs-lookup"><span data-stu-id="1d5d8-138">redirectTo</span></span> | [<span data-ttu-id="1d5d8-139">recipient</span><span class="sxs-lookup"><span data-stu-id="1d5d8-139">recipient</span></span>](recipient.md) | <span data-ttu-id="1d5d8-140">メッセージのリダイレクト先の電子メール アドレスです。</span><span class="sxs-lookup"><span data-stu-id="1d5d8-140">The email address to which a message should be redirected.</span></span> |
| <span data-ttu-id="1d5d8-141">stopProcessingRules</span><span class="sxs-lookup"><span data-stu-id="1d5d8-141">stopProcessingRules</span></span> | <span data-ttu-id="1d5d8-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="1d5d8-142">Boolean</span></span> | <span data-ttu-id="1d5d8-143">後続のルールを評価する必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1d5d8-143">Indicates whether subsequent rules should be evaluated.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="1d5d8-144">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1d5d8-144">JSON representation</span></span>
<span data-ttu-id="1d5d8-145">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1d5d8-145">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "messageRuleActions resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->