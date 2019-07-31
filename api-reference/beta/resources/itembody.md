---
title: itemBody リソースの種類
description: メッセージ、イベント、またはグループの投稿など、アイテムの本文のプロパティを表します。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 0fa0360e3fe6c05e18446640900ca8840731219c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36010064"
---
# <a name="itembody-resource-type"></a><span data-ttu-id="7b846-103">itemBody リソースの種類</span><span class="sxs-lookup"><span data-stu-id="7b846-103">itemBody resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7b846-104">メッセージ、イベント、またはグループの投稿など、アイテムの本文のプロパティを表します。</span><span class="sxs-lookup"><span data-stu-id="7b846-104">Represents properties of the body of an item, such as a message, event or group post.</span></span>

## <a name="properties"></a><span data-ttu-id="7b846-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7b846-105">Properties</span></span>
| <span data-ttu-id="7b846-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7b846-106">Property</span></span>     | <span data-ttu-id="7b846-107">型</span><span class="sxs-lookup"><span data-stu-id="7b846-107">Type</span></span>   |<span data-ttu-id="7b846-108">説明</span><span class="sxs-lookup"><span data-stu-id="7b846-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7b846-109">content</span><span class="sxs-lookup"><span data-stu-id="7b846-109">content</span></span>|<span data-ttu-id="7b846-110">String</span><span class="sxs-lookup"><span data-stu-id="7b846-110">String</span></span>|<span data-ttu-id="7b846-111">アイテムのコンテンツ。</span><span class="sxs-lookup"><span data-stu-id="7b846-111">The content of the item.</span></span>|
|<span data-ttu-id="7b846-112">contentType</span><span class="sxs-lookup"><span data-stu-id="7b846-112">contentType</span></span>|<span data-ttu-id="7b846-113">String</span><span class="sxs-lookup"><span data-stu-id="7b846-113">String</span></span>|<span data-ttu-id="7b846-p101">コンテンツの種類。可能な値は、`text` と `HTML` です。</span><span class="sxs-lookup"><span data-stu-id="7b846-p101">The type of the content. Possible values are `text` and `HTML`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="7b846-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="7b846-116">JSON representation</span></span>

<span data-ttu-id="7b846-117">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="7b846-117">Here is a JSON representation of the resource</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "itemBody resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
