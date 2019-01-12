---
author: rahmit
ms.author: rahmit
ms.date: 09/01/2018
title: WebPart
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 9147d434a94380c4d178efdf80ccba90734bf96f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27939043"
---
# <a name="webpart-resource"></a><span data-ttu-id="fe52d-102">web パーツ リソース</span><span class="sxs-lookup"><span data-stu-id="fe52d-102">webPart resource</span></span>

> <span data-ttu-id="fe52d-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="fe52d-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fe52d-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fe52d-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fe52d-105">**Web パーツ**リソースは、型との[sitePage](sitepage.md)上の web パーツのレンダリング情報を表します。</span><span class="sxs-lookup"><span data-stu-id="fe52d-105">The **webPart** resource represents type and rendering information for a web part on a [sitePage](sitepage.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="fe52d-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fe52d-106">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.webPart"
}-->

```json
{
  "type": "string (guid)",
  "data": {
    "instanceId": "string (guid) (optional)"
  }
}
```

## <a name="properties"></a><span data-ttu-id="fe52d-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fe52d-107">Properties</span></span>

| <span data-ttu-id="fe52d-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fe52d-108">Property</span></span>                | <span data-ttu-id="fe52d-109">種類</span><span class="sxs-lookup"><span data-stu-id="fe52d-109">Type</span></span>             | <span data-ttu-id="fe52d-110">説明</span><span class="sxs-lookup"><span data-stu-id="fe52d-110">Description</span></span>
|:------------------------|:-----------------|:----------------------------------
| <span data-ttu-id="fe52d-111">**type**</span><span class="sxs-lookup"><span data-stu-id="fe52d-111">**type**</span></span>                | <span data-ttu-id="fe52d-112">String</span><span class="sxs-lookup"><span data-stu-id="fe52d-112">String</span></span>           | <span data-ttu-id="fe52d-113">Web パーツの種類を指定する一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="fe52d-113">A unique identifier specifying the webPart type.</span></span> <span data-ttu-id="fe52d-114">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="fe52d-114">Read-only.</span></span>
| <span data-ttu-id="fe52d-115">**data**</span><span class="sxs-lookup"><span data-stu-id="fe52d-115">**data**</span></span>                | <span data-ttu-id="fe52d-116">[sitePageData][]</span><span class="sxs-lookup"><span data-stu-id="fe52d-116">[sitePageData][]</span></span> | <span data-ttu-id="fe52d-117">Web パーツ (web パーツによって異なります) に必要なプロパティ</span><span class="sxs-lookup"><span data-stu-id="fe52d-117">The required properties for the webPart (varies by webPart)</span></span>

[sitePageData]: sitepagedata.md

## <a name="remarks"></a><span data-ttu-id="fe52d-119">解説</span><span class="sxs-lookup"><span data-stu-id="fe52d-119">Remarks</span></span>

<span data-ttu-id="fe52d-120">Web パーツは、[**データ**の独自の必要なプロパティを定義できます。</span><span class="sxs-lookup"><span data-stu-id="fe52d-120">Web parts can define their own required properties under **data**.</span></span>

<span data-ttu-id="fe52d-121">ページの詳細については、 [sitePage](sitepage.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fe52d-121">For more information about pages, see [sitePage](sitepage.md).</span></span>
<!-- {
  "type": "#page.annotation",
  "description": "Defines a control resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Control"
} -->
