---
title: resource リソースの種類
description: 'イメージまたは OneNote のページ上の他のファイル リソースです。 '
ms.openlocfilehash: 8e0e049cab613c7c1a72c8c96e21bac77c507ae1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27072224"
---
# <a name="resource-resource-type"></a><span data-ttu-id="97e76-103">resource リソースの種類</span><span class="sxs-lookup"><span data-stu-id="97e76-103">resource resource type</span></span>

> <span data-ttu-id="97e76-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="97e76-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="97e76-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="97e76-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="97e76-106">イメージまたは OneNote のページ上の他のファイル リソースです。</span><span class="sxs-lookup"><span data-stu-id="97e76-106">An image or other file resource on a OneNote page.</span></span> 

<span data-ttu-id="97e76-107">リソースのバイナリ データは取得できますが、リソース オブジェクトまたはリソース コレクションの JSON 表記の取得はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="97e76-107">You can get the binary data of a resource, but getting a JSON representation of a resource object or a resource collection is not supported.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenoteResource"
}-->

<span data-ttu-id="97e76-108">GET リクエストをリソースの `content` エンドポイントに送信することによって、特定のリソースのバイナリ データを取得します。</span><span class="sxs-lookup"><span data-stu-id="97e76-108">Get the binary data of a specific resource by sending a GET request to the resource's `content` endpoint:</span></span>

```
GET ../onenote/resources/{id}/content
```

<span data-ttu-id="97e76-109">ファイルのリソース URI は、次のリクエストを使用して、ページの HTML コンテンツを取得するときに返されます。</span><span class="sxs-lookup"><span data-stu-id="97e76-109">The file's resource URI is returned when you get a page's HTML content using the following request:</span></span>

```
GET ../onenote/pages/{id}/content
```

<span data-ttu-id="97e76-110">ページ HTML では、`img` タグには、`data-fullres-src` 属性の元のイメージ リソースのエンドポイントと、`src` 属性の最適化されたイメージのエンドポイントが含まれます。</span><span class="sxs-lookup"><span data-stu-id="97e76-110">In the page HTML, an `img` tag includes endpoints for the original image resource in the `data-fullres-src` attribute and the optimized image in the `src` attribute:</span></span>
```
<img 
    src="image-resource-url"  
    data-src-type="media-type"
    data-fullres-src="image-resource-url"  
    data-fullres-src-type="media-type" ... />
```

<span data-ttu-id="97e76-111">`object` タグ (PDF、DOCX、PNG などのファイルを表す) には、`data` 属性のファイル リソースのエンドポイントが含まれます。</span><span class="sxs-lookup"><span data-stu-id="97e76-111">An `object` tag (which represents files such as PDF, DOCX, and PNG) includes the endpoint for the file resource in the `data` attribute:</span></span>

```
<object
    data="file-resource-url"
    data-attachment="file-name.file-type" 
    type="media-type" ... />
```

## <a name="properties"></a><span data-ttu-id="97e76-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="97e76-112">Properties</span></span>
<span data-ttu-id="97e76-113">なし</span><span class="sxs-lookup"><span data-stu-id="97e76-113">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="97e76-114">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="97e76-114">Relationships</span></span>
<span data-ttu-id="97e76-115">なし。</span><span class="sxs-lookup"><span data-stu-id="97e76-115">None.</span></span>


## <a name="methods"></a><span data-ttu-id="97e76-116">メソッド</span><span class="sxs-lookup"><span data-stu-id="97e76-116">Methods</span></span>
| <span data-ttu-id="97e76-117">メソッド</span><span class="sxs-lookup"><span data-stu-id="97e76-117">Method</span></span>           | <span data-ttu-id="97e76-118">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="97e76-118">Return Type</span></span>    |<span data-ttu-id="97e76-119">説明</span><span class="sxs-lookup"><span data-stu-id="97e76-119">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="97e76-120">リソース バイナリ データの取得</span><span class="sxs-lookup"><span data-stu-id="97e76-120">Get resource binary data</span></span>](../api/resource-get.md) | <span data-ttu-id="97e76-121">Stream</span><span class="sxs-lookup"><span data-stu-id="97e76-121">Stream</span></span> |<span data-ttu-id="97e76-122">ファイルまたはイメージ リソースのバイナリ データを取得します。</span><span class="sxs-lookup"><span data-stu-id="97e76-122">Retrieve the binary data of a file or image resource.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "resource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->