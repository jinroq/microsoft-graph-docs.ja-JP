---
title: singleValueLegacyExtendedProperty リソースの種類
description: '単一値が含まれる拡張プロパティ。 '
localization_priority: Normal
ms.openlocfilehash: f865da1a8a4211ac99a70881b2851b38b8e72727
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27894230"
---
# <a name="singlevaluelegacyextendedproperty-resource-type"></a><span data-ttu-id="b6e65-103">singleValueLegacyExtendedProperty リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b6e65-103">singleValueLegacyExtendedProperty resource type</span></span>

<span data-ttu-id="b6e65-104">単一値が含まれる拡張プロパティ。</span><span class="sxs-lookup"><span data-stu-id="b6e65-104">An extended property that contains a single value.</span></span> 

<span data-ttu-id="b6e65-105">オープン拡張機能または拡張プロパティを使用するのに適した状況と、拡張プロパティを指定する方法の詳細については、「[拡張プロパティの概要](../resources/extended-properties-overview.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b6e65-105">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span> 


## <a name="methods"></a><span data-ttu-id="b6e65-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="b6e65-106">Methods</span></span>

| <span data-ttu-id="b6e65-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="b6e65-107">Method</span></span>           | <span data-ttu-id="b6e65-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="b6e65-108">Return Type</span></span>    |<span data-ttu-id="b6e65-109">説明</span><span class="sxs-lookup"><span data-stu-id="b6e65-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="b6e65-110">Post</span><span class="sxs-lookup"><span data-stu-id="b6e65-110">Post</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) | <span data-ttu-id="b6e65-111">サポートされているリソース インスタンス: [メッセージ](../resources/message.md)、[mailFolder](../resources/mailfolder.md)、[イベント](../resources/event.md)、[予定表](../resources/calendar.md)、[連絡先](../resources/contact.md)、または [contactFolder](../resources/contactfolder.md) (ただし、グループ[投稿](../resources/post.md)を除く)。</span><span class="sxs-lookup"><span data-stu-id="b6e65-111">A supported resource instance: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), or [contactFolder](../resources/contactfolder.md), but not group [post](../resources/post.md).</span></span> | <span data-ttu-id="b6e65-112">サポートされているリソースの新しいインスタンスまたは既存のインスタンスに **singleValueLegacyExtendedProperty** を作成します。</span><span class="sxs-lookup"><span data-stu-id="b6e65-112">Create a **singleValueLegacyExtendedProperty** in a new or existing instance of a supported resource.</span></span> |
|[<span data-ttu-id="b6e65-113">Get</span><span class="sxs-lookup"><span data-stu-id="b6e65-113">Get</span></span>](../api/singlevaluelegacyextendedproperty-get.md) |<span data-ttu-id="b6e65-114">サポートされているリソースのインスタンス ([メッセージ](../resources/message.md)、[mailFolder](../resources/mailfolder.md)、[イベント](../resources/event.md)、[予定表](../resources/calendar.md)、[連絡先](../resources/contact.md)、[contactFolder](../resources/contactfolder.md)、またはグループ[投稿](../resources/post.md)) のいずれか、またはそれらのコレクション、あるいは [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) オブジェクトで拡張されているインスタンスなどのいずれか。</span><span class="sxs-lookup"><span data-stu-id="b6e65-114">One or a collection of supported resource instance ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), or group [post](../resources/post.md)), or one such instance expanded with a [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) object.</span></span> |<span data-ttu-id="b6e65-115">`$expand` または `$filter` を使用して拡張プロパティでリソース インスタンスを取得します。</span><span class="sxs-lookup"><span data-stu-id="b6e65-115">Get a resource instance with an extended property using `$expand` or `$filter`.</span></span>|

## <a name="properties"></a><span data-ttu-id="b6e65-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b6e65-116">Properties</span></span>
| <span data-ttu-id="b6e65-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b6e65-117">Property</span></span>     | <span data-ttu-id="b6e65-118">種類</span><span class="sxs-lookup"><span data-stu-id="b6e65-118">Type</span></span>   |<span data-ttu-id="b6e65-119">説明</span><span class="sxs-lookup"><span data-stu-id="b6e65-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b6e65-120">ID</span><span class="sxs-lookup"><span data-stu-id="b6e65-120">id</span></span>|<span data-ttu-id="b6e65-121">文字列</span><span class="sxs-lookup"><span data-stu-id="b6e65-121">string</span></span>|<span data-ttu-id="b6e65-p101">プロパティの識別に使用されるプロパティ ID。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b6e65-p101">The property ID used to identify the property. Read-only.</span></span>|
|<span data-ttu-id="b6e65-124">value</span><span class="sxs-lookup"><span data-stu-id="b6e65-124">value</span></span>|<span data-ttu-id="b6e65-125">文字列</span><span class="sxs-lookup"><span data-stu-id="b6e65-125">string</span></span>|<span data-ttu-id="b6e65-126">プロパティ値。</span><span class="sxs-lookup"><span data-stu-id="b6e65-126">A property value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="b6e65-127">関係</span><span class="sxs-lookup"><span data-stu-id="b6e65-127">Relationships</span></span>
<span data-ttu-id="b6e65-128">なし</span><span class="sxs-lookup"><span data-stu-id="b6e65-128">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="b6e65-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b6e65-129">JSON representation</span></span>

<span data-ttu-id="b6e65-130">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b6e65-130">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "optionalProperties": [],
  "baseType": "microsoft.graph.entity",
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
