---
title: messageRuleActions リソースの種類
description: ルールに使用可能なアクションのセットを表します。
author: angelgolfer-ms
localization_priority: Normal
ms.prod: outlook
ms.openlocfilehash: 33f1167d7317f941ebfa79b372e9cf575c14989b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32548503"
---
# <a name="messageruleactions-resource-type"></a><span data-ttu-id="e781c-103">messageRuleActions リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e781c-103">messageRuleActions resource type</span></span>


<span data-ttu-id="e781c-104">ルールに使用可能なアクションのセットを表します。</span><span class="sxs-lookup"><span data-stu-id="e781c-104">Represents the set of actions that are available to a rule.</span></span>

## <a name="properties"></a><span data-ttu-id="e781c-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e781c-105">Properties</span></span>
| <span data-ttu-id="e781c-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e781c-106">Property</span></span>     | <span data-ttu-id="e781c-107">型</span><span class="sxs-lookup"><span data-stu-id="e781c-107">Type</span></span>   |<span data-ttu-id="e781c-108">説明</span><span class="sxs-lookup"><span data-stu-id="e781c-108">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="e781c-109">assignCategories</span><span class="sxs-lookup"><span data-stu-id="e781c-109">assignCategories</span></span> | <span data-ttu-id="e781c-110">String コレクション</span><span class="sxs-lookup"><span data-stu-id="e781c-110">String collection</span></span> | <span data-ttu-id="e781c-111">メッセージに割り当てられるカテゴリの一覧です。</span><span class="sxs-lookup"><span data-stu-id="e781c-111">A list of categories to be assigned to a message.</span></span> |
| <span data-ttu-id="e781c-112">copyToFolder</span><span class="sxs-lookup"><span data-stu-id="e781c-112">copyToFolder</span></span> | <span data-ttu-id="e781c-113">String</span><span class="sxs-lookup"><span data-stu-id="e781c-113">String</span></span> | <span data-ttu-id="e781c-114">メッセージのコピー先のフォルダーの ID です。</span><span class="sxs-lookup"><span data-stu-id="e781c-114">The ID of a folder that a message is to be copied to.</span></span> |
| <span data-ttu-id="e781c-115">delete</span><span class="sxs-lookup"><span data-stu-id="e781c-115">delete</span></span> | <span data-ttu-id="e781c-116">ブール値</span><span class="sxs-lookup"><span data-stu-id="e781c-116">Boolean</span></span> | <span data-ttu-id="e781c-117">削除済みアイテム フォルダーにメッセージを移動する必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e781c-117">Indicates whether a message should be moved to the Deleted Items folder.</span></span> |
| <span data-ttu-id="e781c-118">forwardAsAttachmentTo</span><span class="sxs-lookup"><span data-stu-id="e781c-118">forwardAsAttachmentTo</span></span> | <span data-ttu-id="e781c-119">[recipient](recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="e781c-119">[recipient](recipient.md) collection</span></span> | <span data-ttu-id="e781c-120">添付ファイルとしてメッセージを転送する受信者の電子メール アドレスです。</span><span class="sxs-lookup"><span data-stu-id="e781c-120">The email addresses of the recipients to which a message should be forwarded as an attachment.</span></span> |
| <span data-ttu-id="e781c-121">forwardTo</span><span class="sxs-lookup"><span data-stu-id="e781c-121">forwardTo</span></span> | <span data-ttu-id="e781c-122">[recipient](recipient.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e781c-122">[recipient](recipient.md) collection</span></span> | <span data-ttu-id="e781c-123">メッセージを転送する受信者の電子メール アドレスです。</span><span class="sxs-lookup"><span data-stu-id="e781c-123">The email addresses of the recipients to which a message should be forwarded.</span></span> |
| <span data-ttu-id="e781c-124">markAsRead</span><span class="sxs-lookup"><span data-stu-id="e781c-124">markAsRead</span></span> | <span data-ttu-id="e781c-125">ブール値</span><span class="sxs-lookup"><span data-stu-id="e781c-125">Boolean</span></span> | <span data-ttu-id="e781c-126">メッセージを開封済みにする必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e781c-126">Indicates whether a message should be marked as read.</span></span> |
| <span data-ttu-id="e781c-127">markImportance</span><span class="sxs-lookup"><span data-stu-id="e781c-127">markImportance</span></span> | <span data-ttu-id="e781c-128">importance</span><span class="sxs-lookup"><span data-stu-id="e781c-128">importance</span></span> | <span data-ttu-id="e781c-129">メッセージの重要度を設定します。使用可能な値は、`low`、`normal`、`high` です。</span><span class="sxs-lookup"><span data-stu-id="e781c-129">Sets the importance of the message, which can be: `low`, `normal`, `high`.</span></span> |
| <span data-ttu-id="e781c-130">moveToFolder</span><span class="sxs-lookup"><span data-stu-id="e781c-130">moveToFolder</span></span> |  <span data-ttu-id="e781c-131">String</span><span class="sxs-lookup"><span data-stu-id="e781c-131">String</span></span>| <span data-ttu-id="e781c-132">メッセージ移動先のフォルダーの ID です。</span><span class="sxs-lookup"><span data-stu-id="e781c-132">The ID of the folder that a message will be moved to.</span></span> |
| <span data-ttu-id="e781c-133">permanentDelete</span><span class="sxs-lookup"><span data-stu-id="e781c-133">permanentDelete</span></span> | <span data-ttu-id="e781c-134">ブール値</span><span class="sxs-lookup"><span data-stu-id="e781c-134">Boolean</span></span> | <span data-ttu-id="e781c-135">メッセージを完全に削除し、削除済みアイテム フォルダーにメッセージを保存しないようにするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e781c-135">Indicates whether a message should be permanently deleted and not saved to the Deleted Items folder.</span></span> |
| <span data-ttu-id="e781c-136">redirectTo</span><span class="sxs-lookup"><span data-stu-id="e781c-136">redirectTo</span></span> | <span data-ttu-id="e781c-137">[recipient](recipient.md) collection</span><span class="sxs-lookup"><span data-stu-id="e781c-137">[recipient](recipient.md) collection</span></span> | <span data-ttu-id="e781c-138">メッセージのリダイレクト先となる電子メールアドレス。</span><span class="sxs-lookup"><span data-stu-id="e781c-138">The email addresses to which a message should be redirected.</span></span> |
| <span data-ttu-id="e781c-139">stopProcessingRules</span><span class="sxs-lookup"><span data-stu-id="e781c-139">stopProcessingRules</span></span> | <span data-ttu-id="e781c-140">Boolean</span><span class="sxs-lookup"><span data-stu-id="e781c-140">Boolean</span></span> | <span data-ttu-id="e781c-141">後続のルールを評価する必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e781c-141">Indicates whether subsequent rules should be evaluated.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="e781c-142">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e781c-142">JSON representation</span></span>
<span data-ttu-id="e781c-143">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e781c-143">Here is a JSON representation of the resource.</span></span>

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
  "redirectTo": [{"@odata.type": "microsoft.graph.recipient"}],
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
