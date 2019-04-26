---
author: kevinlam
ms.author: kevinlam
ms.date: 3/16/2018
title: itempreviewinfo-OneDrive API
localization_priority: Normal
ms.openlocfilehash: c43626292cd07ad14d27202255a499b413dbae63
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345513"
---
# <a name="itempreviewinfo-resource-type"></a><span data-ttu-id="4eaba-102">itempreviewinfo リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4eaba-102">ItemPreviewInfo resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4eaba-103">**itempreviewinfo**リソースには、[ドライブ項目](driveitem.md)のプレビューを埋め込む方法に関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="4eaba-103">The **ItemPreviewInfo** resource contains information on how to embed a preview of a [DriveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="4eaba-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4eaba-104">JSON representation</span></span>

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

## <a name="properties"></a><span data-ttu-id="4eaba-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4eaba-105">Properties</span></span>

| <span data-ttu-id="4eaba-106">名前</span><span class="sxs-lookup"><span data-stu-id="4eaba-106">Name</span></span>           | <span data-ttu-id="4eaba-107">型</span><span class="sxs-lookup"><span data-stu-id="4eaba-107">Type</span></span>   | <span data-ttu-id="4eaba-108">説明</span><span class="sxs-lookup"><span data-stu-id="4eaba-108">Description</span></span>
|:---------------|:-------|:---------------------------------------------------
| <span data-ttu-id="4eaba-109">getUrl</span><span class="sxs-lookup"><span data-stu-id="4eaba-109">getUrl</span></span>         | <span data-ttu-id="4eaba-110">string</span><span class="sxs-lookup"><span data-stu-id="4eaba-110">string</span></span> | <span data-ttu-id="4eaba-111">HTTP GET (iframes など) を使用した埋め込みに適した URL</span><span class="sxs-lookup"><span data-stu-id="4eaba-111">URL suitable for embedding using HTTP GET (iframes, etc.)</span></span>
| <span data-ttu-id="4eaba-112">posturl</span><span class="sxs-lookup"><span data-stu-id="4eaba-112">postUrl</span></span>        | <span data-ttu-id="4eaba-113">string</span><span class="sxs-lookup"><span data-stu-id="4eaba-113">string</span></span> | <span data-ttu-id="4eaba-114">HTTP POST (form post、JS など) を使用した埋め込みに適した URL</span><span class="sxs-lookup"><span data-stu-id="4eaba-114">URL suitable for embedding using HTTP POST (form post, JS, etc.)</span></span>
| <span data-ttu-id="4eaba-115">postparameters</span><span class="sxs-lookup"><span data-stu-id="4eaba-115">postParameters</span></span> | <span data-ttu-id="4eaba-116">string</span><span class="sxs-lookup"><span data-stu-id="4eaba-116">string</span></span> | <span data-ttu-id="4eaba-117">posturl を使用する場合に含める POST パラメーター</span><span class="sxs-lookup"><span data-stu-id="4eaba-117">POST parameters to include if using postUrl</span></span>

<span data-ttu-id="4eaba-118">指定したオプションの現在の状態に応じて、getUrl、posturl、または both のどちらかが返される場合があります。</span><span class="sxs-lookup"><span data-stu-id="4eaba-118">Either getUrl, postUrl, or both may be returned depending on the current state of support for the specified options.</span></span>

<span data-ttu-id="4eaba-119">postparameters はとして`application/x-www-form-urlencoded`書式設定された文字列です。 postparameters への投稿を実行する場合は、コンテンツタイプを適宜設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="4eaba-119">postParameters is a string formatted as `application/x-www-form-urlencoded`, and if performing a POST to the postUrl the content-type should be set accordingly.</span></span> <span data-ttu-id="4eaba-120">例:</span><span class="sxs-lookup"><span data-stu-id="4eaba-120">For example:</span></span>
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

<span data-ttu-id="4eaba-121">url とパラメーターの形式は、不明瞭であると見なされます。</span><span class="sxs-lookup"><span data-stu-id="4eaba-121">The formats of URLs and parameters should be considered opaque.</span></span>
