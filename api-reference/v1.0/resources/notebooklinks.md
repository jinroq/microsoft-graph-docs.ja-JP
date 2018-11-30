---
title: notebookLinks リソースの種類
description: OneNote ノートブックを開くためのリンクです。
ms.openlocfilehash: 713779d3bab12222df7a405c1dccb4e6cd4cb235
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27021920"
---
# <a name="notebooklinks-resource-type"></a><span data-ttu-id="20a91-103">notebookLinks リソースの種類</span><span class="sxs-lookup"><span data-stu-id="20a91-103">notebookLinks resource type</span></span>

<span data-ttu-id="20a91-104">OneNote ノートブックを開くためのリンクです。</span><span class="sxs-lookup"><span data-stu-id="20a91-104">Links for opening a OneNote notebook.</span></span>

## <a name="json-representation"></a><span data-ttu-id="20a91-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="20a91-105">JSON representation</span></span>

<span data-ttu-id="20a91-106">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="20a91-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="20a91-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="20a91-107">Properties</span></span>
| <span data-ttu-id="20a91-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="20a91-108">Property</span></span>     | <span data-ttu-id="20a91-109">型</span><span class="sxs-lookup"><span data-stu-id="20a91-109">Type</span></span>   |<span data-ttu-id="20a91-110">説明</span><span class="sxs-lookup"><span data-stu-id="20a91-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="20a91-111">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="20a91-111">oneNoteClientUrl</span></span>|[<span data-ttu-id="20a91-112">externalLink</span><span class="sxs-lookup"><span data-stu-id="20a91-112">externalLink</span></span>](externallink.md)|<span data-ttu-id="20a91-113">OneNote のネイティブ クライアントでノートブックを開きます (インストールされている場合)。</span><span class="sxs-lookup"><span data-stu-id="20a91-113">Opens the notebook in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="20a91-114">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="20a91-114">oneNoteWebUrl</span></span>|[<span data-ttu-id="20a91-115">externalLink</span><span class="sxs-lookup"><span data-stu-id="20a91-115">externalLink</span></span>](externallink.md)|<span data-ttu-id="20a91-116">OneNote Online でノートブックを開きます。</span><span class="sxs-lookup"><span data-stu-id="20a91-116">Opens the notebook in OneNote Online.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "notebookLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->