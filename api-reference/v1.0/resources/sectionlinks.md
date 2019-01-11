---
title: sectionLinks リソースの種類
description: OneNote セクションを開くためのリンクです。
localization_priority: Normal
ms.openlocfilehash: afc740aebc494aa6f204febbce1be4433005a4b1
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27839936"
---
# <a name="sectionlinks-resource-type"></a><span data-ttu-id="59111-103">sectionLinks リソースの種類</span><span class="sxs-lookup"><span data-stu-id="59111-103">sectionLinks resource type</span></span>

<span data-ttu-id="59111-104">OneNote セクションを開くためのリンクです。</span><span class="sxs-lookup"><span data-stu-id="59111-104">Links for opening a OneNote section.</span></span>

## <a name="json-representation"></a><span data-ttu-id="59111-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="59111-105">JSON representation</span></span>

<span data-ttu-id="59111-106">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="59111-106">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="59111-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="59111-107">Properties</span></span>
| <span data-ttu-id="59111-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="59111-108">Property</span></span>     | <span data-ttu-id="59111-109">種類</span><span class="sxs-lookup"><span data-stu-id="59111-109">Type</span></span>   |<span data-ttu-id="59111-110">説明</span><span class="sxs-lookup"><span data-stu-id="59111-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="59111-111">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="59111-111">oneNoteClientUrl</span></span>|[<span data-ttu-id="59111-112">externalLink</span><span class="sxs-lookup"><span data-stu-id="59111-112">externalLink</span></span>](externallink.md)|<span data-ttu-id="59111-113">OneNote のネイティブ クライアントでセクションを開きます (インストールされている場合)。</span><span class="sxs-lookup"><span data-stu-id="59111-113">Opens the section in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="59111-114">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="59111-114">oneNoteWebUrl</span></span>|[<span data-ttu-id="59111-115">externalLink</span><span class="sxs-lookup"><span data-stu-id="59111-115">externalLink</span></span>](externallink.md)|<span data-ttu-id="59111-116">OneNote Online でセクションを開きます。</span><span class="sxs-lookup"><span data-stu-id="59111-116">Opens the section in OneNote Online.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "sectionLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
