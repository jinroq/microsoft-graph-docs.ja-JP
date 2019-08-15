---
title: 実行時 Contentcommand リソースの種類
description: PATCH 要求で OneNote ページに加えられた変更。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 4cfa6fe84c18d4895e5d709d3ab6254258c1b970
ms.sourcegitcommit: 1066aa4045d48f9c9b764d3b2891cf4f806d17d5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/15/2019
ms.locfileid: "36422283"
---
# <a name="patchcontentcommand-resource-type"></a><span data-ttu-id="0da16-103">実行時 Contentcommand リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0da16-103">patchContentCommand resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0da16-104">PATCH 要求で OneNote ページに加えられた変更。</span><span class="sxs-lookup"><span data-stu-id="0da16-104">The changes to make to a OneNote page in a PATCH request.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0da16-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0da16-105">JSON representation</span></span>

<span data-ttu-id="0da16-106">以下は、リソースの JSON 表記です。これは、 [PATCH pages/{id} '](../api/page-update.md)要求の本文で送信されます。</span><span class="sxs-lookup"><span data-stu-id="0da16-106">Here is a JSON representation of the resource, which is sent in the body of the [PATCH pages/{id}\`](../api/page-update.md) request.</span></span> 

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenotePatchContentCommand"
}-->

```json
{
  "action": "String",
  "content": "string",
  "position": "String",
  "target": "string"
}

```

## <a name="properties"></a><span data-ttu-id="0da16-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0da16-107">Properties</span></span>
| <span data-ttu-id="0da16-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0da16-108">Property</span></span>     | <span data-ttu-id="0da16-109">型</span><span class="sxs-lookup"><span data-stu-id="0da16-109">Type</span></span>   |<span data-ttu-id="0da16-110">説明</span><span class="sxs-lookup"><span data-stu-id="0da16-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0da16-111">action</span><span class="sxs-lookup"><span data-stu-id="0da16-111">action</span></span>|<span data-ttu-id="0da16-112">String</span><span class="sxs-lookup"><span data-stu-id="0da16-112">String</span></span>|<span data-ttu-id="0da16-113">ターゲット要素で実行するアクション。</span><span class="sxs-lookup"><span data-stu-id="0da16-113">The action to perform on the target element.</span></span> <span data-ttu-id="0da16-114">可能な値は、`replace`、`append`、`delete`、`insert`、`prepend` です。</span><span class="sxs-lookup"><span data-stu-id="0da16-114">Possible values are: `replace`, `append`, `delete`, `insert`, or `prepend`.</span></span>|
|<span data-ttu-id="0da16-115">content</span><span class="sxs-lookup"><span data-stu-id="0da16-115">content</span></span>|<span data-ttu-id="0da16-116">String</span><span class="sxs-lookup"><span data-stu-id="0da16-116">String</span></span>|<span data-ttu-id="0da16-117">ページに追加する整形式 HTML の文字列と画像またはファイル バイナリ データ。</span><span class="sxs-lookup"><span data-stu-id="0da16-117">A string of well-formed HTML to add to the page, and any image or file binary data.</span></span> <span data-ttu-id="0da16-118">コンテンツにバイナリデータが含まれている場合は、 `multipart/form-data`コンテンツタイプを使用して要求を "Commands" パートで送信する必要があります。</span><span class="sxs-lookup"><span data-stu-id="0da16-118">If the content contains binary data, the request must be sent using the `multipart/form-data` content type with a "Commands" part.</span></span> |
|<span data-ttu-id="0da16-119">position</span><span class="sxs-lookup"><span data-stu-id="0da16-119">position</span></span>|<span data-ttu-id="0da16-120">String</span><span class="sxs-lookup"><span data-stu-id="0da16-120">String</span></span>|<span data-ttu-id="0da16-121">指定されたコンテンツを追加する位置を、ターゲット要素を基準にして指定します。</span><span class="sxs-lookup"><span data-stu-id="0da16-121">The location to add the supplied content, relative to the target element.</span></span> <span data-ttu-id="0da16-122">可能な値は`after`次のとおりです`before`。 (既定値) または。</span><span class="sxs-lookup"><span data-stu-id="0da16-122">Possible values are: `after` (default) or `before`.</span></span>|
|<span data-ttu-id="0da16-123">target</span><span class="sxs-lookup"><span data-stu-id="0da16-123">target</span></span>|<span data-ttu-id="0da16-124">String</span><span class="sxs-lookup"><span data-stu-id="0da16-124">String</span></span>|<span data-ttu-id="0da16-125">更新する要素。</span><span class="sxs-lookup"><span data-stu-id="0da16-125">The element to update.</span></span> <span data-ttu-id="0da16-126">`#<data-id>`または、また`body`はのいずれ`title`か`{id}`のキーワードを指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="0da16-126">Must be the `#<data-id>` or the generated `{id}` of the element, or the `body` or `title` keyword.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "patchContentCommand resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
