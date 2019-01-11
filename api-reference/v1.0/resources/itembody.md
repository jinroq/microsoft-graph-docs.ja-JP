---
title: itemBody リソースの種類
description: メッセージ、イベント、またはグループの投稿など、アイテムの本文のプロパティを表します。
localization_priority: Normal
ms.openlocfilehash: 2eaf3b5e13833665c452eeecd74169915f5ac2fd
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27805230"
---
# <a name="itembody-resource-type"></a><span data-ttu-id="a6e32-103">itemBody リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a6e32-103">itemBody resource type</span></span>

<span data-ttu-id="a6e32-104">メッセージ、イベント、またはグループの投稿など、アイテムの本文のプロパティを表します。</span><span class="sxs-lookup"><span data-stu-id="a6e32-104">Represents properties of the body of an item, such as a message, event or group post.</span></span>

## <a name="properties"></a><span data-ttu-id="a6e32-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a6e32-105">Properties</span></span>
| <span data-ttu-id="a6e32-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a6e32-106">Property</span></span>     | <span data-ttu-id="a6e32-107">種類</span><span class="sxs-lookup"><span data-stu-id="a6e32-107">Type</span></span>   |<span data-ttu-id="a6e32-108">説明</span><span class="sxs-lookup"><span data-stu-id="a6e32-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a6e32-109">content</span><span class="sxs-lookup"><span data-stu-id="a6e32-109">content</span></span>|<span data-ttu-id="a6e32-110">String</span><span class="sxs-lookup"><span data-stu-id="a6e32-110">String</span></span>|<span data-ttu-id="a6e32-111">アイテムのコンテンツ。</span><span class="sxs-lookup"><span data-stu-id="a6e32-111">The content of the item.</span></span>|
|<span data-ttu-id="a6e32-112">contentType</span><span class="sxs-lookup"><span data-stu-id="a6e32-112">contentType</span></span>|<span data-ttu-id="a6e32-113">bodyType</span><span class="sxs-lookup"><span data-stu-id="a6e32-113">bodyType</span></span>|<span data-ttu-id="a6e32-p101">コンテンツの種類。可能な値は、`Text` と `HTML` です。</span><span class="sxs-lookup"><span data-stu-id="a6e32-p101">The type of the content. Possible values are `Text` and `HTML`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a6e32-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a6e32-116">JSON representation</span></span>

<span data-ttu-id="a6e32-117">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="a6e32-117">Here is a JSON representation of the resource</span></span>

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
