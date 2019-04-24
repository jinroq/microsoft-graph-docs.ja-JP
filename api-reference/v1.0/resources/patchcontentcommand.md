---
title: 実行時 contentcommand リソースの種類
description: PATCH 要求で OneNote ページに加えられた変更。
localization_priority: Normal
ms.openlocfilehash: fb0900490b3fe05e6fb90dc4ab8252620bf43983
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462544"
---
# <a name="patchcontentcommand-resource-type"></a><span data-ttu-id="ef4cf-103">実行時 contentcommand リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ef4cf-103">patchContentCommand resource type</span></span>

<span data-ttu-id="ef4cf-104">PATCH 要求で OneNote ページに加えられた変更。</span><span class="sxs-lookup"><span data-stu-id="ef4cf-104">The changes to make to a OneNote page in a PATCH request.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ef4cf-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ef4cf-105">JSON representation</span></span>

<span data-ttu-id="ef4cf-106">以下は、リソースの JSON 表記です。これは、 [PATCH pages/{id} '](../api/page-update.md)要求の本文で送信されます。</span><span class="sxs-lookup"><span data-stu-id="ef4cf-106">Here is a JSON representation of the resource, which is sent in the body of the [PATCH pages/{id}\`](../api/page-update.md) request.</span></span> 

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

## <a name="properties"></a><span data-ttu-id="ef4cf-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ef4cf-107">Properties</span></span>
| <span data-ttu-id="ef4cf-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ef4cf-108">Property</span></span>     | <span data-ttu-id="ef4cf-109">型</span><span class="sxs-lookup"><span data-stu-id="ef4cf-109">Type</span></span>   |<span data-ttu-id="ef4cf-110">説明</span><span class="sxs-lookup"><span data-stu-id="ef4cf-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ef4cf-111">action</span><span class="sxs-lookup"><span data-stu-id="ef4cf-111">action</span></span>|<span data-ttu-id="ef4cf-112">onenotePatchActionType</span><span class="sxs-lookup"><span data-stu-id="ef4cf-112">onenotePatchActionType</span></span>|<span data-ttu-id="ef4cf-113">ターゲット要素で実行するアクション。</span><span class="sxs-lookup"><span data-stu-id="ef4cf-113">The action to perform on the target element.</span></span> <span data-ttu-id="ef4cf-114">使用可能な値は`replace`、 `append` `delete`、、 `insert`、、 `prepend`またはです。</span><span class="sxs-lookup"><span data-stu-id="ef4cf-114">The possible values are: `replace`, `append`, `delete`, `insert`, or `prepend`.</span></span>|
|<span data-ttu-id="ef4cf-115">content</span><span class="sxs-lookup"><span data-stu-id="ef4cf-115">content</span></span>|<span data-ttu-id="ef4cf-116">String</span><span class="sxs-lookup"><span data-stu-id="ef4cf-116">String</span></span>|<span data-ttu-id="ef4cf-117">ページに追加する整形式 HTML の文字列と画像またはファイル バイナリ データ。</span><span class="sxs-lookup"><span data-stu-id="ef4cf-117">A string of well-formed HTML to add to the page, and any image or file binary data.</span></span> <span data-ttu-id="ef4cf-118">コンテンツにバイナリデータが含まれている場合は、 `multipart/form-data`コンテンツタイプを使用して要求を "Commands" パートで送信する必要があります。</span><span class="sxs-lookup"><span data-stu-id="ef4cf-118">If the content contains binary data, the request must be sent using the `multipart/form-data` content type with a "Commands" part.</span></span> |
|<span data-ttu-id="ef4cf-119">position</span><span class="sxs-lookup"><span data-stu-id="ef4cf-119">position</span></span>|<span data-ttu-id="ef4cf-120">onenotePatchInsertPosition</span><span class="sxs-lookup"><span data-stu-id="ef4cf-120">onenotePatchInsertPosition</span></span>|<span data-ttu-id="ef4cf-121">指定されたコンテンツを追加する位置を、ターゲット要素を基準にして指定します。</span><span class="sxs-lookup"><span data-stu-id="ef4cf-121">The location to add the supplied content, relative to the target element.</span></span> <span data-ttu-id="ef4cf-122">使用可能な値は`after` 、(既定) `before`またはです。</span><span class="sxs-lookup"><span data-stu-id="ef4cf-122">The possible values are: `after` (default) or `before`.</span></span>|
|<span data-ttu-id="ef4cf-123">target</span><span class="sxs-lookup"><span data-stu-id="ef4cf-123">target</span></span>|<span data-ttu-id="ef4cf-124">String</span><span class="sxs-lookup"><span data-stu-id="ef4cf-124">String</span></span>|<span data-ttu-id="ef4cf-125">更新する要素。</span><span class="sxs-lookup"><span data-stu-id="ef4cf-125">The element to update.</span></span> <span data-ttu-id="ef4cf-126">`#<data-id>`または、また`body`はのいずれ`title`か`<id>`のキーワードを指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="ef4cf-126">Must be the `#<data-id>` or the generated `<id>` of the element, or the `body` or `title` keyword.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "patchContentCommand resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
