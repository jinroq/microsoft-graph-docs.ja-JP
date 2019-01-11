---
title: itemBody リソースの種類
description: メッセージ、イベント、またはグループの投稿など、アイテムの本文のプロパティを表します。
localization_priority: Normal
ms.openlocfilehash: 791906c8442250d05d1b94b9eb9b19320f45e9c9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27872143"
---
# <a name="itembody-resource-type"></a><span data-ttu-id="6c3db-103">itemBody リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6c3db-103">itemBody resource type</span></span>

> <span data-ttu-id="6c3db-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6c3db-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6c3db-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6c3db-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6c3db-106">メッセージ、イベント、またはグループの投稿など、アイテムの本文のプロパティを表します。</span><span class="sxs-lookup"><span data-stu-id="6c3db-106">Represents properties of the body of an item, such as a message, event or group post.</span></span>

## <a name="properties"></a><span data-ttu-id="6c3db-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6c3db-107">Properties</span></span>
| <span data-ttu-id="6c3db-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6c3db-108">Property</span></span>     | <span data-ttu-id="6c3db-109">種類</span><span class="sxs-lookup"><span data-stu-id="6c3db-109">Type</span></span>   |<span data-ttu-id="6c3db-110">説明</span><span class="sxs-lookup"><span data-stu-id="6c3db-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6c3db-111">content</span><span class="sxs-lookup"><span data-stu-id="6c3db-111">content</span></span>|<span data-ttu-id="6c3db-112">String</span><span class="sxs-lookup"><span data-stu-id="6c3db-112">String</span></span>|<span data-ttu-id="6c3db-113">アイテムのコンテンツ。</span><span class="sxs-lookup"><span data-stu-id="6c3db-113">The content of the item.</span></span>|
|<span data-ttu-id="6c3db-114">contentType</span><span class="sxs-lookup"><span data-stu-id="6c3db-114">contentType</span></span>|<span data-ttu-id="6c3db-115">String</span><span class="sxs-lookup"><span data-stu-id="6c3db-115">String</span></span>|<span data-ttu-id="6c3db-p102">コンテンツの種類。可能な値は、`Text` と `HTML` です。</span><span class="sxs-lookup"><span data-stu-id="6c3db-p102">The type of the content. Possible values are `Text` and `HTML`.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6c3db-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6c3db-118">JSON representation</span></span>

<span data-ttu-id="6c3db-119">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="6c3db-119">Here is a JSON representation of the resource</span></span>

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
