---
title: pageLinks リソースの種類
description: OneNote ページを開くためのリンク。
localization_priority: Normal
ms.openlocfilehash: 7dab353d4e936559e26a16e64b58bbf3f4c01232
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/26/2019
ms.locfileid: "35236553"
---
# <a name="pagelinks-resource-type"></a><span data-ttu-id="367f5-103">pageLinks リソースの種類</span><span class="sxs-lookup"><span data-stu-id="367f5-103">pageLinks resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="367f5-104">OneNote ページを開くためのリンク。</span><span class="sxs-lookup"><span data-stu-id="367f5-104">Links for opening a OneNote page.</span></span>

## <a name="json-representation"></a><span data-ttu-id="367f5-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="367f5-105">JSON representation</span></span>

<span data-ttu-id="367f5-106">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="367f5-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="367f5-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="367f5-107">Properties</span></span>
| <span data-ttu-id="367f5-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="367f5-108">Property</span></span>     | <span data-ttu-id="367f5-109">型</span><span class="sxs-lookup"><span data-stu-id="367f5-109">Type</span></span>   |<span data-ttu-id="367f5-110">説明</span><span class="sxs-lookup"><span data-stu-id="367f5-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="367f5-111">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="367f5-111">oneNoteClientUrl</span></span>|[<span data-ttu-id="367f5-112">externalLink</span><span class="sxs-lookup"><span data-stu-id="367f5-112">externalLink</span></span>](externallink.md)|<span data-ttu-id="367f5-113">OneNote native client でページを開きます (インストールされている場合)。</span><span class="sxs-lookup"><span data-stu-id="367f5-113">Opens the page in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="367f5-114">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="367f5-114">oneNoteWebUrl</span></span>|[<span data-ttu-id="367f5-115">externalLink</span><span class="sxs-lookup"><span data-stu-id="367f5-115">externalLink</span></span>](externallink.md)|<span data-ttu-id="367f5-116">Web 上の OneNote でページを開きます。</span><span class="sxs-lookup"><span data-stu-id="367f5-116">Opens the page in OneNote on the web.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "pageLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
