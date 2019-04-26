---
title: sectionlinks リソースの種類
description: OneNote セクションを開くためのリンク。
localization_priority: Normal
ms.openlocfilehash: 2054e2a7a61d6c715146b51fb97c02516d8b638e
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33343424"
---
# <a name="sectionlinks-resource-type"></a><span data-ttu-id="dc172-103">sectionlinks リソースの種類</span><span class="sxs-lookup"><span data-stu-id="dc172-103">sectionLinks resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="dc172-104">OneNote セクションを開くためのリンク。</span><span class="sxs-lookup"><span data-stu-id="dc172-104">Links for opening a OneNote section.</span></span>

## <a name="json-representation"></a><span data-ttu-id="dc172-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="dc172-105">JSON representation</span></span>

<span data-ttu-id="dc172-106">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="dc172-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="dc172-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dc172-107">Properties</span></span>
| <span data-ttu-id="dc172-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dc172-108">Property</span></span>     | <span data-ttu-id="dc172-109">型</span><span class="sxs-lookup"><span data-stu-id="dc172-109">Type</span></span>   |<span data-ttu-id="dc172-110">説明</span><span class="sxs-lookup"><span data-stu-id="dc172-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="dc172-111">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="dc172-111">oneNoteClientUrl</span></span>|[<span data-ttu-id="dc172-112">externalLink</span><span class="sxs-lookup"><span data-stu-id="dc172-112">externalLink</span></span>](externallink.md)|<span data-ttu-id="dc172-113">OneNote native client がインストールされている場合は、そのセクションを開きます。</span><span class="sxs-lookup"><span data-stu-id="dc172-113">Opens the section in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="dc172-114">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="dc172-114">oneNoteWebUrl</span></span>|[<span data-ttu-id="dc172-115">externalLink</span><span class="sxs-lookup"><span data-stu-id="dc172-115">externalLink</span></span>](externallink.md)|<span data-ttu-id="dc172-116">OneNote Online でセクションを開きます。</span><span class="sxs-lookup"><span data-stu-id="dc172-116">Opens the section in OneNote Online.</span></span>|

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
