---
title: sectionLinks リソースの種類
description: OneNote セクションを開くためのリンク。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 270cc08f797546f08dbb89c4137631dd30cc4ae0
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008594"
---
# <a name="sectionlinks-resource-type"></a><span data-ttu-id="de239-103">sectionLinks リソースの種類</span><span class="sxs-lookup"><span data-stu-id="de239-103">sectionLinks resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="de239-104">OneNote セクションを開くためのリンク。</span><span class="sxs-lookup"><span data-stu-id="de239-104">Links for opening a OneNote section.</span></span>

## <a name="json-representation"></a><span data-ttu-id="de239-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="de239-105">JSON representation</span></span>

<span data-ttu-id="de239-106">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="de239-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="de239-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="de239-107">Properties</span></span>
| <span data-ttu-id="de239-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="de239-108">Property</span></span>     | <span data-ttu-id="de239-109">型</span><span class="sxs-lookup"><span data-stu-id="de239-109">Type</span></span>   |<span data-ttu-id="de239-110">説明</span><span class="sxs-lookup"><span data-stu-id="de239-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="de239-111">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="de239-111">oneNoteClientUrl</span></span>|[<span data-ttu-id="de239-112">externalLink</span><span class="sxs-lookup"><span data-stu-id="de239-112">externalLink</span></span>](externallink.md)|<span data-ttu-id="de239-113">OneNote native client がインストールされている場合は、そのセクションを開きます。</span><span class="sxs-lookup"><span data-stu-id="de239-113">Opens the section in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="de239-114">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="de239-114">oneNoteWebUrl</span></span>|[<span data-ttu-id="de239-115">externalLink</span><span class="sxs-lookup"><span data-stu-id="de239-115">externalLink</span></span>](externallink.md)|<span data-ttu-id="de239-116">Web 上の OneNote でセクションを開きます。</span><span class="sxs-lookup"><span data-stu-id="de239-116">Opens the section in OneNote on the web.</span></span>|

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
