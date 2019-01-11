---
title: OneNoteResource リソースの種類
description: 'イメージまたは OneNote のページ上の他のファイル リソースです。 '
localization_priority: Normal
ms.openlocfilehash: ed2fb0dd4b6e68c24da1f2441a157f734a5025f6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27855105"
---
# <a name="onenoteresource-resource-type"></a><span data-ttu-id="f7c6f-103">OneNoteResource リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f7c6f-103">OneNoteResource resource type</span></span>

<span data-ttu-id="f7c6f-104">イメージまたは OneNote のページ上の他のファイル リソースです。</span><span class="sxs-lookup"><span data-stu-id="f7c6f-104">An image or other file resource on a OneNote page.</span></span> 

<span data-ttu-id="f7c6f-105">リソースのバイナリ データは取得できますが、リソース オブジェクトまたはリソース コレクションの JSON 表記の取得はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f7c6f-105">You can get the binary data of a resource, but getting a JSON representation of a resource object or a resource collection is not supported.</span></span>

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.onenoteEntityBaseModel",
  "optionalProperties": [],
  "isMediaEntity": true,
  "@odata.type": "microsoft.graph.onenoteResource"
}-->

```json
{
  "content": { "@odata.type": "Edm.Stream" },
  "contentUrl": "string (url)"
}
```

<span data-ttu-id="f7c6f-106">GET リクエストをリソースの `content` エンドポイントに送信することによって、特定のリソースのバイナリ データを取得します。</span><span class="sxs-lookup"><span data-stu-id="f7c6f-106">Get the binary data of a specific resource by sending a GET request to the resource's `content` endpoint:</span></span>

```
GET ../onenote/resources/{id}/content
```

<span data-ttu-id="f7c6f-107">ファイルのリソース URI は、次のリクエストを使用して、ページの HTML コンテンツを取得するときに返されます。</span><span class="sxs-lookup"><span data-stu-id="f7c6f-107">The file's resource URI is returned when you get a page's HTML content using the following request:</span></span>

```
GET ../onenote/pages/{id}/content
```

<span data-ttu-id="f7c6f-108">ページ HTML では、`img` タグには、`data-fullres-src` 属性の元のイメージ リソースのエンドポイントと、`src` 属性の最適化されたイメージのエンドポイントが含まれます。</span><span class="sxs-lookup"><span data-stu-id="f7c6f-108">In the page HTML, an `img` tag includes endpoints for the original image resource in the `data-fullres-src` attribute and the optimized image in the `src` attribute:</span></span>
```
<img 
    src="image-resource-url"  
    data-src-type="media-type"
    data-fullres-src="image-resource-url"  
    data-fullres-src-type="media-type" ... />
```

<span data-ttu-id="f7c6f-109">`object` タグ (PDF、DOCX、PNG などのファイルを表す) には、`data` 属性のファイル リソースのエンドポイントが含まれます。</span><span class="sxs-lookup"><span data-stu-id="f7c6f-109">An `object` tag (which represents files such as PDF, DOCX, and PNG) includes the endpoint for the file resource in the `data` attribute:</span></span>

```
<object
    data="file-resource-url"
    data-attachment="file-name.file-type" 
    type="media-type" ... />
```

## <a name="properties"></a><span data-ttu-id="f7c6f-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f7c6f-110">Properties</span></span>

| <span data-ttu-id="f7c6f-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f7c6f-111">Property</span></span>             | <span data-ttu-id="f7c6f-112">種類</span><span class="sxs-lookup"><span data-stu-id="f7c6f-112">Type</span></span>            | <span data-ttu-id="f7c6f-113">説明</span><span class="sxs-lookup"><span data-stu-id="f7c6f-113">Description</span></span>
|:---------------------|:----------------|:---------------------------------
| <span data-ttu-id="f7c6f-114">content</span><span class="sxs-lookup"><span data-stu-id="f7c6f-114">content</span></span>              | <span data-ttu-id="f7c6f-115">Stream</span><span class="sxs-lookup"><span data-stu-id="f7c6f-115">Stream</span></span>          | <span data-ttu-id="f7c6f-116">コンテンツ ストリーム</span><span class="sxs-lookup"><span data-stu-id="f7c6f-116">The content stream</span></span>
| <span data-ttu-id="f7c6f-117">contentUrl</span><span class="sxs-lookup"><span data-stu-id="f7c6f-117">contentUrl</span></span>           | <span data-ttu-id="f7c6f-118">文字列 (url)</span><span class="sxs-lookup"><span data-stu-id="f7c6f-118">String (url)</span></span>    | <span data-ttu-id="f7c6f-119">コンテンツをダウンロードするための URL</span><span class="sxs-lookup"><span data-stu-id="f7c6f-119">The URL for downloading the content</span></span>

## <a name="relationships"></a><span data-ttu-id="f7c6f-120">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f7c6f-120">Relationships</span></span>
<span data-ttu-id="f7c6f-121">なし。</span><span class="sxs-lookup"><span data-stu-id="f7c6f-121">None.</span></span>


## <a name="methods"></a><span data-ttu-id="f7c6f-122">メソッド</span><span class="sxs-lookup"><span data-stu-id="f7c6f-122">Methods</span></span>
| <span data-ttu-id="f7c6f-123">メソッド</span><span class="sxs-lookup"><span data-stu-id="f7c6f-123">Method</span></span>           | <span data-ttu-id="f7c6f-124">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="f7c6f-124">Return Type</span></span>    |<span data-ttu-id="f7c6f-125">説明</span><span class="sxs-lookup"><span data-stu-id="f7c6f-125">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="f7c6f-126">リソース バイナリ データの取得</span><span class="sxs-lookup"><span data-stu-id="f7c6f-126">Get resource binary data</span></span>](../api/resource-get.md) | <span data-ttu-id="f7c6f-127">Stream</span><span class="sxs-lookup"><span data-stu-id="f7c6f-127">Stream</span></span> |<span data-ttu-id="f7c6f-128">ファイルまたはイメージ リソースのバイナリ データを取得します。</span><span class="sxs-lookup"><span data-stu-id="f7c6f-128">Retrieve the binary data of a file or image resource.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "resource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
