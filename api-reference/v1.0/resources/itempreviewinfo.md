---
author: kevinlam
ms.author: kevinlam
ms.date: 3/16/2018
title: ItemPreviewInfo
localization_priority: Normal
description: ItemPreviewInfo リソースには、ドライブ項目のプレビューを埋め込む方法に関する情報が含まれています。
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 71d660a71bce09f198a0feb9c3acbb9a69a23a5f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36036562"
---
# <a name="itempreviewinfo-resource-type"></a><span data-ttu-id="731f5-103">itemPreviewInfo リソースの種類</span><span class="sxs-lookup"><span data-stu-id="731f5-103">itemPreviewInfo resource type</span></span>

<span data-ttu-id="731f5-104">**Itempreviewinfo**リソースには、[ドライブ項目](driveitem.md)のプレビューを埋め込む方法に関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="731f5-104">The **itemPreviewInfo** resource contains information on how to embed a preview of a [driveItem](driveitem.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="731f5-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="731f5-105">JSON representation</span></span>

```json
{
    "getUrl": "https://www.onedrive.com/embed?foo=bar&bar=baz",
    "postParameters": "param1=value&param2=another%20value",
    "postUrl": "https://www.onedrive.com/embed_by_post"
}
```

## <a name="properties"></a><span data-ttu-id="731f5-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="731f5-106">Properties</span></span>

| <span data-ttu-id="731f5-107">名前</span><span class="sxs-lookup"><span data-stu-id="731f5-107">Name</span></span>           | <span data-ttu-id="731f5-108">型</span><span class="sxs-lookup"><span data-stu-id="731f5-108">Type</span></span>   | <span data-ttu-id="731f5-109">説明</span><span class="sxs-lookup"><span data-stu-id="731f5-109">Description</span></span>
|:---------------|:-------|:---------------------------------------------------
| <span data-ttu-id="731f5-110">getUrl</span><span class="sxs-lookup"><span data-stu-id="731f5-110">getUrl</span></span>         | <span data-ttu-id="731f5-111">string</span><span class="sxs-lookup"><span data-stu-id="731f5-111">string</span></span> | <span data-ttu-id="731f5-112">HTTP GET (iframes など) を使用した埋め込みに適した URL</span><span class="sxs-lookup"><span data-stu-id="731f5-112">URL suitable for embedding using HTTP GET (iframes, etc.)</span></span>
| <span data-ttu-id="731f5-113">postUrl</span><span class="sxs-lookup"><span data-stu-id="731f5-113">postUrl</span></span>        | <span data-ttu-id="731f5-114">string</span><span class="sxs-lookup"><span data-stu-id="731f5-114">string</span></span> | <span data-ttu-id="731f5-115">HTTP POST (form post、JS など) を使用した埋め込みに適した URL</span><span class="sxs-lookup"><span data-stu-id="731f5-115">URL suitable for embedding using HTTP POST (form post, JS, etc.)</span></span>
| <span data-ttu-id="731f5-116">postParameters</span><span class="sxs-lookup"><span data-stu-id="731f5-116">postParameters</span></span> | <span data-ttu-id="731f5-117">string</span><span class="sxs-lookup"><span data-stu-id="731f5-117">string</span></span> | <span data-ttu-id="731f5-118">PostUrl を使用する場合に含める POST パラメーター</span><span class="sxs-lookup"><span data-stu-id="731f5-118">POST parameters to include if using postUrl</span></span>

<span data-ttu-id="731f5-119">指定したオプションの現在の状態に応じて、getUrl、postUrl、または both のどちらかが返される場合があります。</span><span class="sxs-lookup"><span data-stu-id="731f5-119">Either getUrl, postUrl, or both may be returned depending on the current state of support for the specified options.</span></span>

<span data-ttu-id="731f5-120">postParameters はとして`application/x-www-form-urlencoded`書式設定された文字列です。 postparameters への投稿を実行する場合は、コンテンツタイプを適宜設定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="731f5-120">postParameters is a string formatted as `application/x-www-form-urlencoded`, and if performing a POST to the postUrl the content-type should be set accordingly.</span></span> <span data-ttu-id="731f5-121">次に例を示します。</span><span class="sxs-lookup"><span data-stu-id="731f5-121">For example:</span></span>
```
POST https://www.onedrive.com/embed_by_post
Content-Type: application/x-www-form-urlencoded

param1=value&param2=another%20value
```

<span data-ttu-id="731f5-122">Url とパラメーターの形式は、不明瞭であると見なされます。</span><span class="sxs-lookup"><span data-stu-id="731f5-122">The formats of URLs and parameters should be considered opaque.</span></span>
