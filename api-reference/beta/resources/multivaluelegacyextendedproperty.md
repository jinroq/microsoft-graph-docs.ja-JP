---
title: multiValueLegacyExtendedProperty リソースの種類
description: 値のコレクションが含まれる拡張プロパティ。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 2ace395b336a0950c814a4eb65103de440f59305
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966705"
---
# <a name="multivaluelegacyextendedproperty-resource-type"></a><span data-ttu-id="102eb-103">multiValueLegacyExtendedProperty リソースの種類</span><span class="sxs-lookup"><span data-stu-id="102eb-103">multiValueLegacyExtendedProperty resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="102eb-104">値のコレクションが含まれる拡張プロパティ。</span><span class="sxs-lookup"><span data-stu-id="102eb-104">An extended property that contains a collection of values.</span></span>

<span data-ttu-id="102eb-105">オープン拡張機能または拡張プロパティを使用するのに適した状況と、拡張プロパティを指定する方法の詳細については、「[拡張プロパティの概要](../resources/extended-properties-overview.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="102eb-105">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="methods"></a><span data-ttu-id="102eb-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="102eb-106">Methods</span></span>

| <span data-ttu-id="102eb-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="102eb-107">Method</span></span>           | <span data-ttu-id="102eb-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="102eb-108">Return Type</span></span>    |<span data-ttu-id="102eb-109">説明</span><span class="sxs-lookup"><span data-stu-id="102eb-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="102eb-110">Post</span><span class="sxs-lookup"><span data-stu-id="102eb-110">Post</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | <span data-ttu-id="102eb-111">サポートされているリソースインスタンス: [message](../resources/message.md)、 [mailfolder](../resources/mailfolder.md)、 [event](../resources/event.md)、 [calendar](../resources/calendar.md)、 [contact](../resources/contact.md)、 [contactfolder](../resources/contactfolder.md)、 [outlook の仕事](../resources/outlooktask.md)、または[outlook のタスクフォルダー](../resources/outlooktaskfolder.md)。</span><span class="sxs-lookup"><span data-stu-id="102eb-111">A supported resource instance: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [Outlook task](../resources/outlooktask.md), or [Outlook task folder](../resources/outlooktaskfolder.md).</span></span> <span data-ttu-id="102eb-112">グループ[投稿](../resources/post.md) はサポートされていませんので、ご注意ください。</span><span class="sxs-lookup"><span data-stu-id="102eb-112">Note that group [post](../resources/post.md) is not supported.</span></span> | <span data-ttu-id="102eb-113">サポートされているリソースの新しいインスタンスまたは既存のインスタンスに **multiValueLegacyExtendedProperty** を作成します。</span><span class="sxs-lookup"><span data-stu-id="102eb-113">Create a **multiValueLegacyExtendedProperty** in a new or existing instance of a supported resource.</span></span> |
|[<span data-ttu-id="102eb-114">Get</span><span class="sxs-lookup"><span data-stu-id="102eb-114">Get</span></span>](../api/multivaluelegacyextendedproperty-get.md) |<span data-ttu-id="102eb-115">サポートされているリソースインスタンス ([message](../resources/message.md)、 [mailfolder](../resources/mailfolder.md)、 [event](../resources/event.md)、 [calendar](../resources/calendar.md)、 [contact](../resources/contact.md)、 [contactfolder](../resources/contactfolder.md)、 [outlook タスク](../resources/outlooktask.md)、 [outlook タスクフォルダー](../resources/outlooktaskfolder.md)、またはグループの[投稿](../resources/post.md)) [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)オブジェクト。</span><span class="sxs-lookup"><span data-stu-id="102eb-115">A supported resource instance ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [Outlook task](../resources/outlooktask.md), [Outlook task folder](../resources/outlooktaskfolder.md), or group [post](../resources/post.md)) expanded with a [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) object.</span></span> |<span data-ttu-id="102eb-116">`$expand` を使用して拡張プロパティでリソース インスタンスを取得します。</span><span class="sxs-lookup"><span data-stu-id="102eb-116">Get a resource instance with an extended property using `$expand`.</span></span>|

## <a name="properties"></a><span data-ttu-id="102eb-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="102eb-117">Properties</span></span>
| <span data-ttu-id="102eb-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="102eb-118">Property</span></span>     | <span data-ttu-id="102eb-119">型</span><span class="sxs-lookup"><span data-stu-id="102eb-119">Type</span></span>   |<span data-ttu-id="102eb-120">説明</span><span class="sxs-lookup"><span data-stu-id="102eb-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="102eb-121">id</span><span class="sxs-lookup"><span data-stu-id="102eb-121">id</span></span>|<span data-ttu-id="102eb-122">string</span><span class="sxs-lookup"><span data-stu-id="102eb-122">string</span></span>|<span data-ttu-id="102eb-p102">プロパティ識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="102eb-p102">The property identifier. Read-only.</span></span>|
|<span data-ttu-id="102eb-125">value</span><span class="sxs-lookup"><span data-stu-id="102eb-125">value</span></span>|<span data-ttu-id="102eb-126">string collection</span><span class="sxs-lookup"><span data-stu-id="102eb-126">string collection</span></span>|<span data-ttu-id="102eb-127">プロパティ値のコレクション。</span><span class="sxs-lookup"><span data-stu-id="102eb-127">A collection of property values.</span></span>|

## <a name="relationships"></a><span data-ttu-id="102eb-128">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="102eb-128">Relationships</span></span>
<span data-ttu-id="102eb-129">なし</span><span class="sxs-lookup"><span data-stu-id="102eb-129">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="102eb-130">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="102eb-130">JSON representation</span></span>

<span data-ttu-id="102eb-131">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="102eb-131">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
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
<!--
{
  "type": "#page.annotation",
  "description": "multiValueLegacyExtendedProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
