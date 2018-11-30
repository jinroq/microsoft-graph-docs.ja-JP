---
title: recentNotebookLinks リソース型
description: OneNote ノートブックを開くためのリンクです。 このリソース型は、recentNotebook リソース上のプロパティとして存在します。
ms.openlocfilehash: 594616a790becd77086177157f71321ffdd36e24
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27021218"
---
# <a name="recentnotebooklinks-resource-type"></a><span data-ttu-id="4b946-104">recentNotebookLinks リソース型</span><span class="sxs-lookup"><span data-stu-id="4b946-104">recentNotebookLinks resource type</span></span>

<span data-ttu-id="4b946-105">OneNote ノートブックを開くためのリンクです。</span><span class="sxs-lookup"><span data-stu-id="4b946-105">Links for opening a OneNote notebook.</span></span> <span data-ttu-id="4b946-106">このリソース型は、[recentNotebook](recentnotebook.md) リソース上のプロパティとして存在します。</span><span class="sxs-lookup"><span data-stu-id="4b946-106">This resource type exists as a property on a [recentNotebook](recentnotebook.md) resource.</span></span>

## <a name="properties"></a><span data-ttu-id="4b946-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4b946-107">Properties</span></span>
| <span data-ttu-id="4b946-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4b946-108">Property</span></span>     | <span data-ttu-id="4b946-109">型</span><span class="sxs-lookup"><span data-stu-id="4b946-109">Type</span></span>   |<span data-ttu-id="4b946-110">説明</span><span class="sxs-lookup"><span data-stu-id="4b946-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4b946-111">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="4b946-111">oneNoteClientUrl</span></span>|[<span data-ttu-id="4b946-112">externalLink</span><span class="sxs-lookup"><span data-stu-id="4b946-112">externalLink</span></span>](externallink.md)|<span data-ttu-id="4b946-113">OneNote のネイティブ クライアントでノートブックを開きます (インストールされている場合)。</span><span class="sxs-lookup"><span data-stu-id="4b946-113">Opens the notebook in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="4b946-114">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="4b946-114">oneNoteWebUrl</span></span>|[<span data-ttu-id="4b946-115">externalLink</span><span class="sxs-lookup"><span data-stu-id="4b946-115">externalLink</span></span>](externallink.md)|<span data-ttu-id="4b946-116">OneNote Online でノートブックを開きます。</span><span class="sxs-lookup"><span data-stu-id="4b946-116">Opens the notebook in OneNote Online.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4b946-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4b946-117">JSON representation</span></span>

<span data-ttu-id="4b946-118">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4b946-118">The following is a JSON representation of the resource.</span></span>

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
