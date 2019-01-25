---
title: inferenceClassification リソースの種類
description: 'ユーザーにとって、より関連性や重要性があるメッセージに注意が向けられるようにするためのユーザー メッセージの分類です。 '
localization_priority: Normal
ms.openlocfilehash: f06177db9907deb3be38c2cdab82669764503cd6
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510415"
---
# <a name="inferenceclassification-resource-type"></a><span data-ttu-id="082bc-103">inferenceClassification リソースの種類</span><span class="sxs-lookup"><span data-stu-id="082bc-103">inferenceClassification resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="082bc-104">ユーザーにとって、より関連性や重要性があるメッセージに注意が向けられるようにするためのユーザー メッセージの分類です。</span><span class="sxs-lookup"><span data-stu-id="082bc-104">Classification of a user's messages to enable focus on those that are more relevant or important to the user.</span></span> 

<span data-ttu-id="082bc-105">詳しくは、「[優先受信トレイを管理する](manage-focused-inbox.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="082bc-105">For more information, see [Manage Focused Inbox](manage-focused-inbox.md).</span></span>


## <a name="methods"></a><span data-ttu-id="082bc-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="082bc-106">Methods</span></span>

| <span data-ttu-id="082bc-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="082bc-107">Method</span></span>           | <span data-ttu-id="082bc-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="082bc-108">Return Type</span></span>    |<span data-ttu-id="082bc-109">説明</span><span class="sxs-lookup"><span data-stu-id="082bc-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="082bc-110">inferenceClassificationOverride を作成する</span><span class="sxs-lookup"><span data-stu-id="082bc-110">[Create inferenceClassificationOverride](../api/inferenceclassification-post-overrides.md)</span></span> |[<span data-ttu-id="082bc-111">inferenceClassificationOverride</span><span class="sxs-lookup"><span data-stu-id="082bc-111">inferenceClassificationOverride</span></span>](inferenceclassificationoverride.md)| <span data-ttu-id="082bc-p101">SMTP アドレスで示される送信者のオーバーライドを作成します。この SMTP アドレスからの将来のメッセージは、オーバーライドで指定されたとおり一貫して分類されます。</span><span class="sxs-lookup"><span data-stu-id="082bc-p101">Create an override for a sender identified by an SMTP address. Future messages from that SMTP address will be consistently classified as specified in the override.</span></span>|
|<span data-ttu-id="082bc-114">オーバーライドを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="082bc-114">[List overrides](../api/inferenceclassification-list-overrides.md)</span></span> |<span data-ttu-id="082bc-115">inferenceClassificationOverride コレクション</span><span class="sxs-lookup"><span data-stu-id="082bc-115">[inferenceClassificationOverride](inferenceclassificationoverride.md) collection</span></span>| <span data-ttu-id="082bc-116">ユーザーが設定したオーバーライドを取得して、特定の送信者からのメッセージを常に一定の方法で分類します。</span><span class="sxs-lookup"><span data-stu-id="082bc-116">Get the overrides that a user has set up to always classify messages from certain senders in specific ways.</span></span>|

## <a name="properties"></a><span data-ttu-id="082bc-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="082bc-117">Properties</span></span>
| <span data-ttu-id="082bc-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="082bc-118">Property</span></span>     | <span data-ttu-id="082bc-119">型</span><span class="sxs-lookup"><span data-stu-id="082bc-119">Type</span></span>   |<span data-ttu-id="082bc-120">説明</span><span class="sxs-lookup"><span data-stu-id="082bc-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="082bc-121">id</span><span class="sxs-lookup"><span data-stu-id="082bc-121">id</span></span>|<span data-ttu-id="082bc-122">string</span><span class="sxs-lookup"><span data-stu-id="082bc-122">string</span></span>| <span data-ttu-id="082bc-123">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="082bc-123">Read-only.</span></span>|

## <a name="relationships"></a><span data-ttu-id="082bc-124">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="082bc-124">Relationships</span></span>
| <span data-ttu-id="082bc-125">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="082bc-125">Relationship</span></span> | <span data-ttu-id="082bc-126">型</span><span class="sxs-lookup"><span data-stu-id="082bc-126">Type</span></span>   |<span data-ttu-id="082bc-127">説明</span><span class="sxs-lookup"><span data-stu-id="082bc-127">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="082bc-128">overrides</span><span class="sxs-lookup"><span data-stu-id="082bc-128">overrides</span></span>|<span data-ttu-id="082bc-129">inferenceClassificationOverride コレクション</span><span class="sxs-lookup"><span data-stu-id="082bc-129">[inferenceClassificationOverride](inferenceclassificationoverride.md) collection</span></span>| <span data-ttu-id="082bc-p102">ユーザーが、`focused` または `other` の特定の方法で特定の差出人からのメッセージを常時分類するための一連のオーバーライド。読み取り専用です。Null 許容型。</span><span class="sxs-lookup"><span data-stu-id="082bc-p102">A set of overrides for a user to always classify messages from specific senders in certain ways: `focused`, or `other`. Read-only. Nullable.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="082bc-133">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="082bc-133">JSON representation</span></span>

<span data-ttu-id="082bc-134">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="082bc-134">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "inferenceClassification resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/inferenceclassification.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
