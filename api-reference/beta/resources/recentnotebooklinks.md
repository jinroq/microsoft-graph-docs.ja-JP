---
title: recentNotebookLinks リソース型
description: OneNote ノートブックを開くためのリンク。 このリソース型は、recentNotebook リソース上のプロパティとして存在します。
localization_priority: Normal
ms.openlocfilehash: c25ee3bc1e5096f7bbdf046090f8db9c0cc623fd
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343942"
---
# <a name="recentnotebooklinks-resource-type"></a><span data-ttu-id="aed8c-104">recentNotebookLinks リソース型</span><span class="sxs-lookup"><span data-stu-id="aed8c-104">recentNotebookLinks resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="aed8c-105">OneNote ノートブックを開くためのリンク。</span><span class="sxs-lookup"><span data-stu-id="aed8c-105">Links to open a OneNote notebook.</span></span> <span data-ttu-id="aed8c-106">このリソース型は、[recentNotebook](recentnotebook.md) リソース上のプロパティとして存在します。</span><span class="sxs-lookup"><span data-stu-id="aed8c-106">This resource type exists as a property on a [recentNotebook](recentnotebook.md) resource.</span></span>

## <a name="properties"></a><span data-ttu-id="aed8c-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aed8c-107">Properties</span></span>
| <span data-ttu-id="aed8c-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="aed8c-108">Property</span></span>     | <span data-ttu-id="aed8c-109">型</span><span class="sxs-lookup"><span data-stu-id="aed8c-109">Type</span></span>   |<span data-ttu-id="aed8c-110">説明</span><span class="sxs-lookup"><span data-stu-id="aed8c-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="aed8c-111">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="aed8c-111">oneNoteClientUrl</span></span>|[<span data-ttu-id="aed8c-112">externalLink</span><span class="sxs-lookup"><span data-stu-id="aed8c-112">externalLink</span></span>](externallink.md)|<span data-ttu-id="aed8c-113">OneNote クライアントでノートブックを開きます (インストールされている場合)。</span><span class="sxs-lookup"><span data-stu-id="aed8c-113">Opens the notebook in the OneNote client, if it's installed.</span></span>|
|<span data-ttu-id="aed8c-114">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="aed8c-114">oneNoteWebUrl</span></span>|[<span data-ttu-id="aed8c-115">externalLink</span><span class="sxs-lookup"><span data-stu-id="aed8c-115">externalLink</span></span>](externallink.md)|<span data-ttu-id="aed8c-116">OneNote Online でノートブックを開きます。</span><span class="sxs-lookup"><span data-stu-id="aed8c-116">Opens the notebook in OneNote Online.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="aed8c-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="aed8c-117">JSON representation</span></span>

<span data-ttu-id="aed8c-118">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="aed8c-118">The following is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "recentNotebookLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
