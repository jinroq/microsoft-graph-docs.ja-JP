---
title: multiValueLegacyExtendedProperty リソースの種類
description: 値のコレクションが含まれる拡張プロパティ。
localization_priority: Normal
ms.openlocfilehash: 86ba1969e06dc549d1fca00148cbea96f94cf4b6
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29512949"
---
# <a name="multivaluelegacyextendedproperty-resource-type"></a><span data-ttu-id="a521d-103">multiValueLegacyExtendedProperty リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a521d-103">multiValueLegacyExtendedProperty resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a521d-104">値のコレクションが含まれる拡張プロパティ。</span><span class="sxs-lookup"><span data-stu-id="a521d-104">An extended property that contains a collection of values.</span></span>

<span data-ttu-id="a521d-105">オープン拡張機能または拡張プロパティを使用するのに適した状況と、拡張プロパティを指定する方法の詳細については、「[拡張プロパティの概要](../resources/extended-properties-overview.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a521d-105">See [Extended properties overview](../resources/extended-properties-overview.md) for more information about when to use open extensions or extended properties, and how to specify extended properties.</span></span>

## <a name="methods"></a><span data-ttu-id="a521d-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="a521d-106">Methods</span></span>

| <span data-ttu-id="a521d-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="a521d-107">Method</span></span>           | <span data-ttu-id="a521d-108">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="a521d-108">Return Type</span></span>    |<span data-ttu-id="a521d-109">説明</span><span class="sxs-lookup"><span data-stu-id="a521d-109">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a521d-110">Post</span><span class="sxs-lookup"><span data-stu-id="a521d-110">Post</span></span>](../api/multivaluelegacyextendedproperty-post-multivalueextendedproperties.md) | <span data-ttu-id="a521d-111">サポートされているリソース インスタンス:[メッセージ](../resources/message.md)、 [mailFolder](../resources/mailfolder.md)、[イベント](../resources/event.md)、[予定表](../resources/calendar.md)、[お問い合わせください](../resources/contact.md)、 [contactFolder](../resources/contactfolder.md)、 [Outlook のタスク](../resources/outlooktask.md)、または[Outlook の仕事フォルダー](../resources/outlooktaskfolder.md)。</span><span class="sxs-lookup"><span data-stu-id="a521d-111">A supported resource instance: [message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [Outlook task](../resources/outlooktask.md), or [Outlook task folder](../resources/outlooktaskfolder.md).</span></span> <span data-ttu-id="a521d-112">そのグループの[送信](../resources/post.md)はサポートされていません注意してください。</span><span class="sxs-lookup"><span data-stu-id="a521d-112">Note that group [post](../resources/post.md) is not supported.</span></span> | <span data-ttu-id="a521d-113">サポートされているリソースの新しいインスタンスまたは既存のインスタンスに multiValueLegacyExtendedProperty を作成します。</span><span class="sxs-lookup"><span data-stu-id="a521d-113">Create a **multiValueLegacyExtendedProperty** in a new or existing instance of a supported resource.</span></span> |
|[<span data-ttu-id="a521d-114">Get</span><span class="sxs-lookup"><span data-stu-id="a521d-114">Get</span></span>](../api/multivaluelegacyextendedproperty-get.md) |<span data-ttu-id="a521d-115">([メッセージ](../resources/message.md)、 [mailFolder](../resources/mailfolder.md)、[イベント](../resources/event.md)、[予定表](../resources/calendar.md)[にお問い合わせください](../resources/contact.md)、 [contactFolder](../resources/contactfolder.md) [Outlook の仕事](../resources/outlooktask.md)、 [Outlook の仕事フォルダー](../resources/outlooktaskfolder.md)、またはグループの[転記](../resources/post.md))、サポートされているリソースのインスタンスは、[と展開multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="a521d-115">A supported resource instance ([message](../resources/message.md), [mailFolder](../resources/mailfolder.md), [event](../resources/event.md), [calendar](../resources/calendar.md), [contact](../resources/contact.md), [contactFolder](../resources/contactfolder.md), [Outlook task](../resources/outlooktask.md), [Outlook task folder](../resources/outlooktaskfolder.md), or group [post](../resources/post.md)) expanded with a [multiValueLegacyExtendedProperty](multivaluelegacyextendedproperty.md) object.</span></span> |<span data-ttu-id="a521d-116">`$expand` を使用して拡張プロパティでリソース インスタンスを取得します。</span><span class="sxs-lookup"><span data-stu-id="a521d-116">Get a resource instance with an extended property using `$expand`.</span></span>|

## <a name="properties"></a><span data-ttu-id="a521d-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a521d-117">Properties</span></span>
| <span data-ttu-id="a521d-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a521d-118">Property</span></span>     | <span data-ttu-id="a521d-119">型</span><span class="sxs-lookup"><span data-stu-id="a521d-119">Type</span></span>   |<span data-ttu-id="a521d-120">説明</span><span class="sxs-lookup"><span data-stu-id="a521d-120">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a521d-121">id</span><span class="sxs-lookup"><span data-stu-id="a521d-121">id</span></span>|<span data-ttu-id="a521d-122">string</span><span class="sxs-lookup"><span data-stu-id="a521d-122">string</span></span>|<span data-ttu-id="a521d-p102">プロパティ識別子。読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="a521d-p102">The property identifier. Read-only.</span></span>|
|<span data-ttu-id="a521d-125">value</span><span class="sxs-lookup"><span data-stu-id="a521d-125">value</span></span>|<span data-ttu-id="a521d-126">string collection</span><span class="sxs-lookup"><span data-stu-id="a521d-126">string collection</span></span>|<span data-ttu-id="a521d-127">プロパティ値のコレクション。</span><span class="sxs-lookup"><span data-stu-id="a521d-127">A collection of property values.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a521d-128">関係</span><span class="sxs-lookup"><span data-stu-id="a521d-128">Relationships</span></span>
<span data-ttu-id="a521d-129">なし</span><span class="sxs-lookup"><span data-stu-id="a521d-129">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="a521d-130">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a521d-130">JSON representation</span></span>

<span data-ttu-id="a521d-131">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a521d-131">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "multiValueLegacyExtendedProperty resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/multivaluelegacyextendedproperty.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
