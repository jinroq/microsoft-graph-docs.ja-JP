---
title: singleValueLegacyExtendedProperty リソースの種類
description: '単一値が含まれる拡張プロパティ。 '
ms.openlocfilehash: 1b9eeaa05ee15aab30c1761cd35f70f586dffb24
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073323"
---
# <a name="singlevaluelegacyextendedproperty-resource-type"></a><span data-ttu-id="cd67a-103">singleValueLegacyExtendedProperty リソースの種類</span><span class="sxs-lookup"><span data-stu-id="cd67a-103">singleValueLegacyExtendedProperty resource type</span></span>

> <span data-ttu-id="cd67a-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="cd67a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cd67a-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cd67a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cd67a-106">単一値が含まれる拡張プロパティ。</span><span class="sxs-lookup"><span data-stu-id="cd67a-106">An extended property that contains a single value.</span></span> 

<span data-ttu-id="cd67a-107">オープン拡張機能または拡張プロパティを使用するのに適した状況と、拡張プロパティを指定する方法の詳細については、「[拡張プロパティの概要](../resources/extended-properties-overview.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cd67a-107">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span> 


## <a name="methods"></a><span data-ttu-id="cd67a-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="cd67a-108">Methods</span></span>

| <span data-ttu-id="cd67a-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="cd67a-109">Method</span></span>           | <span data-ttu-id="cd67a-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="cd67a-110">Return Type</span></span>    |<span data-ttu-id="cd67a-111">説明</span><span class="sxs-lookup"><span data-stu-id="cd67a-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="cd67a-112">Post</span><span class="sxs-lookup"><span data-stu-id="cd67a-112">Post</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) | <span data-ttu-id="cd67a-113">サポートされているリソース インスタンス:[メッセージ](../resources/message.md)、 [mailFolder](../resources/mailfolder.md)、[イベント](../resources/event.md)、[予定表](../resources/calendar.md)[にお問い合わせください](../resources/contact.md)、 [contactFolder](../resources/contactfolder.md)、 [Outlook の仕事](../resources/outlooktask.md)または[Outlook の仕事フォルダー](../resources/outlooktaskfolder.md)、ですが、グループに[投稿](../resources/post.md)がありません。</span><span class="sxs-lookup"><span data-stu-id="cd67a-113">A supported resource instance: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [Outlook task](../resources/outlooktask.md), or [Outlook task folder](../resources/outlooktaskfolder.md), but not group [post](../resources/post.md).</span></span> | <span data-ttu-id="cd67a-114">サポートされているリソースの新しいインスタンスまたは既存のインスタンスに **singleValueLegacyExtendedProperty** を作成します。</span><span class="sxs-lookup"><span data-stu-id="cd67a-114">Create a **singleValueLegacyExtendedProperty** in a new or existing instance of a supported resource.</span></span> |
|[<span data-ttu-id="cd67a-115">Get</span><span class="sxs-lookup"><span data-stu-id="cd67a-115">Get</span></span>](../api/singlevaluelegacyextendedproperty-get.md) |<span data-ttu-id="cd67a-116">([メッセージ](../resources/message.md)、 [mailFolder](../resources/mailfolder.md)、[イベント](../resources/event.md)、[予定表](../resources/calendar.md)[にお問い合わせください](../resources/contact.md)、 [contactFolder](../resources/contactfolder.md) [Outlook の仕事](../resources/outlooktask.md)、 [Outlook の仕事フォルダー](../resources/outlooktaskfolder.md)、またはグループの[転記](../resources/post.md))、サポートされているリソースのインスタンスのコレクションの 1 つまたはまたは、このような 1 つのインスタンスは、 [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)オブジェクトを使用して展開します。</span><span class="sxs-lookup"><span data-stu-id="cd67a-116">One or a collection of supported resource instance ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [Outlook task](../resources/outlooktask.md), [Outlook task folder](../resources/outlooktaskfolder.md), or group [post](../resources/post.md)), or one such instance expanded with a [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) object.</span></span> |<span data-ttu-id="cd67a-117">`$expand` または `$filter` を使用して拡張プロパティでリソース インスタンスを取得します。</span><span class="sxs-lookup"><span data-stu-id="cd67a-117">Get a resource instance with an extended property using `$expand` or `$filter`.</span></span>|

## <a name="properties"></a><span data-ttu-id="cd67a-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cd67a-118">Properties</span></span>
| <span data-ttu-id="cd67a-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cd67a-119">Property</span></span>     | <span data-ttu-id="cd67a-120">型</span><span class="sxs-lookup"><span data-stu-id="cd67a-120">Type</span></span>   |<span data-ttu-id="cd67a-121">説明</span><span class="sxs-lookup"><span data-stu-id="cd67a-121">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cd67a-122">ID</span><span class="sxs-lookup"><span data-stu-id="cd67a-122">id</span></span>|<span data-ttu-id="cd67a-123">string</span><span class="sxs-lookup"><span data-stu-id="cd67a-123">string</span></span>|<span data-ttu-id="cd67a-p102">プロパティ識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="cd67a-p102">The property identifier. Read-only.</span></span>|
|<span data-ttu-id="cd67a-126">value</span><span class="sxs-lookup"><span data-stu-id="cd67a-126">value</span></span>|<span data-ttu-id="cd67a-127">文字列</span><span class="sxs-lookup"><span data-stu-id="cd67a-127">string</span></span>|<span data-ttu-id="cd67a-128">プロパティ値。</span><span class="sxs-lookup"><span data-stu-id="cd67a-128">A property value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="cd67a-129">関係</span><span class="sxs-lookup"><span data-stu-id="cd67a-129">Relationships</span></span>
<span data-ttu-id="cd67a-130">なし</span><span class="sxs-lookup"><span data-stu-id="cd67a-130">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="cd67a-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="cd67a-131">JSON representation</span></span>

<span data-ttu-id="cd67a-132">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="cd67a-132">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.singleValueLegacyExtendedProperty"
}-->

```json
{
  "id": "string (identifier)",
  "value": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "singleValueLegacyExtendedProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->