---
author: kevinlam
ms.author: kevinlam
ms.date: 3/16/2018
title: ItemPreviewInfo - OneDrive API
localization_priority: Normal
ms.openlocfilehash: 469679e9baa016560f5a02425bc41d628a24dc2c
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509764"
---
# <a name="itempreviewinfo-resource-type"></a><span data-ttu-id="0cf7f-102">ItemPreviewInfo リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0cf7f-102">ItemPreviewInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0cf7f-103">**ItemPreviewInfo**リソースには、 [DriveItem](driveitem.md)のプレビューを埋め込む方法についての情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="0cf7f-103">The **ItemPreviewInfo** resource contains information on how to embed a preview of a [DriveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="0cf7f-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0cf7f-104">JSON representation</span></span>

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

## <a name="properties"></a><span data-ttu-id="0cf7f-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0cf7f-105">Properties</span></span>

| <span data-ttu-id="0cf7f-106">名前</span><span class="sxs-lookup"><span data-stu-id="0cf7f-106">Name</span></span>           | <span data-ttu-id="0cf7f-107">型</span><span class="sxs-lookup"><span data-stu-id="0cf7f-107">Type</span></span>   | <span data-ttu-id="0cf7f-108">説明</span><span class="sxs-lookup"><span data-stu-id="0cf7f-108">Description</span></span>
|:---------------|:-------|:---------------------------------------------------
| <span data-ttu-id="0cf7f-109">getUrl</span><span class="sxs-lookup"><span data-stu-id="0cf7f-109">getUrl</span></span>         | <span data-ttu-id="0cf7f-110">string</span><span class="sxs-lookup"><span data-stu-id="0cf7f-110">string</span></span> | <span data-ttu-id="0cf7f-111">HTTP の GET (iframe など) を使用して埋め込みの適切な URL</span><span class="sxs-lookup"><span data-stu-id="0cf7f-111">URL suitable for embedding using HTTP GET (iframes, etc.)</span></span>
| <span data-ttu-id="0cf7f-112">postUrl</span><span class="sxs-lookup"><span data-stu-id="0cf7f-112">postUrl</span></span>        | <span data-ttu-id="0cf7f-113">string</span><span class="sxs-lookup"><span data-stu-id="0cf7f-113">string</span></span> | <span data-ttu-id="0cf7f-114">HTTP POST を使用して埋め込みの適切な URL (フォーム ポスト、JS など)。</span><span class="sxs-lookup"><span data-stu-id="0cf7f-114">URL suitable for embedding using HTTP POST (form post, JS, etc.)</span></span>
| <span data-ttu-id="0cf7f-115">postParameters</span><span class="sxs-lookup"><span data-stu-id="0cf7f-115">postParameters</span></span> | <span data-ttu-id="0cf7f-116">string</span><span class="sxs-lookup"><span data-stu-id="0cf7f-116">string</span></span> | <span data-ttu-id="0cf7f-117">PostUrl を使用する場合は、POST のパラメーター</span><span class="sxs-lookup"><span data-stu-id="0cf7f-117">POST parameters to include if using postUrl</span></span>

<span data-ttu-id="0cf7f-118">GetUrl、postUrl、またはその両方は、指定したオプションのサポートの現在の状態によって返される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="0cf7f-118">Either getUrl, postUrl, or both may be returned depending on the current state of support for the specified options.</span></span>

<span data-ttu-id="0cf7f-119">として書式設定された文字列は、postParameters`application/x-www-form-urlencoded`と postUrl のコンテンツの種類へのポストを実行し、それに応じて設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="0cf7f-119">postParameters is a string formatted as `application/x-www-form-urlencoded`, and if performing a POST to the postUrl the content-type should be set accordingly.</span></span> <span data-ttu-id="0cf7f-120">次に例を示します。</span><span class="sxs-lookup"><span data-stu-id="0cf7f-120">For example:</span></span>
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

<span data-ttu-id="0cf7f-121">不透明な Url とパラメーターの形式を検討してください。</span><span class="sxs-lookup"><span data-stu-id="0cf7f-121">The formats of URLs and parameters should be considered opaque.</span></span>
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/itempreviewinfo.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
