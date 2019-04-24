---
author: kevinlam
ms.author: kevinlam
ms.date: 3/16/2018
title: itempreviewinfo
localization_priority: Normal
ms.openlocfilehash: e7df636f9c406a499baa5ef3be1748273920cac4
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32585238"
---
# <a name="itempreviewinfo-resource-type"></a><span data-ttu-id="f02b2-102">itempreviewinfo リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f02b2-102">itemPreviewInfo resource type</span></span>

<span data-ttu-id="f02b2-103">**itempreviewinfo**リソースには、[ドライブ項目](driveitem.md)のプレビューを埋め込む方法に関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="f02b2-103">The **itemPreviewInfo** resource contains information on how to embed a preview of a [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="f02b2-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f02b2-104">JSON representation</span></span>

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

## <a name="properties"></a><span data-ttu-id="f02b2-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f02b2-105">Properties</span></span>

| <span data-ttu-id="f02b2-106">名前</span><span class="sxs-lookup"><span data-stu-id="f02b2-106">Name</span></span>           | <span data-ttu-id="f02b2-107">型</span><span class="sxs-lookup"><span data-stu-id="f02b2-107">Type</span></span>   | <span data-ttu-id="f02b2-108">説明</span><span class="sxs-lookup"><span data-stu-id="f02b2-108">Description</span></span>
|:---------------|:-------|:---------------------------------------------------
| <span data-ttu-id="f02b2-109">getUrl</span><span class="sxs-lookup"><span data-stu-id="f02b2-109">getUrl</span></span>         | <span data-ttu-id="f02b2-110">string</span><span class="sxs-lookup"><span data-stu-id="f02b2-110">string</span></span> | <span data-ttu-id="f02b2-111">HTTP GET (iframes など) を使用した埋め込みに適した URL</span><span class="sxs-lookup"><span data-stu-id="f02b2-111">URL suitable for embedding using HTTP GET (iframes, etc.)</span></span>
| <span data-ttu-id="f02b2-112">posturl</span><span class="sxs-lookup"><span data-stu-id="f02b2-112">postUrl</span></span>        | <span data-ttu-id="f02b2-113">string</span><span class="sxs-lookup"><span data-stu-id="f02b2-113">string</span></span> | <span data-ttu-id="f02b2-114">HTTP POST (form post、JS など) を使用した埋め込みに適した URL</span><span class="sxs-lookup"><span data-stu-id="f02b2-114">URL suitable for embedding using HTTP POST (form post, JS, etc.)</span></span>
| <span data-ttu-id="f02b2-115">postparameters</span><span class="sxs-lookup"><span data-stu-id="f02b2-115">postParameters</span></span> | <span data-ttu-id="f02b2-116">string</span><span class="sxs-lookup"><span data-stu-id="f02b2-116">string</span></span> | <span data-ttu-id="f02b2-117">posturl を使用する場合に含める POST パラメーター</span><span class="sxs-lookup"><span data-stu-id="f02b2-117">POST parameters to include if using postUrl</span></span>

<span data-ttu-id="f02b2-118">指定したオプションの現在の状態に応じて、getUrl、posturl、または both のどちらかが返される場合があります。</span><span class="sxs-lookup"><span data-stu-id="f02b2-118">Either getUrl, postUrl, or both may be returned depending on the current state of support for the specified options.</span></span>

<span data-ttu-id="f02b2-119">postparameters はとして`application/x-www-form-urlencoded`書式設定された文字列です。 postparameters への投稿を実行する場合は、コンテンツタイプを適宜設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="f02b2-119">postParameters is a string formatted as `application/x-www-form-urlencoded`, and if performing a POST to the postUrl the content-type should be set accordingly.</span></span> <span data-ttu-id="f02b2-120">次に例を示します。</span><span class="sxs-lookup"><span data-stu-id="f02b2-120">For example:</span></span>
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

<span data-ttu-id="f02b2-121">url とパラメーターの形式は、不明瞭であると見なされます。</span><span class="sxs-lookup"><span data-stu-id="f02b2-121">The formats of URLs and parameters should be considered opaque.</span></span>
