---
title: aadUserConversationMember リソース タイプ
description: 会話のユーザーを表します。
localization_priority: Priority
author: nkramer
ms.prod: microsoft-teams
ms.openlocfilehash: fd326482869d9f72778edc9d4c55996f7aa59045
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/26/2019
ms.locfileid: "35236462"
---
# <a name="aaduserconversationmember-resource-type"></a><span data-ttu-id="32a7a-103">aadUserConversationMember リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="32a7a-103">aadUserConversationMember resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="32a7a-104">[chat](chat.md) の Azure Active Directory ユーザーを表します。</span><span class="sxs-lookup"><span data-stu-id="32a7a-104">Represents an Azure Active Directory user in a [chat](chat.md).</span></span> <span data-ttu-id="32a7a-105">このタイプは、[conversationMember](conversationmember.md) から継承されています。</span><span class="sxs-lookup"><span data-stu-id="32a7a-105">This type inherits from [conversationMember](conversationmember.md).</span></span>

## <a name="methods"></a><span data-ttu-id="32a7a-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="32a7a-106">Methods</span></span>

| <span data-ttu-id="32a7a-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="32a7a-107">Method</span></span>       | <span data-ttu-id="32a7a-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="32a7a-108">Return Type</span></span>  |<span data-ttu-id="32a7a-109">説明</span><span class="sxs-lookup"><span data-stu-id="32a7a-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="32a7a-110">チャットのメンバーを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="32a7a-110">List Chat members</span></span>](../api/conversationmember-list.md) | <span data-ttu-id="32a7a-111">[conversationmember](conversationmember.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="32a7a-111">[conversationmember](conversationmember.md) collection</span></span> | <span data-ttu-id="32a7a-112">チャットのすべてのメンバーのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="32a7a-112">Get the list of all users in the chat.</span></span>|
|[<span data-ttu-id="32a7a-113">チャットのメンバーを取得する</span><span class="sxs-lookup"><span data-stu-id="32a7a-113">Get Chat member</span></span>](../api/conversationmember-get.md) | [<span data-ttu-id="32a7a-114">conversationmember</span><span class="sxs-lookup"><span data-stu-id="32a7a-114">conversationmember</span></span>](conversationmember.md) | <span data-ttu-id="32a7a-115">チャットの 1 人のユーザーを取得します。</span><span class="sxs-lookup"><span data-stu-id="32a7a-115">Get a single user in the chat.</span></span>|

## <a name="properties"></a><span data-ttu-id="32a7a-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="32a7a-116">Properties</span></span>
| <span data-ttu-id="32a7a-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="32a7a-117">Property</span></span>     | <span data-ttu-id="32a7a-118">型</span><span class="sxs-lookup"><span data-stu-id="32a7a-118">Type</span></span>   |<span data-ttu-id="32a7a-119">説明</span><span class="sxs-lookup"><span data-stu-id="32a7a-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="32a7a-120">id</span><span class="sxs-lookup"><span data-stu-id="32a7a-120">id</span></span>|<span data-ttu-id="32a7a-121">String</span><span class="sxs-lookup"><span data-stu-id="32a7a-121">String</span></span>| <span data-ttu-id="32a7a-122">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="32a7a-122">Read-only.</span></span> <span data-ttu-id="32a7a-123">ユーザーの一意の ID。</span><span class="sxs-lookup"><span data-stu-id="32a7a-123">Unique ID of the message.</span></span>|
|<span data-ttu-id="32a7a-124">displayName</span><span class="sxs-lookup"><span data-stu-id="32a7a-124">displayName</span></span>| <span data-ttu-id="32a7a-125">string</span><span class="sxs-lookup"><span data-stu-id="32a7a-125">string</span></span> | <span data-ttu-id="32a7a-126">ユーザーの表示名。</span><span class="sxs-lookup"><span data-stu-id="32a7a-126">The display name of the user.</span></span> |
|<span data-ttu-id="32a7a-127">roles</span><span class="sxs-lookup"><span data-stu-id="32a7a-127">roles</span></span>| <span data-ttu-id="32a7a-128">string コレクション</span><span class="sxs-lookup"><span data-stu-id="32a7a-128">string collection</span></span> | <span data-ttu-id="32a7a-129">そのユーザーのロール。</span><span class="sxs-lookup"><span data-stu-id="32a7a-129">The roles for that user.</span></span> |
|<span data-ttu-id="32a7a-130">userId</span><span class="sxs-lookup"><span data-stu-id="32a7a-130">userId</span></span>| <span data-ttu-id="32a7a-131">string</span><span class="sxs-lookup"><span data-stu-id="32a7a-131">string</span></span> | <span data-ttu-id="32a7a-132">ユーザーの GUID。</span><span class="sxs-lookup"><span data-stu-id="32a7a-132">The guid of the user.</span></span> |
|<span data-ttu-id="32a7a-133">メール</span><span class="sxs-lookup"><span data-stu-id="32a7a-133">email</span></span>| <span data-ttu-id="32a7a-134">string</span><span class="sxs-lookup"><span data-stu-id="32a7a-134">string</span></span>  | <span data-ttu-id="32a7a-135">ユーザーの電子メール アドレス。</span><span class="sxs-lookup"><span data-stu-id="32a7a-135">The e-mail address of the user.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="32a7a-136">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="32a7a-136">JSON representation</span></span>

<span data-ttu-id="32a7a-137">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="32a7a-137">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.aadUserConversationMember"
}-->

```json
{
  "id": "string (identifier)",
  "displayName" : "string",
  "roles" : ["string"],
  "userId" : "string",
  "email" : "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "aadUserConversationMember",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
