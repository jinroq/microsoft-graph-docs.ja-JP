---
title: inferenceClassification リソースの種類
description: 'ユーザーにとって、より関連性や重要性があるメッセージに注意が向けられるようにするためのユーザー メッセージの分類です。 '
localization_priority: Normal
ms.openlocfilehash: f06177db9907deb3be38c2cdab82669764503cd6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32549047"
---
# <a name="inferenceclassification-resource-type"></a><span data-ttu-id="1fd4a-103">inferenceClassification リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1fd4a-103">inferenceClassification resource type</span></span>

<span data-ttu-id="1fd4a-104">ユーザーにとって、より関連性や重要性があるメッセージに注意が向けられるようにするためのユーザー メッセージの分類です。</span><span class="sxs-lookup"><span data-stu-id="1fd4a-104">Classification of a user's messages to enable focus on those that are more relevant or important to the user.</span></span> 

<span data-ttu-id="1fd4a-105">詳しくは、「[優先受信トレイを管理する](manage-focused-inbox.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1fd4a-105">For more information, see [Manage Focused Inbox](manage-focused-inbox.md).</span></span>


## <a name="methods"></a><span data-ttu-id="1fd4a-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="1fd4a-106">Methods</span></span>

| <span data-ttu-id="1fd4a-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="1fd4a-107">Method</span></span>           | <span data-ttu-id="1fd4a-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="1fd4a-108">Return Type</span></span>    |<span data-ttu-id="1fd4a-109">説明</span><span class="sxs-lookup"><span data-stu-id="1fd4a-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1fd4a-110">inferenceClassificationOverride を作成する</span><span class="sxs-lookup"><span data-stu-id="1fd4a-110">Create inferenceClassificationOverride</span></span>](../api/inferenceclassification-post-overrides.md) |[<span data-ttu-id="1fd4a-111">inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="1fd4a-111">inferenceClassificationOverride</span></span>](inferenceclassificationoverride.md)| <span data-ttu-id="1fd4a-p101">SMTP アドレスで示される送信者のオーバーライドを作成します。この SMTP アドレスからの将来のメッセージは、オーバーライドで指定されたとおり一貫して分類されます。</span><span class="sxs-lookup"><span data-stu-id="1fd4a-p101">Create an override for a sender identified by an SMTP address. Future messages from that SMTP address will be consistently classified as specified in the override.</span></span>|
|[<span data-ttu-id="1fd4a-114">オーバーライドを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="1fd4a-114">List overrides</span></span>](../api/inferenceclassification-list-overrides.md) |<span data-ttu-id="1fd4a-115">[inferenceClassificationOverride](inferenceclassificationoverride.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="1fd4a-115">[inferenceClassificationOverride](inferenceclassificationoverride.md) collection</span></span>| <span data-ttu-id="1fd4a-116">ユーザーが設定したオーバーライドを取得して、特定の送信者からのメッセージを常に一定の方法で分類します。</span><span class="sxs-lookup"><span data-stu-id="1fd4a-116">Get the overrides that a user has set up to always classify messages from certain senders in specific ways.</span></span>|

## <a name="properties"></a><span data-ttu-id="1fd4a-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1fd4a-117">Properties</span></span>
| <span data-ttu-id="1fd4a-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1fd4a-118">Property</span></span>     | <span data-ttu-id="1fd4a-119">型</span><span class="sxs-lookup"><span data-stu-id="1fd4a-119">Type</span></span>   |<span data-ttu-id="1fd4a-120">説明</span><span class="sxs-lookup"><span data-stu-id="1fd4a-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1fd4a-121">id</span><span class="sxs-lookup"><span data-stu-id="1fd4a-121">id</span></span>|<span data-ttu-id="1fd4a-122">string</span><span class="sxs-lookup"><span data-stu-id="1fd4a-122">string</span></span>| <span data-ttu-id="1fd4a-123">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="1fd4a-123">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1fd4a-124">関係</span><span class="sxs-lookup"><span data-stu-id="1fd4a-124">Relationships</span></span>
| <span data-ttu-id="1fd4a-125">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1fd4a-125">Relationship</span></span> | <span data-ttu-id="1fd4a-126">型</span><span class="sxs-lookup"><span data-stu-id="1fd4a-126">Type</span></span>   |<span data-ttu-id="1fd4a-127">説明</span><span class="sxs-lookup"><span data-stu-id="1fd4a-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="1fd4a-128">overrides</span><span class="sxs-lookup"><span data-stu-id="1fd4a-128">overrides</span></span>|<span data-ttu-id="1fd4a-129">[inferenceClassificationOverride](inferenceclassificationoverride.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="1fd4a-129">[inferenceClassificationOverride](inferenceclassificationoverride.md) collection</span></span>| <span data-ttu-id="1fd4a-p102">ユーザーが、`focused` または `other` の特定の方法で特定の差出人からのメッセージを常時分類するための一連のオーバーライド。読み取り専用です。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="1fd4a-p102">A set of overrides for a user to always classify messages from specific senders in certain ways: `focused`, or `other`. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="1fd4a-133">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1fd4a-133">JSON representation</span></span>

<span data-ttu-id="1fd4a-134">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1fd4a-134">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.inferenceClassification",
  "@odata.annotations": [
    {
      "property": "overrides",
      "capabilities": {
        "changeTracking": false,
        "expandable": false,
        "searchable": false
      }
    }
  ]
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
