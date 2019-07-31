---
title: onenoteResource リソースの種類
description: 'OneNote ページ上の画像またはその他のファイルリソース。 '
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 3884be59ed0eedafa9d4a45c851570d08ea70848
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009343"
---
# <a name="onenoteresource-resource-type"></a><span data-ttu-id="5231b-103">onenoteResource リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5231b-103">onenoteResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5231b-104">OneNote ページ上の画像またはその他のファイルリソース。</span><span class="sxs-lookup"><span data-stu-id="5231b-104">An image or other file resource on a OneNote page.</span></span> 

<span data-ttu-id="5231b-105">リソースのバイナリデータを取得することはできますが、リソースオブジェクトまたはリソースコレクションの JSON 表記を取得することはサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5231b-105">You can get the binary data of a resource, but getting a JSON representation of a resource object or a resource collection is not supported.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenoteResource"
}-->

```json
{
  "content": "String (Stream)",
  "contentUrl": "String"
}

```
<span data-ttu-id="5231b-106">特定のリソースのバイナリデータを取得するために、GET 要求をリソースの`content`エンドポイントに送信します。</span><span class="sxs-lookup"><span data-stu-id="5231b-106">Get the binary data of a specific resource by sending a GET request to the resource's `content` endpoint:</span></span>

```
GET ../onenote/resources/{id}/content
```

<span data-ttu-id="5231b-107">ファイルのリソース URI は、次の要求を使用してページの HTML コンテンツを取得したときに返されます。</span><span class="sxs-lookup"><span data-stu-id="5231b-107">The file's resource URI is returned when you get a page's HTML content using the following request:</span></span>

```
GET ../onenote/pages/{id}/content
```

<span data-ttu-id="5231b-108">ページ HTML の場合、 `img`タグには、 `data-fullres-src`属性内の元のイメージリソースのエンドポイントと、 `src`属性の最適化されたイメージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="5231b-108">In the page HTML, an `img` tag includes endpoints for the original image resource in the `data-fullres-src` attribute and the optimized image in the `src` attribute:</span></span>
```
<img 
    src="image-resource-url"  
    data-src-type="media-type"
    data-fullres-src="image-resource-url"  
    data-fullres-src-type="media-type" ... />
```

<span data-ttu-id="5231b-109">`object`タグ (PDF、.DOCX、PNG などのファイルを表す) には、 `data`属性のファイルリソースのエンドポイントが含まれています。</span><span class="sxs-lookup"><span data-stu-id="5231b-109">An `object` tag (which represents files such as PDF, DOCX, and PNG) includes the endpoint for the file resource in the `data` attribute:</span></span>

```
<object
    data="file-resource-url"
    data-attachment="file-name.file-type" 
    type="media-type" ... />
```

## <a name="properties"></a><span data-ttu-id="5231b-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5231b-110">Properties</span></span>
| <span data-ttu-id="5231b-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5231b-111">Property</span></span>     | <span data-ttu-id="5231b-112">型</span><span class="sxs-lookup"><span data-stu-id="5231b-112">Type</span></span>   |<span data-ttu-id="5231b-113">説明</span><span class="sxs-lookup"><span data-stu-id="5231b-113">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="5231b-114">content</span><span class="sxs-lookup"><span data-stu-id="5231b-114">content</span></span> | <span data-ttu-id="5231b-115">Edm ストリーム</span><span class="sxs-lookup"><span data-stu-id="5231b-115">Edm.Stream</span></span>||
| <span data-ttu-id="5231b-116">contentUrl</span><span class="sxs-lookup"><span data-stu-id="5231b-116">contentUrl</span></span> | <span data-ttu-id="5231b-117">String</span><span class="sxs-lookup"><span data-stu-id="5231b-117">String</span></span> ||

## <a name="relationships"></a><span data-ttu-id="5231b-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="5231b-118">Relationships</span></span>
<span data-ttu-id="5231b-119">なし。</span><span class="sxs-lookup"><span data-stu-id="5231b-119">None.</span></span>


## <a name="methods"></a><span data-ttu-id="5231b-120">メソッド</span><span class="sxs-lookup"><span data-stu-id="5231b-120">Methods</span></span>
| <span data-ttu-id="5231b-121">メソッド</span><span class="sxs-lookup"><span data-stu-id="5231b-121">Method</span></span>           | <span data-ttu-id="5231b-122">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="5231b-122">Return Type</span></span>    |<span data-ttu-id="5231b-123">説明</span><span class="sxs-lookup"><span data-stu-id="5231b-123">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="5231b-124">リソースバイナリデータの取得</span><span class="sxs-lookup"><span data-stu-id="5231b-124">Get resource binary data</span></span>](../api/resource-get.md) | <span data-ttu-id="5231b-125">Stream</span><span class="sxs-lookup"><span data-stu-id="5231b-125">Stream</span></span> |<span data-ttu-id="5231b-126">ファイルまたはイメージリソースのバイナリデータを取得します。</span><span class="sxs-lookup"><span data-stu-id="5231b-126">Retrieve the binary data of a file or image resource.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "resource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
