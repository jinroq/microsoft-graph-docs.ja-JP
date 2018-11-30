---
author: kevinlam
ms.author: kevinlam
ms.date: 3/16/2018
title: ItemPreviewInfo - OneDrive API
ms.openlocfilehash: 3fa9d10ae3aade7be96e81168b34df84698da1c1
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27068136"
---
# <a name="itempreviewinfo-resource-type"></a><span data-ttu-id="27832-102">ItemPreviewInfo リソースの種類</span><span class="sxs-lookup"><span data-stu-id="27832-102">ItemPreviewInfo resource type</span></span>

> <span data-ttu-id="27832-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="27832-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="27832-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="27832-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="27832-105">**ItemPreviewInfo**リソースには、 [DriveItem](driveitem.md)のプレビューを埋め込む方法についての情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="27832-105">The **ItemPreviewInfo** resource contains information on how to embed a preview of a [DriveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="27832-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="27832-106">JSON representation</span></span>

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

## <a name="properties"></a><span data-ttu-id="27832-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="27832-107">Properties</span></span>

| <span data-ttu-id="27832-108">名前</span><span class="sxs-lookup"><span data-stu-id="27832-108">Name</span></span>           | <span data-ttu-id="27832-109">型</span><span class="sxs-lookup"><span data-stu-id="27832-109">Type</span></span>   | <span data-ttu-id="27832-110">説明</span><span class="sxs-lookup"><span data-stu-id="27832-110">Description</span></span>
|:---------------|:-------|:---------------------------------------------------
| <span data-ttu-id="27832-111">getUrl</span><span class="sxs-lookup"><span data-stu-id="27832-111">getUrl</span></span>         | <span data-ttu-id="27832-112">文字列</span><span class="sxs-lookup"><span data-stu-id="27832-112">string</span></span> | <span data-ttu-id="27832-113">HTTP の GET (iframe など) を使用して埋め込みの適切な URL</span><span class="sxs-lookup"><span data-stu-id="27832-113">URL suitable for embedding using HTTP GET (iframes, etc.)</span></span>
| <span data-ttu-id="27832-114">postUrl</span><span class="sxs-lookup"><span data-stu-id="27832-114">postUrl</span></span>        | <span data-ttu-id="27832-115">文字列</span><span class="sxs-lookup"><span data-stu-id="27832-115">string</span></span> | <span data-ttu-id="27832-116">HTTP POST を使用して埋め込みの適切な URL (フォーム ポスト、JS など)。</span><span class="sxs-lookup"><span data-stu-id="27832-116">URL suitable for embedding using HTTP POST (form post, JS, etc.)</span></span>
| <span data-ttu-id="27832-117">postParameters</span><span class="sxs-lookup"><span data-stu-id="27832-117">postParameters</span></span> | <span data-ttu-id="27832-118">文字列</span><span class="sxs-lookup"><span data-stu-id="27832-118">string</span></span> | <span data-ttu-id="27832-119">PostUrl を使用する場合は、POST のパラメーター</span><span class="sxs-lookup"><span data-stu-id="27832-119">POST parameters to include if using postUrl</span></span>

<span data-ttu-id="27832-120">GetUrl、postUrl、またはその両方は、指定したオプションのサポートの現在の状態によって返される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="27832-120">Either getUrl, postUrl, or both may be returned depending on the current state of support for the specified options.</span></span>

<span data-ttu-id="27832-121">として書式設定された文字列は、postParameters`application/x-www-form-urlencoded`と postUrl のコンテンツの種類へのポストを実行し、それに応じて設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="27832-121">postParameters is a string formatted as `application/x-www-form-urlencoded`, and if performing a POST to the postUrl the content-type should be set accordingly.</span></span> <span data-ttu-id="27832-122">例:</span><span class="sxs-lookup"><span data-stu-id="27832-122">For example:</span></span>
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

<span data-ttu-id="27832-123">不透明な Url とパラメーターの形式を検討してください。</span><span class="sxs-lookup"><span data-stu-id="27832-123">The formats of URLs and parameters should be considered opaque.</span></span>