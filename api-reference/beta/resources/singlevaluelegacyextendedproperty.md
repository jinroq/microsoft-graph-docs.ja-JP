---
title: singleValueLegacyExtendedProperty リソースの種類
description: '単一値が含まれる拡張プロパティ。 '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 256fea5b42f367fb9c6d08b2e871bebd825e3451
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008328"
---
# <a name="singlevaluelegacyextendedproperty-resource-type"></a><span data-ttu-id="102c6-103">singleValueLegacyExtendedProperty リソースの種類</span><span class="sxs-lookup"><span data-stu-id="102c6-103">singleValueLegacyExtendedProperty resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="102c6-104">単一値が含まれる拡張プロパティ。</span><span class="sxs-lookup"><span data-stu-id="102c6-104">An extended property that contains a single value.</span></span> 

<span data-ttu-id="102c6-105">オープン拡張機能または拡張プロパティを使用するのに適した状況と、拡張プロパティを指定する方法の詳細については、「[拡張プロパティの概要](../resources/extended-properties-overview.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="102c6-105">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span> 


## <a name="methods"></a><span data-ttu-id="102c6-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="102c6-106">Methods</span></span>

| <span data-ttu-id="102c6-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="102c6-107">Method</span></span>           | <span data-ttu-id="102c6-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="102c6-108">Return Type</span></span>    |<span data-ttu-id="102c6-109">説明</span><span class="sxs-lookup"><span data-stu-id="102c6-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="102c6-110">Post</span><span class="sxs-lookup"><span data-stu-id="102c6-110">Post</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) | <span data-ttu-id="102c6-111">サポートされているリソースインスタンス: [message](../resources/message.md)、 [mailfolder](../resources/mailfolder.md)、 [event](../resources/event.md)、 [calendar](../resources/calendar.md)、 [contact](../resources/contact.md)、 [contactfolder](../resources/contactfolder.md)、 [outlook の仕事](../resources/outlooktask.md)、または[outlook のタスクフォルダー](../resources/outlooktaskfolder.md)。ただし、グループの[投稿](../resources/post.md)は含まれません。</span><span class="sxs-lookup"><span data-stu-id="102c6-111">A supported resource instance: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [Outlook task](../resources/outlooktask.md), or [Outlook task folder](../resources/outlooktaskfolder.md), but not group [post](../resources/post.md).</span></span> | <span data-ttu-id="102c6-112">サポートされているリソースの新しいインスタンスまたは既存のインスタンスに **singleValueLegacyExtendedProperty** を作成します。</span><span class="sxs-lookup"><span data-stu-id="102c6-112">Create a **singleValueLegacyExtendedProperty** in a new or existing instance of a supported resource.</span></span> |
|[<span data-ttu-id="102c6-113">Get</span><span class="sxs-lookup"><span data-stu-id="102c6-113">Get</span></span>](../api/singlevaluelegacyextendedproperty-get.md) |<span data-ttu-id="102c6-114">サポートされているリソースインスタンス ([message](../resources/message.md)、 [mailfolder](../resources/mailfolder.md)、 [event](../resources/event.md)、 [calendar](../resources/calendar.md)、 [contact](../resources/contact.md)、 [contactfolder](../resources/contactfolder.md)、 [outlook タスク](../resources/outlooktask.md)、 [outlook タスクフォルダー](../resources/outlooktaskfolder.md)、またはグループ[投稿](../resources/post.md)) の1つまたは複数のコレクション。または、 [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)オブジェクトを使用して展開されたインスタンスが1つあります。</span><span class="sxs-lookup"><span data-stu-id="102c6-114">One or a collection of supported resource instance ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [Outlook task](../resources/outlooktask.md), [Outlook task folder](../resources/outlooktaskfolder.md), or group [post](../resources/post.md)), or one such instance expanded with a [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) object.</span></span> |<span data-ttu-id="102c6-115">`$expand` または `$filter` を使用して拡張プロパティでリソース インスタンスを取得します。</span><span class="sxs-lookup"><span data-stu-id="102c6-115">Get a resource instance with an extended property using `$expand` or `$filter`.</span></span>|

## <a name="properties"></a><span data-ttu-id="102c6-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="102c6-116">Properties</span></span>
| <span data-ttu-id="102c6-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="102c6-117">Property</span></span>     | <span data-ttu-id="102c6-118">型</span><span class="sxs-lookup"><span data-stu-id="102c6-118">Type</span></span>   |<span data-ttu-id="102c6-119">説明</span><span class="sxs-lookup"><span data-stu-id="102c6-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="102c6-120">id</span><span class="sxs-lookup"><span data-stu-id="102c6-120">id</span></span>|<span data-ttu-id="102c6-121">string</span><span class="sxs-lookup"><span data-stu-id="102c6-121">string</span></span>|<span data-ttu-id="102c6-p101">プロパティ識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="102c6-p101">The property identifier. Read-only.</span></span>|
|<span data-ttu-id="102c6-124">value</span><span class="sxs-lookup"><span data-stu-id="102c6-124">value</span></span>|<span data-ttu-id="102c6-125">string</span><span class="sxs-lookup"><span data-stu-id="102c6-125">string</span></span>|<span data-ttu-id="102c6-126">プロパティ値。</span><span class="sxs-lookup"><span data-stu-id="102c6-126">A property value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="102c6-127">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="102c6-127">Relationships</span></span>
<span data-ttu-id="102c6-128">なし</span><span class="sxs-lookup"><span data-stu-id="102c6-128">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="102c6-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="102c6-129">JSON representation</span></span>

<span data-ttu-id="102c6-130">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="102c6-130">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "singleValueLegacyExtendedProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
