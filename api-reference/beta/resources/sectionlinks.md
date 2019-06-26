---
title: sectionLinks リソースの種類
description: OneNote セクションを開くためのリンク。
localization_priority: Normal
ms.openlocfilehash: 2c3744e08c492a8857600dc9e51dc205ae387bad
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/26/2019
ms.locfileid: "35236511"
---
# <a name="sectionlinks-resource-type"></a><span data-ttu-id="3e6f7-103">sectionLinks リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3e6f7-103">sectionLinks resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3e6f7-104">OneNote セクションを開くためのリンク。</span><span class="sxs-lookup"><span data-stu-id="3e6f7-104">Links for opening a OneNote section.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3e6f7-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3e6f7-105">JSON representation</span></span>

<span data-ttu-id="3e6f7-106">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="3e6f7-106">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.sectionLinks"
}-->

```json
{
  "oneNoteClientUrl": {"@odata.type": "microsoft.graph.externalLink"},
  "oneNoteWebUrl": {"@odata.type": "microsoft.graph.externalLink"}
}

```
## <a name="properties"></a><span data-ttu-id="3e6f7-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3e6f7-107">Properties</span></span>
| <span data-ttu-id="3e6f7-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3e6f7-108">Property</span></span>     | <span data-ttu-id="3e6f7-109">型</span><span class="sxs-lookup"><span data-stu-id="3e6f7-109">Type</span></span>   |<span data-ttu-id="3e6f7-110">説明</span><span class="sxs-lookup"><span data-stu-id="3e6f7-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3e6f7-111">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="3e6f7-111">oneNoteClientUrl</span></span>|[<span data-ttu-id="3e6f7-112">externalLink</span><span class="sxs-lookup"><span data-stu-id="3e6f7-112">externalLink</span></span>](externallink.md)|<span data-ttu-id="3e6f7-113">OneNote native client がインストールされている場合は、そのセクションを開きます。</span><span class="sxs-lookup"><span data-stu-id="3e6f7-113">Opens the section in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="3e6f7-114">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="3e6f7-114">oneNoteWebUrl</span></span>|[<span data-ttu-id="3e6f7-115">externalLink</span><span class="sxs-lookup"><span data-stu-id="3e6f7-115">externalLink</span></span>](externallink.md)|<span data-ttu-id="3e6f7-116">Web 上の OneNote でセクションを開きます。</span><span class="sxs-lookup"><span data-stu-id="3e6f7-116">Opens the section in OneNote on the web.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "sectionLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
