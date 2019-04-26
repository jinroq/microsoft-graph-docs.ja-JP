---
title: resource リソースの種類
description: 'OneNote ページ上の画像またはその他のファイルリソース。 '
localization_priority: Normal
ms.openlocfilehash: c85897af91290df83f4d6fccaf0552513b4f0535
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32563022"
---
# <a name="resource-resource-type"></a><span data-ttu-id="79fff-103">resource リソースの種類</span><span class="sxs-lookup"><span data-stu-id="79fff-103">resource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="79fff-104">OneNote ページ上の画像またはその他のファイルリソース。</span><span class="sxs-lookup"><span data-stu-id="79fff-104">An image or other file resource on a OneNote page.</span></span> 

<span data-ttu-id="79fff-105">リソースのバイナリデータを取得することはできますが、リソースオブジェクトまたはリソースコレクションの JSON 表記を取得することはサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="79fff-105">You can get the binary data of a resource, but getting a JSON representation of a resource object or a resource collection is not supported.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.onenoteResource"
}-->

<span data-ttu-id="79fff-106">特定のリソースのバイナリデータを取得するために、get 要求をリソースの`content`エンドポイントに送信します。</span><span class="sxs-lookup"><span data-stu-id="79fff-106">Get the binary data of a specific resource by sending a GET request to the resource's `content` endpoint:</span></span>

```
GET ../onenote/resources/{id}/content
```

<span data-ttu-id="79fff-107">ファイルのリソース URI は、次の要求を使用してページの HTML コンテンツを取得したときに返されます。</span><span class="sxs-lookup"><span data-stu-id="79fff-107">The file's resource URI is returned when you get a page's HTML content using the following request:</span></span>

```
GET ../onenote/pages/{id}/content
```

<span data-ttu-id="79fff-108">ページ HTML の場合、 `img`タグには、 `data-fullres-src`属性内の元のイメージリソースのエンドポイントと、 `src`属性の最適化されたイメージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="79fff-108">In the page HTML, an `img` tag includes endpoints for the original image resource in the `data-fullres-src` attribute and the optimized image in the `src` attribute:</span></span>
```
<img 
    src="image-resource-url"  
    data-src-type="media-type"
    data-fullres-src="image-resource-url"  
    data-fullres-src-type="media-type" ... />
```

<span data-ttu-id="79fff-109">`object`タグ (PDF、.docx、PNG などのファイルを表す) には、 `data`属性のファイルリソースのエンドポイントが含まれています。</span><span class="sxs-lookup"><span data-stu-id="79fff-109">An `object` tag (which represents files such as PDF, DOCX, and PNG) includes the endpoint for the file resource in the `data` attribute:</span></span>

```
<object
    data="file-resource-url"
    data-attachment="file-name.file-type" 
    type="media-type" ... />
```

## <a name="properties"></a><span data-ttu-id="79fff-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="79fff-110">Properties</span></span>
<span data-ttu-id="79fff-111">なし</span><span class="sxs-lookup"><span data-stu-id="79fff-111">None.</span></span>

## <a name="relationships"></a><span data-ttu-id="79fff-112">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="79fff-112">Relationships</span></span>
<span data-ttu-id="79fff-113">なし。</span><span class="sxs-lookup"><span data-stu-id="79fff-113">None.</span></span>


## <a name="methods"></a><span data-ttu-id="79fff-114">メソッド</span><span class="sxs-lookup"><span data-stu-id="79fff-114">Methods</span></span>
| <span data-ttu-id="79fff-115">メソッド</span><span class="sxs-lookup"><span data-stu-id="79fff-115">Method</span></span>           | <span data-ttu-id="79fff-116">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="79fff-116">Return Type</span></span>    |<span data-ttu-id="79fff-117">説明</span><span class="sxs-lookup"><span data-stu-id="79fff-117">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="79fff-118">リソースバイナリデータの取得</span><span class="sxs-lookup"><span data-stu-id="79fff-118">Get resource binary data</span></span>](../api/resource-get.md) | <span data-ttu-id="79fff-119">Stream</span><span class="sxs-lookup"><span data-stu-id="79fff-119">Stream</span></span> |<span data-ttu-id="79fff-120">ファイルまたはイメージリソースのバイナリデータを取得します。</span><span class="sxs-lookup"><span data-stu-id="79fff-120">Retrieve the binary data of a file or image resource.</span></span>|

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
