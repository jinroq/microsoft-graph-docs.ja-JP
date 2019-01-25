---
title: resource リソースの種類
description: 'イメージまたは OneNote のページ上の他のファイル リソースです。 '
localization_priority: Normal
ms.openlocfilehash: c85897af91290df83f4d6fccaf0552513b4f0535
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510282"
---
# <a name="resource-resource-type"></a><span data-ttu-id="218bb-103">resource リソースの種類</span><span class="sxs-lookup"><span data-stu-id="218bb-103">resource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="218bb-104">イメージまたは OneNote のページ上の他のファイル リソースです。</span><span class="sxs-lookup"><span data-stu-id="218bb-104">An image or other file resource on a OneNote page.</span></span> 

<span data-ttu-id="218bb-105">リソースのバイナリ データは取得できますが、リソース オブジェクトまたはリソース コレクションの JSON 表記の取得はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="218bb-105">You can get the binary data of a resource, but getting a JSON representation of a resource object or a resource collection is not supported.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenoteResource"
}-->

<span data-ttu-id="218bb-106">GET リクエストをリソースの `content` エンドポイントに送信することによって、特定のリソースのバイナリ データを取得します。</span><span class="sxs-lookup"><span data-stu-id="218bb-106">Get the binary data of a specific resource by sending a GET request to the resource's `content` endpoint:</span></span>

```
GET ../onenote/resources/{id}/content
```

<span data-ttu-id="218bb-107">ファイルのリソース URI は、次のリクエストを使用して、ページの HTML コンテンツを取得するときに返されます。</span><span class="sxs-lookup"><span data-stu-id="218bb-107">The file's resource URI is returned when you get a page's HTML content using the following request:</span></span>

```
GET ../onenote/pages/{id}/content
```

<span data-ttu-id="218bb-108">ページ HTML では、`img` タグには、`data-fullres-src` 属性の元のイメージ リソースのエンドポイントと、`src` 属性の最適化されたイメージのエンドポイントが含まれます。</span><span class="sxs-lookup"><span data-stu-id="218bb-108">In the page HTML, an `img` tag includes endpoints for the original image resource in the `data-fullres-src` attribute and the optimized image in the `src` attribute:</span></span>
```
<img 
    src="image-resource-url"  
    data-src-type="media-type"
    data-fullres-src="image-resource-url"  
    data-fullres-src-type="media-type" ... />
```

<span data-ttu-id="218bb-109">`object` タグ (PDF、DOCX、PNG などのファイルを表す) には、`data` 属性のファイル リソースのエンドポイントが含まれます。</span><span class="sxs-lookup"><span data-stu-id="218bb-109">An `object` tag (which represents files such as PDF, DOCX, and PNG) includes the endpoint for the file resource in the `data` attribute:</span></span>

```
<object
    data="file-resource-url"
    data-attachment="file-name.file-type" 
    type="media-type" ... />
```

## <a name="properties"></a><span data-ttu-id="218bb-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="218bb-110">Properties</span></span>
<span data-ttu-id="218bb-111">なし</span><span class="sxs-lookup"><span data-stu-id="218bb-111">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="218bb-112">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="218bb-112">Relationships</span></span>
<span data-ttu-id="218bb-113">なし。</span><span class="sxs-lookup"><span data-stu-id="218bb-113">None.</span></span>


## <a name="methods"></a><span data-ttu-id="218bb-114">メソッド</span><span class="sxs-lookup"><span data-stu-id="218bb-114">Methods</span></span>
| <span data-ttu-id="218bb-115">メソッド</span><span class="sxs-lookup"><span data-stu-id="218bb-115">Method</span></span>           | <span data-ttu-id="218bb-116">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="218bb-116">Return Type</span></span>    |<span data-ttu-id="218bb-117">説明</span><span class="sxs-lookup"><span data-stu-id="218bb-117">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="218bb-118">リソース バイナリ データの取得</span><span class="sxs-lookup"><span data-stu-id="218bb-118">Get resource binary data</span></span>](../api/resource-get.md) | <span data-ttu-id="218bb-119">Stream</span><span class="sxs-lookup"><span data-stu-id="218bb-119">Stream</span></span> |<span data-ttu-id="218bb-120">ファイルまたはイメージ リソースのバイナリ データを取得します。</span><span class="sxs-lookup"><span data-stu-id="218bb-120">Retrieve the binary data of a file or image resource.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "resource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/resource.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
