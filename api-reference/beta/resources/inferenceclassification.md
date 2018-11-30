---
title: inferenceClassification リソースの種類
description: 'ユーザーにとって、より関連性や重要性があるメッセージに注意が向けられるようにするためのユーザー メッセージの分類です。 '
ms.openlocfilehash: c1536ff2b88b1830c2f2a2bc5a7bed519782df4e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066365"
---
# <a name="inferenceclassification-resource-type"></a><span data-ttu-id="d82fb-103">inferenceClassification リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d82fb-103">inferenceClassification resource type</span></span>

> <span data-ttu-id="d82fb-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d82fb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d82fb-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d82fb-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d82fb-106">ユーザーにとって、より関連性や重要性があるメッセージに注意が向けられるようにするためのユーザー メッセージの分類です。</span><span class="sxs-lookup"><span data-stu-id="d82fb-106">Classification of a user's messages to enable focus on those that are more relevant or important to the user.</span></span> 

<span data-ttu-id="d82fb-107">詳しくは、「[優先受信トレイを管理する](manage-focused-inbox.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d82fb-107">For more information, see [Manage Focused Inbox](manage-focused-inbox.md).</span></span>


## <a name="methods"></a><span data-ttu-id="d82fb-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="d82fb-108">Methods</span></span>

| <span data-ttu-id="d82fb-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="d82fb-109">Method</span></span>           | <span data-ttu-id="d82fb-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="d82fb-110">Return Type</span></span>    |<span data-ttu-id="d82fb-111">説明</span><span class="sxs-lookup"><span data-stu-id="d82fb-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d82fb-112">inferenceClassificationOverride を作成する</span><span class="sxs-lookup"><span data-stu-id="d82fb-112">Create inferenceClassificationOverride</span></span>](../api/inferenceclassification-post-overrides.md) |[<span data-ttu-id="d82fb-113">inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="d82fb-113">inferenceClassificationOverride</span></span>](inferenceclassificationoverride.md)| <span data-ttu-id="d82fb-p102">SMTP アドレスで示される送信者のオーバーライドを作成します。この SMTP アドレスからの将来のメッセージは、オーバーライドで指定されたとおり一貫して分類されます。</span><span class="sxs-lookup"><span data-stu-id="d82fb-p102">Create an override for a sender identified by an SMTP address. Future messages from that SMTP address will be consistently classified as specified in the override.</span></span>|
|[<span data-ttu-id="d82fb-116">オーバーライドを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="d82fb-116">List overrides</span></span>](../api/inferenceclassification-list-overrides.md) |<span data-ttu-id="d82fb-117">[inferenceClassificationOverride](inferenceclassificationoverride.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="d82fb-117">[inferenceClassificationOverride](inferenceclassificationoverride.md) collection</span></span>| <span data-ttu-id="d82fb-118">ユーザーが設定したオーバーライドを取得して、特定の送信者からのメッセージを常に一定の方法で分類します。</span><span class="sxs-lookup"><span data-stu-id="d82fb-118">Get the overrides that a user has set up to always classify messages from certain senders in specific ways.</span></span>|

## <a name="properties"></a><span data-ttu-id="d82fb-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d82fb-119">Properties</span></span>
| <span data-ttu-id="d82fb-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d82fb-120">Property</span></span>     | <span data-ttu-id="d82fb-121">型</span><span class="sxs-lookup"><span data-stu-id="d82fb-121">Type</span></span>   |<span data-ttu-id="d82fb-122">説明</span><span class="sxs-lookup"><span data-stu-id="d82fb-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d82fb-123">ID</span><span class="sxs-lookup"><span data-stu-id="d82fb-123">id</span></span>|<span data-ttu-id="d82fb-124">文字列</span><span class="sxs-lookup"><span data-stu-id="d82fb-124">string</span></span>| <span data-ttu-id="d82fb-125">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="d82fb-125">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d82fb-126">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d82fb-126">Relationships</span></span>
| <span data-ttu-id="d82fb-127">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d82fb-127">Relationship</span></span> | <span data-ttu-id="d82fb-128">型</span><span class="sxs-lookup"><span data-stu-id="d82fb-128">Type</span></span>   |<span data-ttu-id="d82fb-129">説明</span><span class="sxs-lookup"><span data-stu-id="d82fb-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d82fb-130">overrides</span><span class="sxs-lookup"><span data-stu-id="d82fb-130">overrides</span></span>|<span data-ttu-id="d82fb-131">[inferenceClassificationOverride](inferenceclassificationoverride.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="d82fb-131">[inferenceClassificationOverride](inferenceclassificationoverride.md) collection</span></span>| <span data-ttu-id="d82fb-p103">ユーザーが、`focused` または `other` の特定の方法で特定の差出人からのメッセージを常時分類するための一連のオーバーライド。読み取り専用です。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="d82fb-p103">A set of overrides for a user to always classify messages from specific senders in certain ways: `focused`, or `other`. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d82fb-135">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d82fb-135">JSON representation</span></span>

<span data-ttu-id="d82fb-136">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d82fb-136">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.inferenceClassification"
}-->

```json
{
  "id": "string (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "inferenceClassification resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->