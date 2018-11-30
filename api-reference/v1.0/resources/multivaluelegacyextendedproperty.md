---
title: multiValueLegacyExtendedProperty リソースの種類
description: 値のコレクションが含まれる拡張プロパティ。
ms.openlocfilehash: 9aa94465ca1a0fb30c4461b99336040c72e2c5c0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27021467"
---
# <a name="multivaluelegacyextendedproperty-resource-type"></a><span data-ttu-id="9b11f-103">multiValueLegacyExtendedProperty リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9b11f-103">multiValueLegacyExtendedProperty resource type</span></span>

<span data-ttu-id="9b11f-104">値のコレクションが含まれる拡張プロパティ。</span><span class="sxs-lookup"><span data-stu-id="9b11f-104">An extended property that contains a collection of values.</span></span>

<span data-ttu-id="9b11f-105">オープン拡張機能または拡張プロパティを使用するのに適した状況と、拡張プロパティを指定する方法の詳細については、「[拡張プロパティの概要](../resources/extended-properties-overview.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9b11f-105">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="methods"></a><span data-ttu-id="9b11f-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="9b11f-106">Methods</span></span>

| <span data-ttu-id="9b11f-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="9b11f-107">Method</span></span>           | <span data-ttu-id="9b11f-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="9b11f-108">Return Type</span></span>    |<span data-ttu-id="9b11f-109">説明</span><span class="sxs-lookup"><span data-stu-id="9b11f-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="9b11f-110">Post</span><span class="sxs-lookup"><span data-stu-id="9b11f-110">Post</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | <span data-ttu-id="9b11f-p101">サポートされているリソース インスタンス: [メッセージ](../resources/message.md)、[mailFolder](../resources/mailfolder.md)、[イベント](../resources/event.md)、[予定表](../resources/calendar.md)、[連絡先](../resources/contact.md)、または [contactFolder](../resources/contactfolder.md)。グループ[投稿](../resources/post.md) はサポートされていませんので、ご注意ください。</span><span class="sxs-lookup"><span data-stu-id="9b11f-p101">A supported resource instance: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), or [contactFolder](../resources/contactfolder.md). Note that group [post](../resources/post.md) is not supported.</span></span> | <span data-ttu-id="9b11f-113">サポートされているリソースの新しいインスタンスまたは既存のインスタンスに **multiValueLegacyExtendedProperty** を作成します。</span><span class="sxs-lookup"><span data-stu-id="9b11f-113">Create a **multiValueLegacyExtendedProperty** in a new or existing instance of a supported resource.</span></span> |
|[<span data-ttu-id="9b11f-114">Get</span><span class="sxs-lookup"><span data-stu-id="9b11f-114">Get</span></span>](../api/multivaluelegacyextendedproperty-get.md) |<span data-ttu-id="9b11f-115">[multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) オブジェクトで拡張されたサポートされているリソースのインスタンス ([メッセージ](../resources/message.md)、[mailFolder](../resources/mailfolder.md)、[イベント](../resources/event.md)、[予定表](../resources/calendar.md)、[連絡先](../resources/contact.md)、[contactFolder](../resources/contactfolder.md)、またはグループ[投稿](../resources/post.md))。</span><span class="sxs-lookup"><span data-stu-id="9b11f-115">A supported resource instance ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), or group [post](../resources/post.md)) expanded with a [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) object.</span></span> |<span data-ttu-id="9b11f-116">`$expand` を使用して拡張プロパティでリソース インスタンスを取得します。</span><span class="sxs-lookup"><span data-stu-id="9b11f-116">Get a resource instance with an extended property using `$expand`.</span></span>|

## <a name="properties"></a><span data-ttu-id="9b11f-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9b11f-117">Properties</span></span>
| <span data-ttu-id="9b11f-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9b11f-118">Property</span></span>     | <span data-ttu-id="9b11f-119">型</span><span class="sxs-lookup"><span data-stu-id="9b11f-119">Type</span></span>   |<span data-ttu-id="9b11f-120">説明</span><span class="sxs-lookup"><span data-stu-id="9b11f-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9b11f-121">ID</span><span class="sxs-lookup"><span data-stu-id="9b11f-121">id</span></span>|<span data-ttu-id="9b11f-122">文字列</span><span class="sxs-lookup"><span data-stu-id="9b11f-122">string</span></span>|<span data-ttu-id="9b11f-p102">プロパティ識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="9b11f-p102">The property identifier. Read-only.</span></span>|
|<span data-ttu-id="9b11f-125">value</span><span class="sxs-lookup"><span data-stu-id="9b11f-125">value</span></span>|<span data-ttu-id="9b11f-126">string collection</span><span class="sxs-lookup"><span data-stu-id="9b11f-126">string collection</span></span>|<span data-ttu-id="9b11f-127">プロパティ値のコレクション。</span><span class="sxs-lookup"><span data-stu-id="9b11f-127">A collection of property values.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9b11f-128">関係</span><span class="sxs-lookup"><span data-stu-id="9b11f-128">Relationships</span></span>
<span data-ttu-id="9b11f-129">なし</span><span class="sxs-lookup"><span data-stu-id="9b11f-129">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="9b11f-130">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9b11f-130">JSON representation</span></span>

<span data-ttu-id="9b11f-131">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="9b11f-131">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.multiValueLegacyExtendedProperty"
}-->

```json
{
  "id": "string (identifier)",
  "value": ["string"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "multiValueLegacyExtendedProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->