---
title: pageLinks リソースの種類
description: OneNote のページを開くためのリンクです。
ms.openlocfilehash: f1e4fe36d4356986bc88b744a9a62e28b8d368c5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020769"
---
# <a name="pagelinks-resource-type"></a><span data-ttu-id="16b04-103">pageLinks リソースの種類</span><span class="sxs-lookup"><span data-stu-id="16b04-103">pageLinks resource type</span></span>

<span data-ttu-id="16b04-104">OneNote のページを開くためのリンクです。</span><span class="sxs-lookup"><span data-stu-id="16b04-104">Links for opening a OneNote page.</span></span>

## <a name="json-representation"></a><span data-ttu-id="16b04-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="16b04-105">JSON representation</span></span>

<span data-ttu-id="16b04-106">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="16b04-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="16b04-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="16b04-107">Properties</span></span>
| <span data-ttu-id="16b04-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="16b04-108">Property</span></span>     | <span data-ttu-id="16b04-109">型</span><span class="sxs-lookup"><span data-stu-id="16b04-109">Type</span></span>   |<span data-ttu-id="16b04-110">説明</span><span class="sxs-lookup"><span data-stu-id="16b04-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="16b04-111">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="16b04-111">oneNoteClientUrl</span></span>|[<span data-ttu-id="16b04-112">externalLink</span><span class="sxs-lookup"><span data-stu-id="16b04-112">externalLink</span></span>](externallink.md)|<span data-ttu-id="16b04-113">OneNote のネイティブ クライアントでページを開きます (インストールされている場合)。</span><span class="sxs-lookup"><span data-stu-id="16b04-113">Opens the page in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="16b04-114">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="16b04-114">oneNoteWebUrl</span></span>|[<span data-ttu-id="16b04-115">externalLink</span><span class="sxs-lookup"><span data-stu-id="16b04-115">externalLink</span></span>](externallink.md)|<span data-ttu-id="16b04-116">OneNote Online でページを開きます。</span><span class="sxs-lookup"><span data-stu-id="16b04-116">Opens the page in OneNote Online.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "pageLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->