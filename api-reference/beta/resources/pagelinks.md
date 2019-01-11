---
title: pageLinks リソースの種類
description: OneNote のページを開くためのリンクです。
localization_priority: Normal
ms.openlocfilehash: 9bee1b4d3d327118dbf1deec83a37787bd4b18e2
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27832628"
---
# <a name="pagelinks-resource-type"></a><span data-ttu-id="78fda-103">pageLinks リソースの種類</span><span class="sxs-lookup"><span data-stu-id="78fda-103">pageLinks resource type</span></span>

> <span data-ttu-id="78fda-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="78fda-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="78fda-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="78fda-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="78fda-106">OneNote のページを開くためのリンクです。</span><span class="sxs-lookup"><span data-stu-id="78fda-106">Links for opening a OneNote page.</span></span>

## <a name="json-representation"></a><span data-ttu-id="78fda-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="78fda-107">JSON representation</span></span>

<span data-ttu-id="78fda-108">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="78fda-108">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="78fda-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="78fda-109">Properties</span></span>
| <span data-ttu-id="78fda-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="78fda-110">Property</span></span>     | <span data-ttu-id="78fda-111">種類</span><span class="sxs-lookup"><span data-stu-id="78fda-111">Type</span></span>   |<span data-ttu-id="78fda-112">説明</span><span class="sxs-lookup"><span data-stu-id="78fda-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="78fda-113">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="78fda-113">oneNoteClientUrl</span></span>|[<span data-ttu-id="78fda-114">externalLink</span><span class="sxs-lookup"><span data-stu-id="78fda-114">externalLink</span></span>](externallink.md)|<span data-ttu-id="78fda-115">OneNote のネイティブ クライアントでページを開きます (インストールされている場合)。</span><span class="sxs-lookup"><span data-stu-id="78fda-115">Opens the page in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="78fda-116">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="78fda-116">oneNoteWebUrl</span></span>|[<span data-ttu-id="78fda-117">externalLink</span><span class="sxs-lookup"><span data-stu-id="78fda-117">externalLink</span></span>](externallink.md)|<span data-ttu-id="78fda-118">OneNote Online でページを開きます。</span><span class="sxs-lookup"><span data-stu-id="78fda-118">Opens the page in OneNote Online.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "pageLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
