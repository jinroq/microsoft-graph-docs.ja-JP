---
title: multiValueLegacyExtendedProperty リソースの種類
description: 値のコレクションが含まれる拡張プロパティ。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: e513925810d7357f131790445a015be6c193624f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036009"
---
# <a name="multivaluelegacyextendedproperty-resource-type"></a><span data-ttu-id="d7d16-103">multiValueLegacyExtendedProperty リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d7d16-103">multiValueLegacyExtendedProperty resource type</span></span>

<span data-ttu-id="d7d16-104">値のコレクションが含まれる拡張プロパティ。</span><span class="sxs-lookup"><span data-stu-id="d7d16-104">An extended property that contains a collection of values.</span></span>

<span data-ttu-id="d7d16-105">オープン拡張機能または拡張プロパティを使用するのに適した状況と、拡張プロパティを指定する方法の詳細については、「[拡張プロパティの概要](../resources/extended-properties-overview.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d7d16-105">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="methods"></a><span data-ttu-id="d7d16-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="d7d16-106">Methods</span></span>

| <span data-ttu-id="d7d16-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="d7d16-107">Method</span></span>           | <span data-ttu-id="d7d16-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="d7d16-108">Return Type</span></span>    |<span data-ttu-id="d7d16-109">説明</span><span class="sxs-lookup"><span data-stu-id="d7d16-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="d7d16-110">Post</span><span class="sxs-lookup"><span data-stu-id="d7d16-110">Post</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | <span data-ttu-id="d7d16-p101">サポートされているリソース インスタンス: [メッセージ](../resources/message.md)、[mailFolder](../resources/mailfolder.md)、[イベント](../resources/event.md)、[予定表](../resources/calendar.md)、[連絡先](../resources/contact.md)、または [contactFolder](../resources/contactfolder.md)。グループ[投稿](../resources/post.md) はサポートされていませんので、ご注意ください。</span><span class="sxs-lookup"><span data-stu-id="d7d16-p101">A supported resource instance: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), or [contactFolder](../resources/contactfolder.md). Note that group [post](../resources/post.md) is not supported.</span></span> | <span data-ttu-id="d7d16-113">サポートされているリソースの新しいインスタンスまたは既存のインスタンスに **multiValueLegacyExtendedProperty** を作成します。</span><span class="sxs-lookup"><span data-stu-id="d7d16-113">Create a **multiValueLegacyExtendedProperty** in a new or existing instance of a supported resource.</span></span> |
|[<span data-ttu-id="d7d16-114">Get</span><span class="sxs-lookup"><span data-stu-id="d7d16-114">Get</span></span>](../api/multivaluelegacyextendedproperty-get.md) |<span data-ttu-id="d7d16-115">[multiValueLegacyExtendedProperty](../resources/message.md) オブジェクトで拡張されたサポートされているリソースのインスタンス ([メッセージ](../resources/mailfolder.md)、[mailFolder](../resources/event.md)、[イベント](../resources/calendar.md)、[予定表](../resources/contact.md)、[連絡先](../resources/contactfolder.md)、[contactFolder](../resources/post.md)、またはグループ[投稿](multivaluelegacyextendedproperty.md))。</span><span class="sxs-lookup"><span data-stu-id="d7d16-115">A supported resource instance ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), or group [post](../resources/post.md)) expanded with a [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) object.</span></span> |<span data-ttu-id="d7d16-116">`$expand` を使用して拡張プロパティでリソース インスタンスを取得します。</span><span class="sxs-lookup"><span data-stu-id="d7d16-116">Get a resource instance with an extended property using `$expand`.</span></span>|

## <a name="properties"></a><span data-ttu-id="d7d16-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d7d16-117">Properties</span></span>
| <span data-ttu-id="d7d16-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d7d16-118">Property</span></span>     | <span data-ttu-id="d7d16-119">型</span><span class="sxs-lookup"><span data-stu-id="d7d16-119">Type</span></span>   |<span data-ttu-id="d7d16-120">説明</span><span class="sxs-lookup"><span data-stu-id="d7d16-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d7d16-121">id</span><span class="sxs-lookup"><span data-stu-id="d7d16-121">id</span></span>|<span data-ttu-id="d7d16-122">string</span><span class="sxs-lookup"><span data-stu-id="d7d16-122">string</span></span>|<span data-ttu-id="d7d16-p102">プロパティ識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="d7d16-p102">The property identifier. Read-only.</span></span>|
|<span data-ttu-id="d7d16-125">value</span><span class="sxs-lookup"><span data-stu-id="d7d16-125">value</span></span>|<span data-ttu-id="d7d16-126">string collection</span><span class="sxs-lookup"><span data-stu-id="d7d16-126">string collection</span></span>|<span data-ttu-id="d7d16-127">プロパティ値のコレクション。</span><span class="sxs-lookup"><span data-stu-id="d7d16-127">A collection of property values.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d7d16-128">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d7d16-128">Relationships</span></span>
<span data-ttu-id="d7d16-129">なし</span><span class="sxs-lookup"><span data-stu-id="d7d16-129">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="d7d16-130">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d7d16-130">JSON representation</span></span>

<span data-ttu-id="d7d16-131">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d7d16-131">Here is a JSON representation of the resource.</span></span>

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
