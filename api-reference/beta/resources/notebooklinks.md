---
title: notebookLinks リソースの種類
description: OneNote ノートブックを開くためのリンクです。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: resourcePageType
ms.openlocfilehash: 866176f1c831c70b7a057d1a53ad6b5fa7e5cda4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35966651"
---
# <a name="notebooklinks-resource-type"></a><span data-ttu-id="949a2-103">notebookLinks リソースの種類</span><span class="sxs-lookup"><span data-stu-id="949a2-103">notebookLinks resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="949a2-104">OneNote ノートブックを開くためのリンクです。</span><span class="sxs-lookup"><span data-stu-id="949a2-104">Links for opening a OneNote notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="949a2-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="949a2-105">JSON representation</span></span>

<span data-ttu-id="949a2-106">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="949a2-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="949a2-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="949a2-107">Properties</span></span>
| <span data-ttu-id="949a2-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="949a2-108">Property</span></span>     | <span data-ttu-id="949a2-109">型</span><span class="sxs-lookup"><span data-stu-id="949a2-109">Type</span></span>   |<span data-ttu-id="949a2-110">説明</span><span class="sxs-lookup"><span data-stu-id="949a2-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="949a2-111">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="949a2-111">oneNoteClientUrl</span></span>|[<span data-ttu-id="949a2-112">externalLink</span><span class="sxs-lookup"><span data-stu-id="949a2-112">externalLink</span></span>](externallink.md)|<span data-ttu-id="949a2-113">OneNote のネイティブ クライアントでノートブックを開きます (インストールされている場合)。</span><span class="sxs-lookup"><span data-stu-id="949a2-113">Opens the notebook in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="949a2-114">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="949a2-114">oneNoteWebUrl</span></span>|[<span data-ttu-id="949a2-115">externalLink</span><span class="sxs-lookup"><span data-stu-id="949a2-115">externalLink</span></span>](externallink.md)|<span data-ttu-id="949a2-116">OneNote で web 上のノートブックを開きます。</span><span class="sxs-lookup"><span data-stu-id="949a2-116">Opens the notebook in OneNote on the web.</span></span>|

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
