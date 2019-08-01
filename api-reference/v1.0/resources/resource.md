---
title: OneNoteResource リソースの種類
description: 'OneNote ページ上の画像またはその他のファイルリソース。 '
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: cd8ea18047aa3f24343411f8dafd7a79357da87b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36034693"
---
# <a name="onenoteresource-resource-type"></a><span data-ttu-id="a89b7-103">OneNoteResource リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a89b7-103">OneNoteResource resource type</span></span>

<span data-ttu-id="a89b7-104">OneNote ページ上の画像またはその他のファイルリソース。</span><span class="sxs-lookup"><span data-stu-id="a89b7-104">An image or other file resource on a OneNote page.</span></span> 

<span data-ttu-id="a89b7-105">リソースのバイナリデータを取得することはできますが、リソースオブジェクトまたはリソースコレクションの JSON 表記を取得することはサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a89b7-105">You can get the binary data of a resource, but getting a JSON representation of a resource object or a resource collection is not supported.</span></span>

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

<span data-ttu-id="a89b7-106">特定のリソースのバイナリデータを取得するために、GET 要求をリソースの`content`エンドポイントに送信します。</span><span class="sxs-lookup"><span data-stu-id="a89b7-106">Get the binary data of a specific resource by sending a GET request to the resource's `content` endpoint:</span></span>

```
GET ../onenote/resources/{id}/content
```

<span data-ttu-id="a89b7-107">ファイルのリソース URI は、次の要求を使用してページの HTML コンテンツを取得したときに返されます。</span><span class="sxs-lookup"><span data-stu-id="a89b7-107">The file's resource URI is returned when you get a page's HTML content using the following request:</span></span>

```
GET ../onenote/pages/{id}/content
```

<span data-ttu-id="a89b7-108">ページ HTML の場合、 `img`タグには、 `data-fullres-src`属性内の元のイメージリソースのエンドポイントと、 `src`属性の最適化されたイメージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="a89b7-108">In the page HTML, an `img` tag includes endpoints for the original image resource in the `data-fullres-src` attribute and the optimized image in the `src` attribute:</span></span>
```
<img 
    src="image-resource-url"  
    data-src-type="media-type"
    data-fullres-src="image-resource-url"  
    data-fullres-src-type="media-type" ... />
```

<span data-ttu-id="a89b7-109">`object`タグ (PDF、.DOCX、PNG などのファイルを表す) には、 `data`属性のファイルリソースのエンドポイントが含まれています。</span><span class="sxs-lookup"><span data-stu-id="a89b7-109">An `object` tag (which represents files such as PDF, DOCX, and PNG) includes the endpoint for the file resource in the `data` attribute:</span></span>

```
<object
    data="file-resource-url"
    data-attachment="file-name.file-type" 
    type="media-type" ... />
```

## <a name="properties"></a><span data-ttu-id="a89b7-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a89b7-110">Properties</span></span>

| <span data-ttu-id="a89b7-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a89b7-111">Property</span></span>             | <span data-ttu-id="a89b7-112">型</span><span class="sxs-lookup"><span data-stu-id="a89b7-112">Type</span></span>            | <span data-ttu-id="a89b7-113">説明</span><span class="sxs-lookup"><span data-stu-id="a89b7-113">Description</span></span>
|:---------------------|:----------------|:---------------------------------
| <span data-ttu-id="a89b7-114">content</span><span class="sxs-lookup"><span data-stu-id="a89b7-114">content</span></span>              | <span data-ttu-id="a89b7-115">Stream</span><span class="sxs-lookup"><span data-stu-id="a89b7-115">Stream</span></span>          | <span data-ttu-id="a89b7-116">コンテンツストリーム</span><span class="sxs-lookup"><span data-stu-id="a89b7-116">The content stream</span></span>
| <span data-ttu-id="a89b7-117">contentUrl</span><span class="sxs-lookup"><span data-stu-id="a89b7-117">contentUrl</span></span>           | <span data-ttu-id="a89b7-118">String (url)</span><span class="sxs-lookup"><span data-stu-id="a89b7-118">String (url)</span></span>    | <span data-ttu-id="a89b7-119">コンテンツをダウンロードするための URL</span><span class="sxs-lookup"><span data-stu-id="a89b7-119">The URL for downloading the content</span></span>

## <a name="relationships"></a><span data-ttu-id="a89b7-120">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a89b7-120">Relationships</span></span>
<span data-ttu-id="a89b7-121">なし。</span><span class="sxs-lookup"><span data-stu-id="a89b7-121">None.</span></span>


## <a name="methods"></a><span data-ttu-id="a89b7-122">メソッド</span><span class="sxs-lookup"><span data-stu-id="a89b7-122">Methods</span></span>
| <span data-ttu-id="a89b7-123">メソッド</span><span class="sxs-lookup"><span data-stu-id="a89b7-123">Method</span></span>           | <span data-ttu-id="a89b7-124">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="a89b7-124">Return Type</span></span>    |<span data-ttu-id="a89b7-125">説明</span><span class="sxs-lookup"><span data-stu-id="a89b7-125">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="a89b7-126">リソースバイナリデータの取得</span><span class="sxs-lookup"><span data-stu-id="a89b7-126">Get resource binary data</span></span>](../api/resource-get.md) | <span data-ttu-id="a89b7-127">Stream</span><span class="sxs-lookup"><span data-stu-id="a89b7-127">Stream</span></span> |<span data-ttu-id="a89b7-128">ファイルまたはイメージリソースのバイナリデータを取得します。</span><span class="sxs-lookup"><span data-stu-id="a89b7-128">Retrieve the binary data of a file or image resource.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "resource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
