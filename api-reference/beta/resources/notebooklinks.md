---
title: notebookLinks リソースの種類
description: OneNote ノートブックを開くためのリンクです。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: f6995c112410d22cfe5849f54d0077bf8b79f6b3
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29517366"
---
# <a name="notebooklinks-resource-type"></a><span data-ttu-id="f5af5-103">notebookLinks リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f5af5-103">notebookLinks resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f5af5-104">OneNote ノートブックを開くためのリンクです。</span><span class="sxs-lookup"><span data-stu-id="f5af5-104">Links for opening a OneNote notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="f5af5-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f5af5-105">JSON representation</span></span>

<span data-ttu-id="f5af5-106">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f5af5-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="f5af5-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f5af5-107">Properties</span></span>
| <span data-ttu-id="f5af5-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f5af5-108">Property</span></span>     | <span data-ttu-id="f5af5-109">型</span><span class="sxs-lookup"><span data-stu-id="f5af5-109">Type</span></span>   |<span data-ttu-id="f5af5-110">説明</span><span class="sxs-lookup"><span data-stu-id="f5af5-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f5af5-111">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="f5af5-111">oneNoteClientUrl</span></span>|[<span data-ttu-id="f5af5-112">externalLink</span><span class="sxs-lookup"><span data-stu-id="f5af5-112">externalLink</span></span>](externallink.md)|<span data-ttu-id="f5af5-113">OneNote のネイティブ クライアントでノートブックを開きます (インストールされている場合)。</span><span class="sxs-lookup"><span data-stu-id="f5af5-113">Opens the notebook in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="f5af5-114">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="f5af5-114">oneNoteWebUrl</span></span>|[<span data-ttu-id="f5af5-115">externalLink</span><span class="sxs-lookup"><span data-stu-id="f5af5-115">externalLink</span></span>](externallink.md)|<span data-ttu-id="f5af5-116">OneNote Online でノートブックを開きます。</span><span class="sxs-lookup"><span data-stu-id="f5af5-116">Opens the notebook in OneNote Online.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "notebookLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/notebooklinks.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
