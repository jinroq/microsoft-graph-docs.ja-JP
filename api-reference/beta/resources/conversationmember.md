---
title: conversationMember リソース タイプ
description: 会話のユーザーを表します。
localization_priority: Priority
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: f6908106390e527ab4e33e777dd232b58ead727a
ms.sourcegitcommit: afea19508ad74a3583b11b5f7b544c53eafb3740
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/22/2019
ms.locfileid: "34379298"
---
# <a name="conversationmember-resource-type"></a><span data-ttu-id="1f237-103">conversationMember リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="1f237-103">conversationMember resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1f237-104">[chat](chat.md) のユーザーを表します。</span><span class="sxs-lookup"><span data-stu-id="1f237-104">Represents a user in a [chat](chat.md).</span></span>

## <a name="methods"></a><span data-ttu-id="1f237-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="1f237-105">Methods</span></span>

| <span data-ttu-id="1f237-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="1f237-106">Method</span></span>       | <span data-ttu-id="1f237-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="1f237-107">Return Type</span></span>  |<span data-ttu-id="1f237-108">説明</span><span class="sxs-lookup"><span data-stu-id="1f237-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1f237-109">チャットのメンバーを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="1f237-109">List Chat members</span></span>](../api/conversationmember-list.md) | <span data-ttu-id="1f237-110">[conversationmember](conversationmember.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="1f237-110">[conversationmember](conversationmember.md) collection</span></span> | <span data-ttu-id="1f237-111">チャットのすべてのメンバーのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="1f237-111">Get the list of all users in the chat.</span></span>|
|[<span data-ttu-id="1f237-112">チャットのメンバーを取得する</span><span class="sxs-lookup"><span data-stu-id="1f237-112">Get Chat member</span></span>](../api/conversationmember-get.md) | [<span data-ttu-id="1f237-113">conversationmember</span><span class="sxs-lookup"><span data-stu-id="1f237-113">conversationmember</span></span>](conversationmember.md) | <span data-ttu-id="1f237-114">チャットの 1 人のユーザーを取得します。</span><span class="sxs-lookup"><span data-stu-id="1f237-114">Get a single user in the chat.</span></span>|

## <a name="properties"></a><span data-ttu-id="1f237-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1f237-115">Properties</span></span>
| <span data-ttu-id="1f237-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1f237-116">Property</span></span>     | <span data-ttu-id="1f237-117">型</span><span class="sxs-lookup"><span data-stu-id="1f237-117">Type</span></span>   |<span data-ttu-id="1f237-118">説明</span><span class="sxs-lookup"><span data-stu-id="1f237-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1f237-119">id</span><span class="sxs-lookup"><span data-stu-id="1f237-119">id</span></span>|<span data-ttu-id="1f237-120">String</span><span class="sxs-lookup"><span data-stu-id="1f237-120">String</span></span>| <span data-ttu-id="1f237-121">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="1f237-121">Read-only.</span></span> <span data-ttu-id="1f237-122">ユーザーの一意の ID。</span><span class="sxs-lookup"><span data-stu-id="1f237-122">Unique ID of the message.</span></span>|
|<span data-ttu-id="1f237-123">displayName</span><span class="sxs-lookup"><span data-stu-id="1f237-123">displayName</span></span>| <span data-ttu-id="1f237-124">string</span><span class="sxs-lookup"><span data-stu-id="1f237-124">string</span></span> | <span data-ttu-id="1f237-125">ユーザーの表示名。</span><span class="sxs-lookup"><span data-stu-id="1f237-125">The display name of the user.</span></span> |
|<span data-ttu-id="1f237-126">roles</span><span class="sxs-lookup"><span data-stu-id="1f237-126">roles</span></span>| <span data-ttu-id="1f237-127">string コレクション</span><span class="sxs-lookup"><span data-stu-id="1f237-127">string collection</span></span> | <span data-ttu-id="1f237-128">そのユーザーのロール。</span><span class="sxs-lookup"><span data-stu-id="1f237-128">The roles for that user.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="1f237-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1f237-129">JSON representation</span></span>

<span data-ttu-id="1f237-130">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1f237-130">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.conversationMember"
}-->

```json
{
  "id": "string (identifier)",
  "displayName" : "string",
  "roles" : ["string"]
}

```

## <a name="see-also"></a><span data-ttu-id="1f237-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="1f237-131">See Also</span></span>

[<span data-ttu-id="1f237-132">aadUserConversationMember</span><span class="sxs-lookup"><span data-stu-id="1f237-132">aadUserConversationMember</span></span>](aaduserconversationmember.md)

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "conversationMember",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
