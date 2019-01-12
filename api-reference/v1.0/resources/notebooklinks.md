---
title: notebookLinks リソースの種類
description: OneNote ノートブックを開くためのリンクです。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
ms.openlocfilehash: d3def81fb9bb3b7f657be3ed04230a65235db5f3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27984256"
---
# <a name="notebooklinks-resource-type"></a><span data-ttu-id="a131e-103">notebookLinks リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a131e-103">notebookLinks resource type</span></span>

<span data-ttu-id="a131e-104">OneNote ノートブックを開くためのリンクです。</span><span class="sxs-lookup"><span data-stu-id="a131e-104">Links for opening a OneNote notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="a131e-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a131e-105">JSON representation</span></span>

<span data-ttu-id="a131e-106">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a131e-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="a131e-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a131e-107">Properties</span></span>
| <span data-ttu-id="a131e-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a131e-108">Property</span></span>     | <span data-ttu-id="a131e-109">種類</span><span class="sxs-lookup"><span data-stu-id="a131e-109">Type</span></span>   |<span data-ttu-id="a131e-110">説明</span><span class="sxs-lookup"><span data-stu-id="a131e-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a131e-111">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="a131e-111">oneNoteClientUrl</span></span>|[<span data-ttu-id="a131e-112">externalLink</span><span class="sxs-lookup"><span data-stu-id="a131e-112">externalLink</span></span>](externallink.md)|<span data-ttu-id="a131e-113">OneNote のネイティブ クライアントでノートブックを開きます (インストールされている場合)。</span><span class="sxs-lookup"><span data-stu-id="a131e-113">Opens the notebook in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="a131e-114">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="a131e-114">oneNoteWebUrl</span></span>|[<span data-ttu-id="a131e-115">externalLink</span><span class="sxs-lookup"><span data-stu-id="a131e-115">externalLink</span></span>](externallink.md)|<span data-ttu-id="a131e-116">OneNote Online でノートブックを開きます。</span><span class="sxs-lookup"><span data-stu-id="a131e-116">Opens the notebook in OneNote Online.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "notebookLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
