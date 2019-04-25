---
title: OneNoteResource リソースの種類
description: 'OneNote ページ上の画像またはその他のファイルリソース。 '
localization_priority: Normal
ms.openlocfilehash: ed2fb0dd4b6e68c24da1f2441a157f734a5025f6
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32579325"
---
# <a name="onenoteresource-resource-type"></a><span data-ttu-id="25c3d-103">OneNoteResource リソースの種類</span><span class="sxs-lookup"><span data-stu-id="25c3d-103">OneNoteResource resource type</span></span>

<span data-ttu-id="25c3d-104">OneNote ページ上の画像またはその他のファイルリソース。</span><span class="sxs-lookup"><span data-stu-id="25c3d-104">An image or other file resource on a OneNote page.</span></span> 

<span data-ttu-id="25c3d-105">リソースのバイナリデータを取得することはできますが、リソースオブジェクトまたはリソースコレクションの JSON 表記を取得することはサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="25c3d-105">You can get the binary data of a resource, but getting a JSON representation of a resource object or a resource collection is not supported.</span></span>

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

<span data-ttu-id="25c3d-106">特定のリソースのバイナリデータを取得するために、get 要求をリソースの`content`エンドポイントに送信します。</span><span class="sxs-lookup"><span data-stu-id="25c3d-106">Get the binary data of a specific resource by sending a GET request to the resource's `content` endpoint:</span></span>

```
GET ../onenote/resources/{id}/content
```

<span data-ttu-id="25c3d-107">ファイルのリソース URI は、次の要求を使用してページの HTML コンテンツを取得したときに返されます。</span><span class="sxs-lookup"><span data-stu-id="25c3d-107">The file's resource URI is returned when you get a page's HTML content using the following request:</span></span>

```
GET ../onenote/pages/{id}/content
```

<span data-ttu-id="25c3d-108">ページ HTML の場合、 `img`タグには、 `data-fullres-src`属性内の元のイメージリソースのエンドポイントと、 `src`属性の最適化されたイメージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="25c3d-108">In the page HTML, an `img` tag includes endpoints for the original image resource in the `data-fullres-src` attribute and the optimized image in the `src` attribute:</span></span>
```
<img 
    src="image-resource-url"  
    data-src-type="media-type"
    data-fullres-src="image-resource-url"  
    data-fullres-src-type="media-type" ... />
```

<span data-ttu-id="25c3d-109">`object`タグ (PDF、.docx、PNG などのファイルを表す) には、 `data`属性のファイルリソースのエンドポイントが含まれています。</span><span class="sxs-lookup"><span data-stu-id="25c3d-109">An `object` tag (which represents files such as PDF, DOCX, and PNG) includes the endpoint for the file resource in the `data` attribute:</span></span>

```
<object
    data="file-resource-url"
    data-attachment="file-name.file-type" 
    type="media-type" ... />
```

## <a name="properties"></a><span data-ttu-id="25c3d-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="25c3d-110">Properties</span></span>

| <span data-ttu-id="25c3d-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="25c3d-111">Property</span></span>             | <span data-ttu-id="25c3d-112">型</span><span class="sxs-lookup"><span data-stu-id="25c3d-112">Type</span></span>            | <span data-ttu-id="25c3d-113">説明</span><span class="sxs-lookup"><span data-stu-id="25c3d-113">Description</span></span>
|:---------------------|:----------------|:---------------------------------
| <span data-ttu-id="25c3d-114">content</span><span class="sxs-lookup"><span data-stu-id="25c3d-114">content</span></span>              | <span data-ttu-id="25c3d-115">Stream</span><span class="sxs-lookup"><span data-stu-id="25c3d-115">Stream</span></span>          | <span data-ttu-id="25c3d-116">コンテンツストリーム</span><span class="sxs-lookup"><span data-stu-id="25c3d-116">The content stream</span></span>
| <span data-ttu-id="25c3d-117">contentUrl</span><span class="sxs-lookup"><span data-stu-id="25c3d-117">contentUrl</span></span>           | <span data-ttu-id="25c3d-118">String (url)</span><span class="sxs-lookup"><span data-stu-id="25c3d-118">String (url)</span></span>    | <span data-ttu-id="25c3d-119">コンテンツをダウンロードするための URL</span><span class="sxs-lookup"><span data-stu-id="25c3d-119">The URL for downloading the content</span></span>

## <a name="relationships"></a><span data-ttu-id="25c3d-120">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="25c3d-120">Relationships</span></span>
<span data-ttu-id="25c3d-121">なし。</span><span class="sxs-lookup"><span data-stu-id="25c3d-121">None.</span></span>


## <a name="methods"></a><span data-ttu-id="25c3d-122">メソッド</span><span class="sxs-lookup"><span data-stu-id="25c3d-122">Methods</span></span>
| <span data-ttu-id="25c3d-123">メソッド</span><span class="sxs-lookup"><span data-stu-id="25c3d-123">Method</span></span>           | <span data-ttu-id="25c3d-124">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="25c3d-124">Return Type</span></span>    |<span data-ttu-id="25c3d-125">説明</span><span class="sxs-lookup"><span data-stu-id="25c3d-125">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="25c3d-126">リソースバイナリデータの取得</span><span class="sxs-lookup"><span data-stu-id="25c3d-126">Get resource binary data</span></span>](../api/resource-get.md) | <span data-ttu-id="25c3d-127">Stream</span><span class="sxs-lookup"><span data-stu-id="25c3d-127">Stream</span></span> |<span data-ttu-id="25c3d-128">ファイルまたはイメージリソースのバイナリデータを取得します。</span><span class="sxs-lookup"><span data-stu-id="25c3d-128">Retrieve the binary data of a file or image resource.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "resource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
