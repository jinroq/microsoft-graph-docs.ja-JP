---
title: patchContentCommand リソースの種類
description: PATCH 要求で OneNote ページに加える変更。
ms.openlocfilehash: fb559a96aa5eef94dd07280b888da0df989b2363
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073273"
---
# <a name="patchcontentcommand-resource-type"></a><span data-ttu-id="90cc7-103">patchContentCommand リソースの種類</span><span class="sxs-lookup"><span data-stu-id="90cc7-103">patchContentCommand resource type</span></span>

> <span data-ttu-id="90cc7-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="90cc7-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="90cc7-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="90cc7-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="90cc7-106">PATCH 要求で OneNote ページに加える変更。</span><span class="sxs-lookup"><span data-stu-id="90cc7-106">The changes to make to a OneNote page in a PATCH request.</span></span>

## <a name="json-representation"></a><span data-ttu-id="90cc7-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="90cc7-107">JSON representation</span></span>

<span data-ttu-id="90cc7-108">以下は、リソースの JSON 表記です。[PATCH pages/{id}\`](../api/page-update.md) 要求の本文に送信されます。</span><span class="sxs-lookup"><span data-stu-id="90cc7-108">Here is a JSON representation of the resource, which is sent in the body of the [PATCH pages/{id}\`](../api/page-update.md) request.</span></span> 

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

## <a name="properties"></a><span data-ttu-id="90cc7-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="90cc7-109">Properties</span></span>
| <span data-ttu-id="90cc7-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="90cc7-110">Property</span></span>     | <span data-ttu-id="90cc7-111">型</span><span class="sxs-lookup"><span data-stu-id="90cc7-111">Type</span></span>   |<span data-ttu-id="90cc7-112">説明</span><span class="sxs-lookup"><span data-stu-id="90cc7-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="90cc7-113">action</span><span class="sxs-lookup"><span data-stu-id="90cc7-113">action</span></span>|<span data-ttu-id="90cc7-114">String</span><span class="sxs-lookup"><span data-stu-id="90cc7-114">String</span></span>|<span data-ttu-id="90cc7-p102">ターゲット要素で実行するアクション。使用可能な値: `replace`、`append`、`delete`、`insert`、`prepend`。</span><span class="sxs-lookup"><span data-stu-id="90cc7-p102">The action to perform on the target element. Possible values are: `replace`, `append`, `delete`, `insert`, or `prepend`.</span></span>|
|<span data-ttu-id="90cc7-117">content</span><span class="sxs-lookup"><span data-stu-id="90cc7-117">content</span></span>|<span data-ttu-id="90cc7-118">String</span><span class="sxs-lookup"><span data-stu-id="90cc7-118">String</span></span>|<span data-ttu-id="90cc7-p103">ページに追加する整形式 HTML の文字列と画像またはファイル バイナリ データ。コンテンツにバイナリ データが含まれている場合、コンテンツ タイプとして `multipart/form-data` を利用し、"Commands" パートを含む要求を送信する必要があります。</span><span class="sxs-lookup"><span data-stu-id="90cc7-p103">A string of well-formed HTML to add to the page, and any image or file binary data. If the content contains binary data, the request must be sent using the `multipart/form-data` content type with a "Commands" part.</span></span> |
|<span data-ttu-id="90cc7-121">position</span><span class="sxs-lookup"><span data-stu-id="90cc7-121">position</span></span>|<span data-ttu-id="90cc7-122">String</span><span class="sxs-lookup"><span data-stu-id="90cc7-122">String</span></span>|<span data-ttu-id="90cc7-p104">指定されたコンテンツを追加する位置。ターゲット要素を基準とした相対位置です。使用可能な値: `after` (既定値) または `before`。</span><span class="sxs-lookup"><span data-stu-id="90cc7-p104">The location to add the supplied content, relative to the target element. Possible values are: `after` (default) or `before`.</span></span>|
|<span data-ttu-id="90cc7-125">target</span><span class="sxs-lookup"><span data-stu-id="90cc7-125">target</span></span>|<span data-ttu-id="90cc7-126">String</span><span class="sxs-lookup"><span data-stu-id="90cc7-126">String</span></span>|<span data-ttu-id="90cc7-p105">更新する要素。要素の `#<data-id>` または生成された `<id>`、または `body` か `title` のキーワードでなければなりません。</span><span class="sxs-lookup"><span data-stu-id="90cc7-p105">The element to update. Must be the `#<data-id>` or the generated `<id>` of the element, or the `body` or `title` keyword.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "patchContentCommand resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->