---
title: inferenceClassification リソースの種類
description: 'ユーザーにとって、より関連性や重要性があるメッセージに注意が向けられるようにするためのユーザー メッセージの分類です。 '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: bf1ea3b61df2166f58f161b804f55e87e474be97
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36006270"
---
# <a name="inferenceclassification-resource-type"></a><span data-ttu-id="64df6-103">inferenceClassification リソースの種類</span><span class="sxs-lookup"><span data-stu-id="64df6-103">inferenceClassification resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="64df6-104">ユーザーにとって、より関連性や重要性があるメッセージに注意が向けられるようにするためのユーザー メッセージの分類です。</span><span class="sxs-lookup"><span data-stu-id="64df6-104">Classification of a user's messages to enable focus on those that are more relevant or important to the user.</span></span> 

<span data-ttu-id="64df6-105">詳しくは、「[優先受信トレイを管理する](manage-focused-inbox.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="64df6-105">For more information, see [Manage Focused Inbox](manage-focused-inbox.md).</span></span>


## <a name="methods"></a><span data-ttu-id="64df6-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="64df6-106">Methods</span></span>

| <span data-ttu-id="64df6-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="64df6-107">Method</span></span>           | <span data-ttu-id="64df6-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="64df6-108">Return Type</span></span>    |<span data-ttu-id="64df6-109">説明</span><span class="sxs-lookup"><span data-stu-id="64df6-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="64df6-110">inferenceClassificationOverride を作成する</span><span class="sxs-lookup"><span data-stu-id="64df6-110">Create inferenceClassificationOverride</span></span>](../api/inferenceclassification-post-overrides.md) |[<span data-ttu-id="64df6-111">inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="64df6-111">inferenceClassificationOverride</span></span>](inferenceclassificationoverride.md)| <span data-ttu-id="64df6-p101">SMTP アドレスで示される送信者のオーバーライドを作成します。この SMTP アドレスからの将来のメッセージは、オーバーライドで指定されたとおり一貫して分類されます。</span><span class="sxs-lookup"><span data-stu-id="64df6-p101">Create an override for a sender identified by an SMTP address. Future messages from that SMTP address will be consistently classified as specified in the override.</span></span>|
|[<span data-ttu-id="64df6-114">オーバーライドを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="64df6-114">List overrides</span></span>](../api/inferenceclassification-list-overrides.md) |<span data-ttu-id="64df6-115">[inferenceClassificationOverride](inferenceclassificationoverride.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="64df6-115">[inferenceClassificationOverride](inferenceclassificationoverride.md) collection</span></span>| <span data-ttu-id="64df6-116">ユーザーが設定したオーバーライドを取得して、特定の送信者からのメッセージを常に一定の方法で分類します。</span><span class="sxs-lookup"><span data-stu-id="64df6-116">Get the overrides that a user has set up to always classify messages from certain senders in specific ways.</span></span>|

## <a name="properties"></a><span data-ttu-id="64df6-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="64df6-117">Properties</span></span>
| <span data-ttu-id="64df6-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="64df6-118">Property</span></span>     | <span data-ttu-id="64df6-119">型</span><span class="sxs-lookup"><span data-stu-id="64df6-119">Type</span></span>   |<span data-ttu-id="64df6-120">説明</span><span class="sxs-lookup"><span data-stu-id="64df6-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="64df6-121">id</span><span class="sxs-lookup"><span data-stu-id="64df6-121">id</span></span>|<span data-ttu-id="64df6-122">string</span><span class="sxs-lookup"><span data-stu-id="64df6-122">string</span></span>| <span data-ttu-id="64df6-123">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="64df6-123">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="64df6-124">関係</span><span class="sxs-lookup"><span data-stu-id="64df6-124">Relationships</span></span>
| <span data-ttu-id="64df6-125">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="64df6-125">Relationship</span></span> | <span data-ttu-id="64df6-126">型</span><span class="sxs-lookup"><span data-stu-id="64df6-126">Type</span></span>   |<span data-ttu-id="64df6-127">説明</span><span class="sxs-lookup"><span data-stu-id="64df6-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="64df6-128">overrides</span><span class="sxs-lookup"><span data-stu-id="64df6-128">overrides</span></span>|<span data-ttu-id="64df6-129">[inferenceClassificationOverride](inferenceclassificationoverride.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="64df6-129">[inferenceClassificationOverride](inferenceclassificationoverride.md) collection</span></span>| <span data-ttu-id="64df6-p102">ユーザーが、`focused` または `other` の特定の方法で特定の差出人からのメッセージを常時分類するための一連のオーバーライド。読み取り専用です。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="64df6-p102">A set of overrides for a user to always classify messages from specific senders in certain ways: `focused`, or `other`. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="64df6-133">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="64df6-133">JSON representation</span></span>

<span data-ttu-id="64df6-134">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="64df6-134">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "keyProperty": "id",
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
<!--
{
  "type": "#page.annotation",
  "description": "inferenceClassification resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
