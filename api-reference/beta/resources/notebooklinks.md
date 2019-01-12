---
title: notebookLinks リソースの種類
description: OneNote ノートブックを開くためのリンクです。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: da6896fccbea412fb29d88e02088dd7a52e25173
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27956179"
---
# <a name="notebooklinks-resource-type"></a><span data-ttu-id="2b19b-103">notebookLinks リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2b19b-103">notebookLinks resource type</span></span>

> <span data-ttu-id="2b19b-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2b19b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2b19b-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2b19b-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2b19b-106">OneNote ノートブックを開くためのリンクです。</span><span class="sxs-lookup"><span data-stu-id="2b19b-106">Links for opening a OneNote notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2b19b-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2b19b-107">JSON representation</span></span>

<span data-ttu-id="2b19b-108">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2b19b-108">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.notebookLinks"
}-->

```json
{
  "oneNoteClientUrl": {"@odata.type": "microsoft.graph.externalLink"},
  "oneNoteWebUrl": {"@odata.type": "microsoft.graph.externalLink"}
}

```
## <a name="properties"></a><span data-ttu-id="2b19b-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2b19b-109">Properties</span></span>
| <span data-ttu-id="2b19b-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2b19b-110">Property</span></span>     | <span data-ttu-id="2b19b-111">種類</span><span class="sxs-lookup"><span data-stu-id="2b19b-111">Type</span></span>   |<span data-ttu-id="2b19b-112">説明</span><span class="sxs-lookup"><span data-stu-id="2b19b-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2b19b-113">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="2b19b-113">oneNoteClientUrl</span></span>|[<span data-ttu-id="2b19b-114">externalLink</span><span class="sxs-lookup"><span data-stu-id="2b19b-114">externalLink</span></span>](externallink.md)|<span data-ttu-id="2b19b-115">OneNote のネイティブ クライアントでノートブックを開きます (インストールされている場合)。</span><span class="sxs-lookup"><span data-stu-id="2b19b-115">Opens the notebook in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="2b19b-116">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="2b19b-116">oneNoteWebUrl</span></span>|[<span data-ttu-id="2b19b-117">externalLink</span><span class="sxs-lookup"><span data-stu-id="2b19b-117">externalLink</span></span>](externallink.md)|<span data-ttu-id="2b19b-118">OneNote Online でノートブックを開きます。</span><span class="sxs-lookup"><span data-stu-id="2b19b-118">Opens the notebook in OneNote Online.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "notebookLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
