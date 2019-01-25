---
title: patchContentCommand リソースの種類
description: PATCH 要求で OneNote ページに加える変更。
localization_priority: Normal
ms.openlocfilehash: d0d8f320d22a8b3466ddd53deee5bcb7955ff3d1
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523884"
---
# <a name="patchcontentcommand-resource-type"></a><span data-ttu-id="9180f-103">patchContentCommand リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9180f-103">patchContentCommand resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9180f-104">PATCH 要求で OneNote ページに加える変更。</span><span class="sxs-lookup"><span data-stu-id="9180f-104">The changes to make to a OneNote page in a PATCH request.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9180f-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9180f-105">JSON representation</span></span>

<span data-ttu-id="9180f-106">以下は、リソースの JSON 表記です。[PATCH pages/{id}\`](../api/page-update.md) 要求の本文に送信されます。</span><span class="sxs-lookup"><span data-stu-id="9180f-106">Here is a JSON representation of the resource, which is sent in the body of the [PATCH pages/{id}\`](../api/page-update.md) request.</span></span> 

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

## <a name="properties"></a><span data-ttu-id="9180f-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9180f-107">Properties</span></span>
| <span data-ttu-id="9180f-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9180f-108">Property</span></span>     | <span data-ttu-id="9180f-109">型</span><span class="sxs-lookup"><span data-stu-id="9180f-109">Type</span></span>   |<span data-ttu-id="9180f-110">説明</span><span class="sxs-lookup"><span data-stu-id="9180f-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9180f-111">action</span><span class="sxs-lookup"><span data-stu-id="9180f-111">action</span></span>|<span data-ttu-id="9180f-112">String</span><span class="sxs-lookup"><span data-stu-id="9180f-112">String</span></span>|<span data-ttu-id="9180f-p101">ターゲット要素で実行するアクション。使用可能な値: `replace`、`append`、`delete`、`insert`、`prepend`。</span><span class="sxs-lookup"><span data-stu-id="9180f-p101">The action to perform on the target element. Possible values are: `replace`, `append`, `delete`, `insert`, or `prepend`.</span></span>|
|<span data-ttu-id="9180f-115">content</span><span class="sxs-lookup"><span data-stu-id="9180f-115">content</span></span>|<span data-ttu-id="9180f-116">String</span><span class="sxs-lookup"><span data-stu-id="9180f-116">String</span></span>|<span data-ttu-id="9180f-p102">ページに追加する整形式 HTML の文字列と画像またはファイル バイナリ データ。コンテンツにバイナリ データが含まれている場合、コンテンツ タイプとして `multipart/form-data` を利用し、"Commands" パートを含む要求を送信する必要があります。</span><span class="sxs-lookup"><span data-stu-id="9180f-p102">A string of well-formed HTML to add to the page, and any image or file binary data. If the content contains binary data, the request must be sent using the `multipart/form-data` content type with a "Commands" part.</span></span> |
|<span data-ttu-id="9180f-119">position</span><span class="sxs-lookup"><span data-stu-id="9180f-119">position</span></span>|<span data-ttu-id="9180f-120">String</span><span class="sxs-lookup"><span data-stu-id="9180f-120">String</span></span>|<span data-ttu-id="9180f-p103">指定されたコンテンツを追加する位置。ターゲット要素を基準とした相対位置です。使用可能な値: `after` (既定値) または `before`。</span><span class="sxs-lookup"><span data-stu-id="9180f-p103">The location to add the supplied content, relative to the target element. Possible values are: `after` (default) or `before`.</span></span>|
|<span data-ttu-id="9180f-123">target</span><span class="sxs-lookup"><span data-stu-id="9180f-123">target</span></span>|<span data-ttu-id="9180f-124">String</span><span class="sxs-lookup"><span data-stu-id="9180f-124">String</span></span>|<span data-ttu-id="9180f-p104">更新する要素。要素の `#<data-id>` または生成された `<id>`、または `body` か `title` のキーワードでなければなりません。</span><span class="sxs-lookup"><span data-stu-id="9180f-p104">The element to update. Must be the `#<data-id>` or the generated `<id>` of the element, or the `body` or `title` keyword.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "patchContentCommand resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/patchcontentcommand.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
