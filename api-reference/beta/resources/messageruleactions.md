---
title: messageRuleActions リソースの種類
description: ルールに使用可能なアクションのセットを表します。
author: angelgolfer-ms
ms.openlocfilehash: 515d31ff8c11b95a3aa0042449d22df883e0eecf
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27314995"
---
# <a name="messageruleactions-resource-type"></a><span data-ttu-id="0cb9a-103">messageRuleActions リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0cb9a-103">messageRuleActions resource type</span></span>

> <span data-ttu-id="0cb9a-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0cb9a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0cb9a-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0cb9a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0cb9a-106">ルールに使用可能なアクションのセットを表します。</span><span class="sxs-lookup"><span data-stu-id="0cb9a-106">Represents the set of actions that are available to a rule.</span></span>

## <a name="properties"></a><span data-ttu-id="0cb9a-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0cb9a-107">Properties</span></span>
| <span data-ttu-id="0cb9a-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0cb9a-108">Property</span></span>     | <span data-ttu-id="0cb9a-109">種類</span><span class="sxs-lookup"><span data-stu-id="0cb9a-109">Type</span></span>   |<span data-ttu-id="0cb9a-110">説明</span><span class="sxs-lookup"><span data-stu-id="0cb9a-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="0cb9a-111">assignCategories</span><span class="sxs-lookup"><span data-stu-id="0cb9a-111">assignCategories</span></span> | <span data-ttu-id="0cb9a-112">String コレクション</span><span class="sxs-lookup"><span data-stu-id="0cb9a-112">String collection</span></span> | <span data-ttu-id="0cb9a-113">メッセージに割り当てられるカテゴリの一覧です。</span><span class="sxs-lookup"><span data-stu-id="0cb9a-113">A list of categories to be assigned to a message.</span></span> |
| <span data-ttu-id="0cb9a-114">copyToFolder</span><span class="sxs-lookup"><span data-stu-id="0cb9a-114">copyToFolder</span></span> | <span data-ttu-id="0cb9a-115">String</span><span class="sxs-lookup"><span data-stu-id="0cb9a-115">String</span></span> | <span data-ttu-id="0cb9a-116">メッセージのコピー先のフォルダーの ID です。</span><span class="sxs-lookup"><span data-stu-id="0cb9a-116">The ID of a folder that a message is to be copied to.</span></span> |
| <span data-ttu-id="0cb9a-117">delete</span><span class="sxs-lookup"><span data-stu-id="0cb9a-117">delete</span></span> | <span data-ttu-id="0cb9a-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="0cb9a-118">Boolean</span></span> | <span data-ttu-id="0cb9a-119">削除済みアイテム フォルダーにメッセージを移動する必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="0cb9a-119">Indicates whether a message should be moved to the Deleted Items folder.</span></span> |
| <span data-ttu-id="0cb9a-120">forwardAsAttachmentTo</span><span class="sxs-lookup"><span data-stu-id="0cb9a-120">forwardAsAttachmentTo</span></span> | <span data-ttu-id="0cb9a-121">[recipient](recipient.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="0cb9a-121">[recipient](recipient.md) collection</span></span> | <span data-ttu-id="0cb9a-122">添付ファイルとしてメッセージを転送する受信者の電子メール アドレスです。</span><span class="sxs-lookup"><span data-stu-id="0cb9a-122">The email addresses of the recipients to which a message should be forwarded as an attachment.</span></span> |
| <span data-ttu-id="0cb9a-123">forwardTo</span><span class="sxs-lookup"><span data-stu-id="0cb9a-123">forwardTo</span></span> | <span data-ttu-id="0cb9a-124">[recipient](recipient.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="0cb9a-124">[recipient](recipient.md) collection</span></span> | <span data-ttu-id="0cb9a-125">メッセージを転送する受信者の電子メール アドレスです。</span><span class="sxs-lookup"><span data-stu-id="0cb9a-125">The email addresses of the recipients to which a message should be forwarded.</span></span> |
| <span data-ttu-id="0cb9a-126">markAsRead</span><span class="sxs-lookup"><span data-stu-id="0cb9a-126">markAsRead</span></span> | <span data-ttu-id="0cb9a-127">Boolean</span><span class="sxs-lookup"><span data-stu-id="0cb9a-127">Boolean</span></span> | <span data-ttu-id="0cb9a-128">メッセージを開封済みにする必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="0cb9a-128">Indicates whether a message should be marked as read.</span></span> |
| <span data-ttu-id="0cb9a-129">markImportance</span><span class="sxs-lookup"><span data-stu-id="0cb9a-129">markImportance</span></span> | <span data-ttu-id="0cb9a-130">String</span><span class="sxs-lookup"><span data-stu-id="0cb9a-130">String</span></span> | <span data-ttu-id="0cb9a-131">メッセージの重要度を設定します。使用可能な値は、`low`、`normal`、`high` です。</span><span class="sxs-lookup"><span data-stu-id="0cb9a-131">Sets the importance of the message, which can be: `low`, `normal`, `high`.</span></span> |
| <span data-ttu-id="0cb9a-132">moveToFolder</span><span class="sxs-lookup"><span data-stu-id="0cb9a-132">moveToFolder</span></span> |  <span data-ttu-id="0cb9a-133">String</span><span class="sxs-lookup"><span data-stu-id="0cb9a-133">String</span></span>| <span data-ttu-id="0cb9a-134">メッセージ移動先のフォルダーの ID です。</span><span class="sxs-lookup"><span data-stu-id="0cb9a-134">The ID of the folder that a message will be moved to.</span></span> |
| <span data-ttu-id="0cb9a-135">permanentDelete</span><span class="sxs-lookup"><span data-stu-id="0cb9a-135">permanentDelete</span></span> | <span data-ttu-id="0cb9a-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="0cb9a-136">Boolean</span></span> | <span data-ttu-id="0cb9a-137">メッセージを完全に削除し、削除済みアイテム フォルダーにメッセージを保存しないようにするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="0cb9a-137">Indicates whether a message should be permanently deleted and not saved to the Deleted Items folder.</span></span> |
| <span data-ttu-id="0cb9a-138">redirectTo</span><span class="sxs-lookup"><span data-stu-id="0cb9a-138">redirectTo</span></span> | [<span data-ttu-id="0cb9a-139">recipient</span><span class="sxs-lookup"><span data-stu-id="0cb9a-139">recipient</span></span>](recipient.md) | <span data-ttu-id="0cb9a-140">メッセージのリダイレクト先の電子メール アドレスです。</span><span class="sxs-lookup"><span data-stu-id="0cb9a-140">The email address to which a message should be redirected.</span></span> |
| <span data-ttu-id="0cb9a-141">stopProcessingRules</span><span class="sxs-lookup"><span data-stu-id="0cb9a-141">stopProcessingRules</span></span> | <span data-ttu-id="0cb9a-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="0cb9a-142">Boolean</span></span> | <span data-ttu-id="0cb9a-143">後続のルールを評価する必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="0cb9a-143">Indicates whether subsequent rules should be evaluated.</span></span> |


## <a name="json-representation"></a><span data-ttu-id="0cb9a-144">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0cb9a-144">JSON representation</span></span>
<span data-ttu-id="0cb9a-145">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0cb9a-145">Here is a JSON representation of the resource.</span></span>

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