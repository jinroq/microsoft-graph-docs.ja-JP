---
title: inferenceClassification リソースの種類
description: 'ユーザーにとって、より関連性や重要性があるメッセージに注意が向けられるようにするためのユーザー メッセージの分類です。 '
localization_priority: Normal
ms.openlocfilehash: 82d16e24e21231b8ec168eda793257ef780c2219
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27877792"
---
# <a name="inferenceclassification-resource-type"></a><span data-ttu-id="55ab7-103">inferenceClassification リソースの種類</span><span class="sxs-lookup"><span data-stu-id="55ab7-103">inferenceClassification resource type</span></span>

> <span data-ttu-id="55ab7-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="55ab7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="55ab7-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="55ab7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="55ab7-106">ユーザーにとって、より関連性や重要性があるメッセージに注意が向けられるようにするためのユーザー メッセージの分類です。</span><span class="sxs-lookup"><span data-stu-id="55ab7-106">Classification of a user's messages to enable focus on those that are more relevant or important to the user.</span></span> 

<span data-ttu-id="55ab7-107">詳しくは、「[優先受信トレイを管理する](manage-focused-inbox.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="55ab7-107">For more information, see [Manage Focused Inbox](manage-focused-inbox.md).</span></span>


## <a name="methods"></a><span data-ttu-id="55ab7-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="55ab7-108">Methods</span></span>

| <span data-ttu-id="55ab7-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="55ab7-109">Method</span></span>           | <span data-ttu-id="55ab7-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="55ab7-110">Return Type</span></span>    |<span data-ttu-id="55ab7-111">説明</span><span class="sxs-lookup"><span data-stu-id="55ab7-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="55ab7-112">inferenceClassificationOverride を作成する</span><span class="sxs-lookup"><span data-stu-id="55ab7-112">Create inferenceClassificationOverride</span></span>](../api/inferenceclassification-post-overrides.md) |[<span data-ttu-id="55ab7-113">inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="55ab7-113">inferenceClassificationOverride</span></span>](inferenceclassificationoverride.md)| <span data-ttu-id="55ab7-p102">SMTP アドレスで示される送信者のオーバーライドを作成します。この SMTP アドレスからの将来のメッセージは、オーバーライドで指定されたとおり一貫して分類されます。</span><span class="sxs-lookup"><span data-stu-id="55ab7-p102">Create an override for a sender identified by an SMTP address. Future messages from that SMTP address will be consistently classified as specified in the override.</span></span>|
|[<span data-ttu-id="55ab7-116">オーバーライドを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="55ab7-116">List overrides</span></span>](../api/inferenceclassification-list-overrides.md) |<span data-ttu-id="55ab7-117">[inferenceClassificationOverride](inferenceclassificationoverride.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="55ab7-117">[inferenceClassificationOverride](inferenceclassificationoverride.md) collection</span></span>| <span data-ttu-id="55ab7-118">ユーザーが設定したオーバーライドを取得して、特定の送信者からのメッセージを常に一定の方法で分類します。</span><span class="sxs-lookup"><span data-stu-id="55ab7-118">Get the overrides that a user has set up to always classify messages from certain senders in specific ways.</span></span>|

## <a name="properties"></a><span data-ttu-id="55ab7-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="55ab7-119">Properties</span></span>
| <span data-ttu-id="55ab7-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="55ab7-120">Property</span></span>     | <span data-ttu-id="55ab7-121">種類</span><span class="sxs-lookup"><span data-stu-id="55ab7-121">Type</span></span>   |<span data-ttu-id="55ab7-122">説明</span><span class="sxs-lookup"><span data-stu-id="55ab7-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="55ab7-123">ID</span><span class="sxs-lookup"><span data-stu-id="55ab7-123">id</span></span>|<span data-ttu-id="55ab7-124">文字列</span><span class="sxs-lookup"><span data-stu-id="55ab7-124">string</span></span>| <span data-ttu-id="55ab7-125">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="55ab7-125">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="55ab7-126">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="55ab7-126">Relationships</span></span>
| <span data-ttu-id="55ab7-127">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="55ab7-127">Relationship</span></span> | <span data-ttu-id="55ab7-128">型</span><span class="sxs-lookup"><span data-stu-id="55ab7-128">Type</span></span>   |<span data-ttu-id="55ab7-129">説明</span><span class="sxs-lookup"><span data-stu-id="55ab7-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="55ab7-130">overrides</span><span class="sxs-lookup"><span data-stu-id="55ab7-130">overrides</span></span>|<span data-ttu-id="55ab7-131">[inferenceClassificationOverride](inferenceclassificationoverride.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="55ab7-131">[inferenceClassificationOverride](inferenceclassificationoverride.md) collection</span></span>| <span data-ttu-id="55ab7-p103">ユーザーが、`focused` または `other` の特定の方法で特定の差出人からのメッセージを常時分類するための一連のオーバーライド。読み取り専用です。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="55ab7-p103">A set of overrides for a user to always classify messages from specific senders in certain ways: `focused`, or `other`. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="55ab7-135">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="55ab7-135">JSON representation</span></span>

<span data-ttu-id="55ab7-136">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="55ab7-136">Here is a JSON representation of the resource.</span></span>

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
