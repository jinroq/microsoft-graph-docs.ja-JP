---
title: multiValueLegacyExtendedProperty リソースの種類
description: 値のコレクションが含まれる拡張プロパティ。
localization_priority: Normal
ms.openlocfilehash: e98963eea5e1e996170f6330b9b4b333a72ad159
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27839453"
---
# <a name="multivaluelegacyextendedproperty-resource-type"></a><span data-ttu-id="8f2de-103">multiValueLegacyExtendedProperty リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8f2de-103">multiValueLegacyExtendedProperty resource type</span></span>

> <span data-ttu-id="8f2de-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8f2de-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="8f2de-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8f2de-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="8f2de-106">値のコレクションが含まれる拡張プロパティ。</span><span class="sxs-lookup"><span data-stu-id="8f2de-106">An extended property that contains a collection of values.</span></span>

<span data-ttu-id="8f2de-107">オープン拡張機能または拡張プロパティを使用するのに適した状況と、拡張プロパティを指定する方法の詳細については、「[拡張プロパティの概要](../resources/extended-properties-overview.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8f2de-107">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="methods"></a><span data-ttu-id="8f2de-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="8f2de-108">Methods</span></span>

| <span data-ttu-id="8f2de-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="8f2de-109">Method</span></span>           | <span data-ttu-id="8f2de-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="8f2de-110">Return Type</span></span>    |<span data-ttu-id="8f2de-111">説明</span><span class="sxs-lookup"><span data-stu-id="8f2de-111">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="8f2de-112">Post</span><span class="sxs-lookup"><span data-stu-id="8f2de-112">Post</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | <span data-ttu-id="8f2de-113">サポートされているリソース インスタンス:[メッセージ](../resources/message.md)、 [mailFolder](../resources/mailfolder.md)、[イベント](../resources/event.md)、[予定表](../resources/calendar.md)、[お問い合わせください](../resources/contact.md)、 [contactFolder](../resources/contactfolder.md)、 [Outlook のタスク](../resources/outlooktask.md)、または[Outlook の仕事フォルダー](../resources/outlooktaskfolder.md)。</span><span class="sxs-lookup"><span data-stu-id="8f2de-113">A supported resource instance: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [Outlook task](../resources/outlooktask.md), or [Outlook task folder](../resources/outlooktaskfolder.md).</span></span> <span data-ttu-id="8f2de-114">そのグループの[送信](../resources/post.md)はサポートされていません注意してください。</span><span class="sxs-lookup"><span data-stu-id="8f2de-114">Note that group [post](../resources/post.md) is not supported.</span></span> | <span data-ttu-id="8f2de-115">サポートされているリソースの新しいインスタンスまたは既存のインスタンスに **multiValueLegacyExtendedProperty** を作成します。</span><span class="sxs-lookup"><span data-stu-id="8f2de-115">Create a **multiValueLegacyExtendedProperty** in a new or existing instance of a supported resource.</span></span> |
|[<span data-ttu-id="8f2de-116">Get</span><span class="sxs-lookup"><span data-stu-id="8f2de-116">Get</span></span>](../api/multivaluelegacyextendedproperty-get.md) |<span data-ttu-id="8f2de-117">([メッセージ](../resources/message.md)、 [mailFolder](../resources/mailfolder.md)、[イベント](../resources/event.md)、[予定表](../resources/calendar.md)[にお問い合わせください](../resources/contact.md)、 [contactFolder](../resources/contactfolder.md) [Outlook の仕事](../resources/outlooktask.md)、 [Outlook の仕事フォルダー](../resources/outlooktaskfolder.md)、またはグループの[転記](../resources/post.md))、サポートされているリソースのインスタンスは、[と展開multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="8f2de-117">A supported resource instance ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [Outlook task](../resources/outlooktask.md), [Outlook task folder](../resources/outlooktaskfolder.md), or group [post](../resources/post.md)) expanded with a [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) object.</span></span> |<span data-ttu-id="8f2de-118">`$expand` を使用して拡張プロパティでリソース インスタンスを取得します。</span><span class="sxs-lookup"><span data-stu-id="8f2de-118">Get a resource instance with an extended property using `$expand`.</span></span>|

## <a name="properties"></a><span data-ttu-id="8f2de-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8f2de-119">Properties</span></span>
| <span data-ttu-id="8f2de-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8f2de-120">Property</span></span>     | <span data-ttu-id="8f2de-121">種類</span><span class="sxs-lookup"><span data-stu-id="8f2de-121">Type</span></span>   |<span data-ttu-id="8f2de-122">説明</span><span class="sxs-lookup"><span data-stu-id="8f2de-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="8f2de-123">ID</span><span class="sxs-lookup"><span data-stu-id="8f2de-123">id</span></span>|<span data-ttu-id="8f2de-124">文字列</span><span class="sxs-lookup"><span data-stu-id="8f2de-124">string</span></span>|<span data-ttu-id="8f2de-p103">プロパティ識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="8f2de-p103">The property identifier. Read-only.</span></span>|
|<span data-ttu-id="8f2de-127">value</span><span class="sxs-lookup"><span data-stu-id="8f2de-127">value</span></span>|<span data-ttu-id="8f2de-128">string collection</span><span class="sxs-lookup"><span data-stu-id="8f2de-128">string collection</span></span>|<span data-ttu-id="8f2de-129">プロパティ値のコレクション。</span><span class="sxs-lookup"><span data-stu-id="8f2de-129">A collection of property values.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8f2de-130">関係</span><span class="sxs-lookup"><span data-stu-id="8f2de-130">Relationships</span></span>
<span data-ttu-id="8f2de-131">なし</span><span class="sxs-lookup"><span data-stu-id="8f2de-131">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="8f2de-132">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8f2de-132">JSON representation</span></span>

<span data-ttu-id="8f2de-133">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8f2de-133">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.multivaluelegacyextendedproperty"
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
