---
title: sectionLinks リソースの種類
description: OneNote セクションを開くためのリンクです。
localization_priority: Normal
ms.openlocfilehash: 190842708979d62430a4716a8785fd40309cb189
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858941"
---
# <a name="sectionlinks-resource-type"></a><span data-ttu-id="42134-103">sectionLinks リソースの種類</span><span class="sxs-lookup"><span data-stu-id="42134-103">sectionLinks resource type</span></span>

> <span data-ttu-id="42134-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="42134-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="42134-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="42134-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="42134-106">OneNote セクションを開くためのリンクです。</span><span class="sxs-lookup"><span data-stu-id="42134-106">Links for opening a OneNote section.</span></span>

## <a name="json-representation"></a><span data-ttu-id="42134-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="42134-107">JSON representation</span></span>

<span data-ttu-id="42134-108">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="42134-108">Here is a JSON representation of the resource.</span></span>

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
## <a name="properties"></a><span data-ttu-id="42134-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="42134-109">Properties</span></span>
| <span data-ttu-id="42134-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="42134-110">Property</span></span>     | <span data-ttu-id="42134-111">種類</span><span class="sxs-lookup"><span data-stu-id="42134-111">Type</span></span>   |<span data-ttu-id="42134-112">説明</span><span class="sxs-lookup"><span data-stu-id="42134-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="42134-113">oneNoteClientUrl</span><span class="sxs-lookup"><span data-stu-id="42134-113">oneNoteClientUrl</span></span>|[<span data-ttu-id="42134-114">externalLink</span><span class="sxs-lookup"><span data-stu-id="42134-114">externalLink</span></span>](externallink.md)|<span data-ttu-id="42134-115">OneNote のネイティブ クライアントでセクションを開きます (インストールされている場合)。</span><span class="sxs-lookup"><span data-stu-id="42134-115">Opens the section in the OneNote native client if it's installed.</span></span>|
|<span data-ttu-id="42134-116">oneNoteWebUrl</span><span class="sxs-lookup"><span data-stu-id="42134-116">oneNoteWebUrl</span></span>|[<span data-ttu-id="42134-117">externalLink</span><span class="sxs-lookup"><span data-stu-id="42134-117">externalLink</span></span>](externallink.md)|<span data-ttu-id="42134-118">OneNote Online でセクションを開きます。</span><span class="sxs-lookup"><span data-stu-id="42134-118">Opens the section in OneNote Online.</span></span>|

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "sectionLinks resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
