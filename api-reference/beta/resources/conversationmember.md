---
title: conversationMember リソース タイプ
description: 会話のユーザーを表します。
localization_priority: Normal
author: nkramer
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 10a40e53831cc44559a42d1684039c186554e433
ms.sourcegitcommit: 624ac42e74533a9bf0d0d22b3b15adbb258fd594
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/05/2019
ms.locfileid: "34709349"
---
# <a name="conversationmember-resource-type"></a><span data-ttu-id="422e5-103">conversationMember リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="422e5-103">conversationMember resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="422e5-104">[chat](chat.md) のユーザーを表します。</span><span class="sxs-lookup"><span data-stu-id="422e5-104">Represents a user in a [chat](chat.md).</span></span>

## <a name="methods"></a><span data-ttu-id="422e5-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="422e5-105">Methods</span></span>

| <span data-ttu-id="422e5-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="422e5-106">Method</span></span>       | <span data-ttu-id="422e5-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="422e5-107">Return Type</span></span>  |<span data-ttu-id="422e5-108">説明</span><span class="sxs-lookup"><span data-stu-id="422e5-108">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="422e5-109">チャットのメンバーを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="422e5-109">List Chat members</span></span>](../api/conversationmember-list.md) | <span data-ttu-id="422e5-110">[conversationmember](conversationmember.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="422e5-110">[conversationmember](conversationmember.md) collection</span></span> | <span data-ttu-id="422e5-111">チャットのすべてのメンバーのリストを取得します。</span><span class="sxs-lookup"><span data-stu-id="422e5-111">Get the list of all users in the chat.</span></span>|
|[<span data-ttu-id="422e5-112">チャットのメンバーを取得する</span><span class="sxs-lookup"><span data-stu-id="422e5-112">Get Chat member</span></span>](../api/conversationmember-get.md) | [<span data-ttu-id="422e5-113">conversationmember</span><span class="sxs-lookup"><span data-stu-id="422e5-113">conversationmember</span></span>](conversationmember.md) | <span data-ttu-id="422e5-114">チャットの 1 人のユーザーを取得します。</span><span class="sxs-lookup"><span data-stu-id="422e5-114">Get a single user in the chat.</span></span>|

## <a name="properties"></a><span data-ttu-id="422e5-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="422e5-115">Properties</span></span>

| <span data-ttu-id="422e5-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="422e5-116">Property</span></span>     | <span data-ttu-id="422e5-117">型</span><span class="sxs-lookup"><span data-stu-id="422e5-117">Type</span></span>   |<span data-ttu-id="422e5-118">説明</span><span class="sxs-lookup"><span data-stu-id="422e5-118">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="422e5-119">id</span><span class="sxs-lookup"><span data-stu-id="422e5-119">id</span></span>|<span data-ttu-id="422e5-120">String</span><span class="sxs-lookup"><span data-stu-id="422e5-120">String</span></span>| <span data-ttu-id="422e5-121">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="422e5-121">Read-only.</span></span> <span data-ttu-id="422e5-122">ユーザーの一意の ID。</span><span class="sxs-lookup"><span data-stu-id="422e5-122">Unique ID of the message.</span></span>|
|<span data-ttu-id="422e5-123">displayName</span><span class="sxs-lookup"><span data-stu-id="422e5-123">displayName</span></span>| <span data-ttu-id="422e5-124">string</span><span class="sxs-lookup"><span data-stu-id="422e5-124">string</span></span> | <span data-ttu-id="422e5-125">ユーザーの表示名。</span><span class="sxs-lookup"><span data-stu-id="422e5-125">The display name of the user.</span></span> |
|<span data-ttu-id="422e5-126">roles</span><span class="sxs-lookup"><span data-stu-id="422e5-126">roles</span></span>| <span data-ttu-id="422e5-127">string コレクション</span><span class="sxs-lookup"><span data-stu-id="422e5-127">string collection</span></span> | <span data-ttu-id="422e5-128">そのユーザーのロール。</span><span class="sxs-lookup"><span data-stu-id="422e5-128">The roles for that user.</span></span> |

## <a name="relationships"></a><span data-ttu-id="422e5-129">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="422e5-129">Relationships</span></span>

<span data-ttu-id="422e5-130">なし</span><span class="sxs-lookup"><span data-stu-id="422e5-130">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="422e5-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="422e5-131">JSON representation</span></span>

<span data-ttu-id="422e5-132">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="422e5-132">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.conversationMember",
  "baseType": "",
  "keyProperty": "id"
}-->

```json
{
  "displayName": "String",
  "id": "String (identifier)",
  "roles": ["String"]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "conversationMember resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->