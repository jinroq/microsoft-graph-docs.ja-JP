---
author: kevinlam
ms.author: kevinlam
ms.date: 3/16/2018
title: ItemPreviewInfo
ms.openlocfilehash: 8b8f7a962e237cc20a42503efd31f083996ad715
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022646"
---
# <a name="itempreviewinfo-resource-type"></a><span data-ttu-id="f1e7e-102">itemPreviewInfo リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f1e7e-102">itemPreviewInfo resource type</span></span>

<span data-ttu-id="f1e7e-103">**ItemPreviewInfo**リソースには、 [driveItem](driveitem.md)のプレビューを埋め込む方法についての情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="f1e7e-103">The **itemPreviewInfo** resource contains information on how to embed a preview of a [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="f1e7e-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f1e7e-104">JSON representation</span></span>

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

## <a name="properties"></a><span data-ttu-id="f1e7e-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f1e7e-105">Properties</span></span>

| <span data-ttu-id="f1e7e-106">名前</span><span class="sxs-lookup"><span data-stu-id="f1e7e-106">Name</span></span>           | <span data-ttu-id="f1e7e-107">型</span><span class="sxs-lookup"><span data-stu-id="f1e7e-107">Type</span></span>   | <span data-ttu-id="f1e7e-108">説明</span><span class="sxs-lookup"><span data-stu-id="f1e7e-108">Description</span></span>
|:---------------|:-------|:---------------------------------------------------
| <span data-ttu-id="f1e7e-109">getUrl</span><span class="sxs-lookup"><span data-stu-id="f1e7e-109">getUrl</span></span>         | <span data-ttu-id="f1e7e-110">文字列</span><span class="sxs-lookup"><span data-stu-id="f1e7e-110">string</span></span> | <span data-ttu-id="f1e7e-111">HTTP の GET (iframe など) を使用して埋め込みの適切な URL</span><span class="sxs-lookup"><span data-stu-id="f1e7e-111">URL suitable for embedding using HTTP GET (iframes, etc.)</span></span>
| <span data-ttu-id="f1e7e-112">postUrl</span><span class="sxs-lookup"><span data-stu-id="f1e7e-112">postUrl</span></span>        | <span data-ttu-id="f1e7e-113">文字列</span><span class="sxs-lookup"><span data-stu-id="f1e7e-113">string</span></span> | <span data-ttu-id="f1e7e-114">HTTP POST を使用して埋め込みの適切な URL (フォーム ポスト、JS など)。</span><span class="sxs-lookup"><span data-stu-id="f1e7e-114">URL suitable for embedding using HTTP POST (form post, JS, etc.)</span></span>
| <span data-ttu-id="f1e7e-115">postParameters</span><span class="sxs-lookup"><span data-stu-id="f1e7e-115">postParameters</span></span> | <span data-ttu-id="f1e7e-116">文字列</span><span class="sxs-lookup"><span data-stu-id="f1e7e-116">string</span></span> | <span data-ttu-id="f1e7e-117">PostUrl を使用する場合は、POST のパラメーター</span><span class="sxs-lookup"><span data-stu-id="f1e7e-117">POST parameters to include if using postUrl</span></span>

<span data-ttu-id="f1e7e-118">GetUrl、postUrl、またはその両方は、指定したオプションのサポートの現在の状態によって返される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="f1e7e-118">Either getUrl, postUrl, or both may be returned depending on the current state of support for the specified options.</span></span>

<span data-ttu-id="f1e7e-119">として書式設定された文字列は、postParameters`application/x-www-form-urlencoded`と postUrl のコンテンツの種類へのポストを実行し、それに応じて設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="f1e7e-119">postParameters is a string formatted as `application/x-www-form-urlencoded`, and if performing a POST to the postUrl the content-type should be set accordingly.</span></span> <span data-ttu-id="f1e7e-120">例:</span><span class="sxs-lookup"><span data-stu-id="f1e7e-120">For example:</span></span>
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

<span data-ttu-id="f1e7e-121">不透明な Url とパラメーターの形式を検討してください。</span><span class="sxs-lookup"><span data-stu-id="f1e7e-121">The formats of URLs and parameters should be considered opaque.</span></span>
