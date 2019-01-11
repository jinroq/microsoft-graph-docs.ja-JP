---
title: recentNotebookLinks リソース型
description: OneNote ノートブックを開くためのリンクです。 このリソース型は、recentNotebook リソース上のプロパティとして存在します。
localization_priority: Normal
ms.openlocfilehash: 846047bd602d19cb4745e0a63f0326aaf7bfb512
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27810585"
---
# <a name="recentnotebooklinks-resource-type"></a><span data-ttu-id="5bb62-104">recentNotebookLinks リソース型</span><span class="sxs-lookup"><span data-stu-id="5bb62-104">recentNotebookLinks resource type</span></span>

<span data-ttu-id="5bb62-105">OneNote ノートブックを開くためのリンクです。</span><span class="sxs-lookup"><span data-stu-id="5bb62-105">Links for opening a OneNote notebook.</span></span> <span data-ttu-id="5bb62-106">このリソース型は、[recentNotebook](recentnotebook.md) リソース上のプロパティとして存在します。</span><span class="sxs-lookup"><span data-stu-id="5bb62-106">This resource type exists as a property on a [recentNotebook](recentnotebook.md) resource.</span></span>

## <a name="properties"></a><span data-ttu-id="5bb62-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5bb62-107">Properties</span></span>
| <span data-ttu-id="5bb62-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5bb62-108">Property</span></span>     | <span data-ttu-id="5bb62-109">種類</span><span class="sxs-lookup"><span data-stu-id="5bb62-109">Type</span></span>   |<span data-ttu-id="5bb62-110">説明</span><span class="sxs-lookup"><span data-stu-id="5bb62-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="5bb62-111">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="5bb62-111">oneNoteClientUrl</span></span>|[<span data-ttu-id="5bb62-112">externalLink</span><span class="sxs-lookup"><span data-stu-id="5bb62-112">externalLink</span></span>](externallink.md)|<span data-ttu-id="5bb62-113">OneNote のネイティブ クライアントでノートブックを開きます (インストールされている場合)。</span><span class="sxs-lookup"><span data-stu-id="5bb62-113">Opens the notebook in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="5bb62-114">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="5bb62-114">oneNoteWebUrl</span></span>|[<span data-ttu-id="5bb62-115">externalLink</span><span class="sxs-lookup"><span data-stu-id="5bb62-115">externalLink</span></span>](externallink.md)|<span data-ttu-id="5bb62-116">OneNote Online でノートブックを開きます。</span><span class="sxs-lookup"><span data-stu-id="5bb62-116">Opens the notebook in OneNote Online.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5bb62-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5bb62-117">JSON representation</span></span>

<span data-ttu-id="5bb62-118">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5bb62-118">The following is a JSON representation of the resource.</span></span>

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
