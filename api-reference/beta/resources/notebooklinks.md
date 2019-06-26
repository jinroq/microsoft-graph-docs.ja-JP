---
title: notebookLinks リソースの種類
description: OneNote ノートブックを開くためのリンクです。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: 12be75eda0d4f3146332cec0b2eeda09a1d9c5e7
ms.sourcegitcommit: 750c82f161a0f62bc2486995456ccd92ee5c7831
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/26/2019
ms.locfileid: "35236602"
---
# <a name="notebooklinks-resource-type"></a><span data-ttu-id="ba717-103">notebookLinks リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ba717-103">notebookLinks resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ba717-104">OneNote ノートブックを開くためのリンクです。</span><span class="sxs-lookup"><span data-stu-id="ba717-104">Links for opening a OneNote notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ba717-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ba717-105">JSON representation</span></span>

<span data-ttu-id="ba717-106">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ba717-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="ba717-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ba717-107">Properties</span></span>
| <span data-ttu-id="ba717-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ba717-108">Property</span></span>     | <span data-ttu-id="ba717-109">型</span><span class="sxs-lookup"><span data-stu-id="ba717-109">Type</span></span>   |<span data-ttu-id="ba717-110">説明</span><span class="sxs-lookup"><span data-stu-id="ba717-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ba717-111">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="ba717-111">oneNoteClientUrl</span></span>|[<span data-ttu-id="ba717-112">externalLink</span><span class="sxs-lookup"><span data-stu-id="ba717-112">externalLink</span></span>](externallink.md)|<span data-ttu-id="ba717-113">OneNote のネイティブ クライアントでノートブックを開きます (インストールされている場合)。</span><span class="sxs-lookup"><span data-stu-id="ba717-113">Opens the notebook in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="ba717-114">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="ba717-114">oneNoteWebUrl</span></span>|[<span data-ttu-id="ba717-115">externalLink</span><span class="sxs-lookup"><span data-stu-id="ba717-115">externalLink</span></span>](externallink.md)|<span data-ttu-id="ba717-116">OneNote で web 上のノートブックを開きます。</span><span class="sxs-lookup"><span data-stu-id="ba717-116">Opens the notebook in OneNote on the web.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "notebookLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
