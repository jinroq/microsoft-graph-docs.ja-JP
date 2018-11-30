---
title: itemBody リソースの種類
description: メッセージ、イベント、またはグループの投稿など、アイテムの本文のプロパティを表します。
ms.openlocfilehash: ebcc2797052ac3a5a73547332e37c5e9c1bd3a41
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022858"
---
# <a name="itembody-resource-type"></a><span data-ttu-id="f5400-103">itemBody リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f5400-103">itemBody resource type</span></span>

<span data-ttu-id="f5400-104">メッセージ、イベント、またはグループの投稿など、アイテムの本文のプロパティを表します。</span><span class="sxs-lookup"><span data-stu-id="f5400-104">Represents properties of the body of an item, such as a message, event or group post.</span></span>

## <a name="properties"></a><span data-ttu-id="f5400-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f5400-105">Properties</span></span>
| <span data-ttu-id="f5400-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f5400-106">Property</span></span>     | <span data-ttu-id="f5400-107">型</span><span class="sxs-lookup"><span data-stu-id="f5400-107">Type</span></span>   |<span data-ttu-id="f5400-108">説明</span><span class="sxs-lookup"><span data-stu-id="f5400-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f5400-109">content</span><span class="sxs-lookup"><span data-stu-id="f5400-109">content</span></span>|<span data-ttu-id="f5400-110">String</span><span class="sxs-lookup"><span data-stu-id="f5400-110">String</span></span>|<span data-ttu-id="f5400-111">アイテムのコンテンツ。</span><span class="sxs-lookup"><span data-stu-id="f5400-111">The content of the item.</span></span>|
|<span data-ttu-id="f5400-112">contentType</span><span class="sxs-lookup"><span data-stu-id="f5400-112">contentType</span></span>|<span data-ttu-id="f5400-113">bodyType</span><span class="sxs-lookup"><span data-stu-id="f5400-113">bodyType</span></span>|<span data-ttu-id="f5400-p101">コンテンツの種類。可能な値は、`Text` と `HTML` です。</span><span class="sxs-lookup"><span data-stu-id="f5400-p101">The type of the content. Possible values are `Text` and `HTML`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f5400-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f5400-116">JSON representation</span></span>

<span data-ttu-id="f5400-117">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="f5400-117">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.itemBody"
}-->

```json
{
  "content": "string",
  "contentType": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "itemBody resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
