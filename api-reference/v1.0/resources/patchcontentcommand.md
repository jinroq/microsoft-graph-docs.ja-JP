---
title: patchContentCommand リソースの種類
description: PATCH 要求で OneNote ページに加える変更。
localization_priority: Normal
ms.openlocfilehash: fb0900490b3fe05e6fb90dc4ab8252620bf43983
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27804537"
---
# <a name="patchcontentcommand-resource-type"></a><span data-ttu-id="ac626-103">patchContentCommand リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ac626-103">patchContentCommand resource type</span></span>

<span data-ttu-id="ac626-104">PATCH 要求で OneNote ページに加える変更。</span><span class="sxs-lookup"><span data-stu-id="ac626-104">The changes to make to a OneNote page in a PATCH request.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ac626-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ac626-105">JSON representation</span></span>

<span data-ttu-id="ac626-106">以下は、リソースの JSON 表記です。[PATCH pages/{id}\`](../api/page-update.md) 要求の本文に送信されます。</span><span class="sxs-lookup"><span data-stu-id="ac626-106">Here is a JSON representation of the resource, which is sent in the body of the [PATCH pages/{id}\`](../api/page-update.md) request.</span></span> 

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

## <a name="properties"></a><span data-ttu-id="ac626-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ac626-107">Properties</span></span>
| <span data-ttu-id="ac626-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ac626-108">Property</span></span>     | <span data-ttu-id="ac626-109">種類</span><span class="sxs-lookup"><span data-stu-id="ac626-109">Type</span></span>   |<span data-ttu-id="ac626-110">説明</span><span class="sxs-lookup"><span data-stu-id="ac626-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ac626-111">action</span><span class="sxs-lookup"><span data-stu-id="ac626-111">action</span></span>|<span data-ttu-id="ac626-112">onenotePatchActionType</span><span class="sxs-lookup"><span data-stu-id="ac626-112">onenotePatchActionType</span></span>|<span data-ttu-id="ac626-113">ターゲット要素で実行するアクション。</span><span class="sxs-lookup"><span data-stu-id="ac626-113">The action to perform on the target element.</span></span> <span data-ttu-id="ac626-114">可能な値: `replace`、 `append`、 `delete`、 `insert`、または`prepend`。</span><span class="sxs-lookup"><span data-stu-id="ac626-114">The possible values are: `replace`, `append`, `delete`, `insert`, or `prepend`.</span></span>|
|<span data-ttu-id="ac626-115">content</span><span class="sxs-lookup"><span data-stu-id="ac626-115">content</span></span>|<span data-ttu-id="ac626-116">String</span><span class="sxs-lookup"><span data-stu-id="ac626-116">String</span></span>|<span data-ttu-id="ac626-p102">ページに追加する整形式 HTML の文字列と画像またはファイル バイナリ データ。コンテンツにバイナリ データが含まれている場合、コンテンツ タイプとして `multipart/form-data` を利用し、"Commands" パートを含む要求を送信する必要があります。</span><span class="sxs-lookup"><span data-stu-id="ac626-p102">A string of well-formed HTML to add to the page, and any image or file binary data. If the content contains binary data, the request must be sent using the `multipart/form-data` content type with a "Commands" part.</span></span> |
|<span data-ttu-id="ac626-119">position</span><span class="sxs-lookup"><span data-stu-id="ac626-119">position</span></span>|<span data-ttu-id="ac626-120">onenotePatchInsertPosition</span><span class="sxs-lookup"><span data-stu-id="ac626-120">onenotePatchInsertPosition</span></span>|<span data-ttu-id="ac626-121">指定されたコンテンツを追加する位置。ターゲット要素を基準とした相対位置です。</span><span class="sxs-lookup"><span data-stu-id="ac626-121">The location to add the supplied content, relative to the target element.</span></span> <span data-ttu-id="ac626-122">可能な値: `after` (既定値) または`before`。</span><span class="sxs-lookup"><span data-stu-id="ac626-122">The possible values are: `after` (default) or `before`.</span></span>|
|<span data-ttu-id="ac626-123">target</span><span class="sxs-lookup"><span data-stu-id="ac626-123">target</span></span>|<span data-ttu-id="ac626-124">String</span><span class="sxs-lookup"><span data-stu-id="ac626-124">String</span></span>|<span data-ttu-id="ac626-p104">更新する要素。要素の `#<data-id>` または生成された `<id>`、または `body` か `title` のキーワードでなければなりません。</span><span class="sxs-lookup"><span data-stu-id="ac626-p104">The element to update. Must be the `#<data-id>` or the generated `<id>` of the element, or the `body` or `title` keyword.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "patchContentCommand resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
