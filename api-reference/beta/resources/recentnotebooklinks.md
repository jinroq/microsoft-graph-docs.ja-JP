---
title: recentNotebookLinks リソース型
description: OneNote ノートブックを開くへのリンクです。 このリソース型は、recentNotebook リソース上のプロパティとして存在します。
localization_priority: Normal
ms.openlocfilehash: 5ccf861541526a1673d6174176cb8b2a62df6c23
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27812874"
---
# <a name="recentnotebooklinks-resource-type"></a><span data-ttu-id="fe4f8-104">recentNotebookLinks リソース型</span><span class="sxs-lookup"><span data-stu-id="fe4f8-104">recentNotebookLinks resource type</span></span>

> <span data-ttu-id="fe4f8-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="fe4f8-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fe4f8-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fe4f8-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fe4f8-107">OneNote ノートブックを開くへのリンクです。</span><span class="sxs-lookup"><span data-stu-id="fe4f8-107">Links to open a OneNote notebook.</span></span> <span data-ttu-id="fe4f8-108">このリソース型は、[recentNotebook](recentnotebook.md) リソース上のプロパティとして存在します。</span><span class="sxs-lookup"><span data-stu-id="fe4f8-108">This resource type exists as a property on a [recentNotebook](recentnotebook.md) resource.</span></span>

## <a name="properties"></a><span data-ttu-id="fe4f8-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fe4f8-109">Properties</span></span>
| <span data-ttu-id="fe4f8-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fe4f8-110">Property</span></span>     | <span data-ttu-id="fe4f8-111">種類</span><span class="sxs-lookup"><span data-stu-id="fe4f8-111">Type</span></span>   |<span data-ttu-id="fe4f8-112">説明</span><span class="sxs-lookup"><span data-stu-id="fe4f8-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="fe4f8-113">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="fe4f8-113">oneNoteClientUrl</span></span>|[<span data-ttu-id="fe4f8-114">externalLink</span><span class="sxs-lookup"><span data-stu-id="fe4f8-114">externalLink</span></span>](externallink.md)|<span data-ttu-id="fe4f8-115">インストールされている場合は、OneNote クライアントで、ノートブックを開きます。</span><span class="sxs-lookup"><span data-stu-id="fe4f8-115">Opens the notebook in the OneNote client, if it's installed.</span></span>|
|<span data-ttu-id="fe4f8-116">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="fe4f8-116">oneNoteWebUrl</span></span>|[<span data-ttu-id="fe4f8-117">externalLink</span><span class="sxs-lookup"><span data-stu-id="fe4f8-117">externalLink</span></span>](externallink.md)|<span data-ttu-id="fe4f8-118">OneNote Online でノートブックを開きます。</span><span class="sxs-lookup"><span data-stu-id="fe4f8-118">Opens the notebook in OneNote Online.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="fe4f8-119">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fe4f8-119">JSON representation</span></span>

<span data-ttu-id="fe4f8-120">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="fe4f8-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.recentNotebookLinks"
}-->

```json
{
  "oneNoteClientUrl": {"@odata.type": "microsoft.graph.externalLink"},
  "oneNoteWebUrl": {"@odata.type": "microsoft.graph.externalLink"}
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "recentNotebookLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
