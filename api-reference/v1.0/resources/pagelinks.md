---
title: pageLinks リソースの種類
description: OneNote ページを開くためのリンク。
localization_priority: Normal
ms.openlocfilehash: a5950366f6c6079443338b68db258c5762c15a7a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32462509"
---
# <a name="pagelinks-resource-type"></a><span data-ttu-id="43cf2-103">pageLinks リソースの種類</span><span class="sxs-lookup"><span data-stu-id="43cf2-103">pageLinks resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="43cf2-104">OneNote ページを開くためのリンク。</span><span class="sxs-lookup"><span data-stu-id="43cf2-104">Links for opening a OneNote page.</span></span>

## <a name="json-representation"></a><span data-ttu-id="43cf2-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="43cf2-105">JSON representation</span></span>

<span data-ttu-id="43cf2-106">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="43cf2-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="43cf2-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="43cf2-107">Properties</span></span>
| <span data-ttu-id="43cf2-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="43cf2-108">Property</span></span>     | <span data-ttu-id="43cf2-109">型</span><span class="sxs-lookup"><span data-stu-id="43cf2-109">Type</span></span>   |<span data-ttu-id="43cf2-110">説明</span><span class="sxs-lookup"><span data-stu-id="43cf2-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="43cf2-111">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="43cf2-111">oneNoteClientUrl</span></span>|[<span data-ttu-id="43cf2-112">externalLink</span><span class="sxs-lookup"><span data-stu-id="43cf2-112">externalLink</span></span>](externallink.md)|<span data-ttu-id="43cf2-113">OneNote native client でページを開きます (インストールされている場合)。</span><span class="sxs-lookup"><span data-stu-id="43cf2-113">Opens the page in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="43cf2-114">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="43cf2-114">oneNoteWebUrl</span></span>|[<span data-ttu-id="43cf2-115">externalLink</span><span class="sxs-lookup"><span data-stu-id="43cf2-115">externalLink</span></span>](externallink.md)|<span data-ttu-id="43cf2-116">OneNote Online でページを開きます。</span><span class="sxs-lookup"><span data-stu-id="43cf2-116">Opens the page in OneNote Online.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "pageLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/pagelinks.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
