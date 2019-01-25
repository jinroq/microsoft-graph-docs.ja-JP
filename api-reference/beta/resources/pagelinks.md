---
title: pageLinks リソースの種類
description: OneNote のページを開くためのリンクです。
localization_priority: Normal
ms.openlocfilehash: 07c89d99b5731eccd57bec79c25d7d97509c54a0
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523828"
---
# <a name="pagelinks-resource-type"></a><span data-ttu-id="0751d-103">pageLinks リソースの種類</span><span class="sxs-lookup"><span data-stu-id="0751d-103">pageLinks resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0751d-104">OneNote のページを開くためのリンクです。</span><span class="sxs-lookup"><span data-stu-id="0751d-104">Links for opening a OneNote page.</span></span>

## <a name="json-representation"></a><span data-ttu-id="0751d-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0751d-105">JSON representation</span></span>

<span data-ttu-id="0751d-106">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0751d-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="0751d-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0751d-107">Properties</span></span>
| <span data-ttu-id="0751d-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0751d-108">Property</span></span>     | <span data-ttu-id="0751d-109">型</span><span class="sxs-lookup"><span data-stu-id="0751d-109">Type</span></span>   |<span data-ttu-id="0751d-110">説明</span><span class="sxs-lookup"><span data-stu-id="0751d-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0751d-111">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="0751d-111">oneNoteClientUrl</span></span>|[<span data-ttu-id="0751d-112">externalLink</span><span class="sxs-lookup"><span data-stu-id="0751d-112">externalLink</span></span>](externallink.md)|<span data-ttu-id="0751d-113">OneNote のネイティブ クライアントでページを開きます (インストールされている場合)。</span><span class="sxs-lookup"><span data-stu-id="0751d-113">Opens the page in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="0751d-114">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="0751d-114">oneNoteWebUrl</span></span>|[<span data-ttu-id="0751d-115">externalLink</span><span class="sxs-lookup"><span data-stu-id="0751d-115">externalLink</span></span>](externallink.md)|<span data-ttu-id="0751d-116">OneNote Online でページを開きます。</span><span class="sxs-lookup"><span data-stu-id="0751d-116">Opens the page in OneNote Online.</span></span>|

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
