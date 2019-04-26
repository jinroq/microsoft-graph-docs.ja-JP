---
title: sectionlinks リソースの種類
description: OneNote セクションを開くためのリンク。
localization_priority: Normal
ms.openlocfilehash: a5e2f4800472e8cedc495e6de1c17a6586710e87
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562876"
---
# <a name="sectionlinks-resource-type"></a><span data-ttu-id="3bf02-103">sectionlinks リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3bf02-103">sectionLinks resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3bf02-104">OneNote セクションを開くためのリンク。</span><span class="sxs-lookup"><span data-stu-id="3bf02-104">Links for opening a OneNote section.</span></span>

## <a name="json-representation"></a><span data-ttu-id="3bf02-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3bf02-105">JSON representation</span></span>

<span data-ttu-id="3bf02-106">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="3bf02-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="3bf02-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3bf02-107">Properties</span></span>
| <span data-ttu-id="3bf02-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3bf02-108">Property</span></span>     | <span data-ttu-id="3bf02-109">型</span><span class="sxs-lookup"><span data-stu-id="3bf02-109">Type</span></span>   |<span data-ttu-id="3bf02-110">説明</span><span class="sxs-lookup"><span data-stu-id="3bf02-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3bf02-111">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="3bf02-111">oneNoteClientUrl</span></span>|[<span data-ttu-id="3bf02-112">externalLink</span><span class="sxs-lookup"><span data-stu-id="3bf02-112">externalLink</span></span>](externallink.md)|<span data-ttu-id="3bf02-113">OneNote native client がインストールされている場合は、そのセクションを開きます。</span><span class="sxs-lookup"><span data-stu-id="3bf02-113">Opens the section in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="3bf02-114">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="3bf02-114">oneNoteWebUrl</span></span>|[<span data-ttu-id="3bf02-115">externalLink</span><span class="sxs-lookup"><span data-stu-id="3bf02-115">externalLink</span></span>](externallink.md)|<span data-ttu-id="3bf02-116">OneNote Online でセクションを開きます。</span><span class="sxs-lookup"><span data-stu-id="3bf02-116">Opens the section in OneNote Online.</span></span>|

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
