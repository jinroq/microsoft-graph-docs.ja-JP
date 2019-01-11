---
title: pageLinks リソースの種類
description: OneNote のページを開くためのリンクです。
localization_priority: Normal
ms.openlocfilehash: a5950366f6c6079443338b68db258c5762c15a7a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27872948"
---
# <a name="pagelinks-resource-type"></a><span data-ttu-id="a66ae-103">pageLinks リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a66ae-103">pageLinks resource type</span></span>

<span data-ttu-id="a66ae-104">OneNote のページを開くためのリンクです。</span><span class="sxs-lookup"><span data-stu-id="a66ae-104">Links for opening a OneNote page.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a66ae-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a66ae-105">JSON representation</span></span>

<span data-ttu-id="a66ae-106">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a66ae-106">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.pageLinks"
}-->

```json
{
  "oneNoteClientUrl": {"@odata.type": "microsoft.graph.externalLink"},
  "oneNoteWebUrl": {"@odata.type": "microsoft.graph.externalLink"}
}

```
## <a name="properties"></a><span data-ttu-id="a66ae-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a66ae-107">Properties</span></span>
| <span data-ttu-id="a66ae-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a66ae-108">Property</span></span>     | <span data-ttu-id="a66ae-109">種類</span><span class="sxs-lookup"><span data-stu-id="a66ae-109">Type</span></span>   |<span data-ttu-id="a66ae-110">説明</span><span class="sxs-lookup"><span data-stu-id="a66ae-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a66ae-111">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="a66ae-111">oneNoteClientUrl</span></span>|[<span data-ttu-id="a66ae-112">externalLink</span><span class="sxs-lookup"><span data-stu-id="a66ae-112">externalLink</span></span>](externallink.md)|<span data-ttu-id="a66ae-113">OneNote のネイティブ クライアントでページを開きます (インストールされている場合)。</span><span class="sxs-lookup"><span data-stu-id="a66ae-113">Opens the page in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="a66ae-114">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="a66ae-114">oneNoteWebUrl</span></span>|[<span data-ttu-id="a66ae-115">externalLink</span><span class="sxs-lookup"><span data-stu-id="a66ae-115">externalLink</span></span>](externallink.md)|<span data-ttu-id="a66ae-116">OneNote Online でページを開きます。</span><span class="sxs-lookup"><span data-stu-id="a66ae-116">Opens the page in OneNote Online.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "pageLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
