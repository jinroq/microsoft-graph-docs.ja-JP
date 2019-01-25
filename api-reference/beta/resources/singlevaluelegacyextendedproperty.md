---
title: singleValueLegacyExtendedProperty リソースの種類
description: '単一値が含まれる拡張プロパティ。 '
localization_priority: Normal
ms.openlocfilehash: 0d889756204853a525269f28cfdd3cc1b40be8a4
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512368"
---
# <a name="singlevaluelegacyextendedproperty-resource-type"></a><span data-ttu-id="fe19c-103">singleValueLegacyExtendedProperty リソースの種類</span><span class="sxs-lookup"><span data-stu-id="fe19c-103">singleValueLegacyExtendedProperty resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fe19c-104">単一値が含まれる拡張プロパティ。</span><span class="sxs-lookup"><span data-stu-id="fe19c-104">An extended property that contains a single value.</span></span> 

<span data-ttu-id="fe19c-105">オープン拡張機能または拡張プロパティを使用するのに適した状況と、拡張プロパティを指定する方法の詳細については、「[拡張プロパティの概要](../resources/extended-properties-overview.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fe19c-105">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span> 


## <a name="methods"></a><span data-ttu-id="fe19c-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="fe19c-106">Methods</span></span>

| <span data-ttu-id="fe19c-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="fe19c-107">Method</span></span>           | <span data-ttu-id="fe19c-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="fe19c-108">Return Type</span></span>    |<span data-ttu-id="fe19c-109">説明</span><span class="sxs-lookup"><span data-stu-id="fe19c-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="fe19c-110">Post</span><span class="sxs-lookup"><span data-stu-id="fe19c-110">Post</span></span>](../api/singlevaluelegacyextendedproperty-post-singlevalueextendedproperties.md) | <span data-ttu-id="fe19c-111">サポートされているリソース インスタンス:[メッセージ](../resources/message.md)、 [mailFolder](../resources/mailfolder.md)、[イベント](../resources/event.md)、[予定表](../resources/calendar.md)[にお問い合わせください](../resources/contact.md)、 [contactFolder](../resources/contactfolder.md)、 [Outlook の仕事](../resources/outlooktask.md)または[Outlook の仕事フォルダー](../resources/outlooktaskfolder.md)、ですが、グループに[投稿](../resources/post.md)がありません。</span><span class="sxs-lookup"><span data-stu-id="fe19c-111">A supported resource instance: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [Outlook task](../resources/outlooktask.md), or [Outlook task folder](../resources/outlooktaskfolder.md), but not group [post](../resources/post.md).</span></span> | <span data-ttu-id="fe19c-112">サポートされているリソースの新しいインスタンスまたは既存のインスタンスに **singleValueLegacyExtendedProperty** を作成します。</span><span class="sxs-lookup"><span data-stu-id="fe19c-112">Create a **singleValueLegacyExtendedProperty** in a new or existing instance of a supported resource.</span></span> |
|[<span data-ttu-id="fe19c-113">Get</span><span class="sxs-lookup"><span data-stu-id="fe19c-113">Get</span></span>](../api/singlevaluelegacyextendedproperty-get.md) |<span data-ttu-id="fe19c-114">([メッセージ](../resources/message.md)、 [mailFolder](../resources/mailfolder.md)、[イベント](../resources/event.md)、[予定表](../resources/calendar.md)[にお問い合わせください](../resources/contact.md)、 [contactFolder](../resources/contactfolder.md) [Outlook の仕事](../resources/outlooktask.md)、 [Outlook の仕事フォルダー](../resources/outlooktaskfolder.md)、またはグループの[転記](../resources/post.md))、サポートされているリソースのインスタンスのコレクションの 1 つまたはまたは、このような 1 つのインスタンスは、 [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md)オブジェクトを使用して展開します。</span><span class="sxs-lookup"><span data-stu-id="fe19c-114">One or a collection of supported resource instance ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [Outlook task](../resources/outlooktask.md), [Outlook task folder](../resources/outlooktaskfolder.md), or group [post](../resources/post.md)), or one such instance expanded with a [singleValueLegacyExtendedProperty](singlevaluelegacyextendedproperty.md) object.</span></span> |<span data-ttu-id="fe19c-115">`$expand` または `$filter` を使用して拡張プロパティでリソース インスタンスを取得します。</span><span class="sxs-lookup"><span data-stu-id="fe19c-115">Get a resource instance with an extended property using `$expand` or `$filter`.</span></span>|

## <a name="properties"></a><span data-ttu-id="fe19c-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fe19c-116">Properties</span></span>
| <span data-ttu-id="fe19c-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fe19c-117">Property</span></span>     | <span data-ttu-id="fe19c-118">型</span><span class="sxs-lookup"><span data-stu-id="fe19c-118">Type</span></span>   |<span data-ttu-id="fe19c-119">説明</span><span class="sxs-lookup"><span data-stu-id="fe19c-119">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fe19c-120">id</span><span class="sxs-lookup"><span data-stu-id="fe19c-120">id</span></span>|<span data-ttu-id="fe19c-121">string</span><span class="sxs-lookup"><span data-stu-id="fe19c-121">string</span></span>|<span data-ttu-id="fe19c-p101">プロパティ識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="fe19c-p101">The property identifier. Read-only.</span></span>|
|<span data-ttu-id="fe19c-124">value</span><span class="sxs-lookup"><span data-stu-id="fe19c-124">value</span></span>|<span data-ttu-id="fe19c-125">string</span><span class="sxs-lookup"><span data-stu-id="fe19c-125">string</span></span>|<span data-ttu-id="fe19c-126">プロパティ値。</span><span class="sxs-lookup"><span data-stu-id="fe19c-126">A property value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="fe19c-127">関係</span><span class="sxs-lookup"><span data-stu-id="fe19c-127">Relationships</span></span>
<span data-ttu-id="fe19c-128">なし</span><span class="sxs-lookup"><span data-stu-id="fe19c-128">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="fe19c-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fe19c-129">JSON representation</span></span>

<span data-ttu-id="fe19c-130">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="fe19c-130">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/singlevaluelegacyextendedproperty.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
