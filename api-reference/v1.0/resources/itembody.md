---
title: itemBody リソースの種類
description: メッセージ、イベント、またはグループの投稿など、アイテムの本文のプロパティを表します。
localization_priority: Normal
ms.openlocfilehash: df2e7e8cea9e1b2e6a6d1011029a1898e2794f45
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29642563"
---
# <a name="itembody-resource-type"></a><span data-ttu-id="4564b-103">itemBody リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4564b-103">itemBody resource type</span></span>

<span data-ttu-id="4564b-104">メッセージ、イベント、またはグループの投稿など、アイテムの本文のプロパティを表します。</span><span class="sxs-lookup"><span data-stu-id="4564b-104">Represents properties of the body of an item, such as a message, event or group post.</span></span>

## <a name="properties"></a><span data-ttu-id="4564b-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4564b-105">Properties</span></span>
| <span data-ttu-id="4564b-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4564b-106">Property</span></span>     | <span data-ttu-id="4564b-107">型</span><span class="sxs-lookup"><span data-stu-id="4564b-107">Type</span></span>   |<span data-ttu-id="4564b-108">説明</span><span class="sxs-lookup"><span data-stu-id="4564b-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4564b-109">content</span><span class="sxs-lookup"><span data-stu-id="4564b-109">content</span></span>|<span data-ttu-id="4564b-110">String</span><span class="sxs-lookup"><span data-stu-id="4564b-110">String</span></span>|<span data-ttu-id="4564b-111">アイテムのコンテンツ。</span><span class="sxs-lookup"><span data-stu-id="4564b-111">The content of the item.</span></span>|
|<span data-ttu-id="4564b-112">contentType</span><span class="sxs-lookup"><span data-stu-id="4564b-112">contentType</span></span>|<span data-ttu-id="4564b-113">bodyType</span><span class="sxs-lookup"><span data-stu-id="4564b-113">bodyType</span></span>|<span data-ttu-id="4564b-p101">コンテンツの種類。可能な値は、`text` と `HTML` です。</span><span class="sxs-lookup"><span data-stu-id="4564b-p101">The type of the content. Possible values are `text` and `HTML`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4564b-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4564b-116">JSON representation</span></span>

<span data-ttu-id="4564b-117">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="4564b-117">Here is a JSON representation of the resource</span></span>

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
