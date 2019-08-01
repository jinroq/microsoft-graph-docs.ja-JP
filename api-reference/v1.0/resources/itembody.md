---
title: itemBody リソースの種類
description: メッセージ、イベント、またはグループの投稿など、アイテムの本文のプロパティを表します。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 406a753ef8b58ba5ff19f7669239c3d9abb860c5
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036555"
---
# <a name="itembody-resource-type"></a><span data-ttu-id="0da96-103">itemBody リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0da96-103">itemBody resource type</span></span>

<span data-ttu-id="0da96-104">メッセージ、イベント、またはグループの投稿など、アイテムの本文のプロパティを表します。</span><span class="sxs-lookup"><span data-stu-id="0da96-104">Represents properties of the body of an item, such as a message, event or group post.</span></span>

## <a name="properties"></a><span data-ttu-id="0da96-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0da96-105">Properties</span></span>
| <span data-ttu-id="0da96-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0da96-106">Property</span></span>     | <span data-ttu-id="0da96-107">型</span><span class="sxs-lookup"><span data-stu-id="0da96-107">Type</span></span>   |<span data-ttu-id="0da96-108">説明</span><span class="sxs-lookup"><span data-stu-id="0da96-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0da96-109">content</span><span class="sxs-lookup"><span data-stu-id="0da96-109">content</span></span>|<span data-ttu-id="0da96-110">String</span><span class="sxs-lookup"><span data-stu-id="0da96-110">String</span></span>|<span data-ttu-id="0da96-111">アイテムのコンテンツ。</span><span class="sxs-lookup"><span data-stu-id="0da96-111">The content of the item.</span></span>|
|<span data-ttu-id="0da96-112">contentType</span><span class="sxs-lookup"><span data-stu-id="0da96-112">contentType</span></span>|<span data-ttu-id="0da96-113">bodyType</span><span class="sxs-lookup"><span data-stu-id="0da96-113">bodyType</span></span>|<span data-ttu-id="0da96-114">コンテンツの種類。</span><span class="sxs-lookup"><span data-stu-id="0da96-114">The type of the content.</span></span> <span data-ttu-id="0da96-115">可能な値は、`text` と `HTML` です。</span><span class="sxs-lookup"><span data-stu-id="0da96-115">Possible values are `text` and `HTML`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="0da96-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0da96-116">JSON representation</span></span>

<span data-ttu-id="0da96-117">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="0da96-117">Here is a JSON representation of the resource</span></span>

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
