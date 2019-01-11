---
title: resource リソースの種類
description: 'イメージまたは OneNote のページ上の他のファイル リソースです。 '
localization_priority: Normal
ms.openlocfilehash: a8ba7b2afb5b083e4fe5250ef499043029a1195b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27879521"
---
# <a name="resource-resource-type"></a><span data-ttu-id="afa8f-103">resource リソースの種類</span><span class="sxs-lookup"><span data-stu-id="afa8f-103">resource resource type</span></span>

> <span data-ttu-id="afa8f-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="afa8f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="afa8f-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="afa8f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="afa8f-106">イメージまたは OneNote のページ上の他のファイル リソースです。</span><span class="sxs-lookup"><span data-stu-id="afa8f-106">An image or other file resource on a OneNote page.</span></span> 

<span data-ttu-id="afa8f-107">リソースのバイナリ データは取得できますが、リソース オブジェクトまたはリソース コレクションの JSON 表記の取得はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="afa8f-107">You can get the binary data of a resource, but getting a JSON representation of a resource object or a resource collection is not supported.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenoteResource"
}-->

<span data-ttu-id="afa8f-108">GET リクエストをリソースの `content` エンドポイントに送信することによって、特定のリソースのバイナリ データを取得します。</span><span class="sxs-lookup"><span data-stu-id="afa8f-108">Get the binary data of a specific resource by sending a GET request to the resource's `content` endpoint:</span></span>

```
GET ../onenote/resources/{id}/content
```

<span data-ttu-id="afa8f-109">ファイルのリソース URI は、次のリクエストを使用して、ページの HTML コンテンツを取得するときに返されます。</span><span class="sxs-lookup"><span data-stu-id="afa8f-109">The file's resource URI is returned when you get a page's HTML content using the following request:</span></span>

```
GET ../onenote/pages/{id}/content
```

<span data-ttu-id="afa8f-110">ページ HTML では、`img` タグには、`data-fullres-src` 属性の元のイメージ リソースのエンドポイントと、`src` 属性の最適化されたイメージのエンドポイントが含まれます。</span><span class="sxs-lookup"><span data-stu-id="afa8f-110">In the page HTML, an `img` tag includes endpoints for the original image resource in the `data-fullres-src` attribute and the optimized image in the `src` attribute:</span></span>
```
<img 
    src="image-resource-url"  
    data-src-type="media-type"
    data-fullres-src="image-resource-url"  
    data-fullres-src-type="media-type" ... />
```

<span data-ttu-id="afa8f-111">`object` タグ (PDF、DOCX、PNG などのファイルを表す) には、`data` 属性のファイル リソースのエンドポイントが含まれます。</span><span class="sxs-lookup"><span data-stu-id="afa8f-111">An `object` tag (which represents files such as PDF, DOCX, and PNG) includes the endpoint for the file resource in the `data` attribute:</span></span>

```
<object
    data="file-resource-url"
    data-attachment="file-name.file-type" 
    type="media-type" ... />
```

## <a name="properties"></a><span data-ttu-id="afa8f-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="afa8f-112">Properties</span></span>
<span data-ttu-id="afa8f-113">なし</span><span class="sxs-lookup"><span data-stu-id="afa8f-113">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="afa8f-114">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="afa8f-114">Relationships</span></span>
<span data-ttu-id="afa8f-115">なし。</span><span class="sxs-lookup"><span data-stu-id="afa8f-115">None.</span></span>


## <a name="methods"></a><span data-ttu-id="afa8f-116">メソッド</span><span class="sxs-lookup"><span data-stu-id="afa8f-116">Methods</span></span>
| <span data-ttu-id="afa8f-117">メソッド</span><span class="sxs-lookup"><span data-stu-id="afa8f-117">Method</span></span>           | <span data-ttu-id="afa8f-118">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="afa8f-118">Return Type</span></span>    |<span data-ttu-id="afa8f-119">説明</span><span class="sxs-lookup"><span data-stu-id="afa8f-119">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="afa8f-120">リソース バイナリ データの取得</span><span class="sxs-lookup"><span data-stu-id="afa8f-120">Get resource binary data</span></span>](../api/resource-get.md) | <span data-ttu-id="afa8f-121">Stream</span><span class="sxs-lookup"><span data-stu-id="afa8f-121">Stream</span></span> |<span data-ttu-id="afa8f-122">ファイルまたはイメージ リソースのバイナリ データを取得します。</span><span class="sxs-lookup"><span data-stu-id="afa8f-122">Retrieve the binary data of a file or image resource.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "resource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
