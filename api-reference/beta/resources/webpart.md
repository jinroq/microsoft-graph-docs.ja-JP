---
author: rahmit
ms.author: rahmit
ms.date: 09/01/2018
title: WebPart
ms.openlocfilehash: e9bb612e20bc3d2416503f571f5abf364215efb2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069476"
---
# <a name="webpart-resource"></a><span data-ttu-id="bbf08-102">web パーツ リソース</span><span class="sxs-lookup"><span data-stu-id="bbf08-102">webPart resource</span></span>

> <span data-ttu-id="bbf08-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="bbf08-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bbf08-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bbf08-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bbf08-105">**Web パーツ**リソースは、型との[sitePage](sitepage.md)上の web パーツのレンダリング情報を表します。</span><span class="sxs-lookup"><span data-stu-id="bbf08-105">The **webPart** resource represents type and rendering information for a web part on a [sitePage](sitepage.md).</span></span>

## <a name="json-representation"></a><span data-ttu-id="bbf08-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="bbf08-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="bbf08-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bbf08-107">Properties</span></span>

| <span data-ttu-id="bbf08-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bbf08-108">Property</span></span>                | <span data-ttu-id="bbf08-109">型</span><span class="sxs-lookup"><span data-stu-id="bbf08-109">Type</span></span>             | <span data-ttu-id="bbf08-110">説明</span><span class="sxs-lookup"><span data-stu-id="bbf08-110">Description</span></span>
|:------------------------|:-----------------|:----------------------------------
| <span data-ttu-id="bbf08-111">**type**</span><span class="sxs-lookup"><span data-stu-id="bbf08-111">**type**</span></span>                | <span data-ttu-id="bbf08-112">String</span><span class="sxs-lookup"><span data-stu-id="bbf08-112">String</span></span>           | <span data-ttu-id="bbf08-113">Web パーツの種類を指定する一意の識別子です。</span><span class="sxs-lookup"><span data-stu-id="bbf08-113">A unique identifier specifying the webPart type.</span></span> <span data-ttu-id="bbf08-114">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="bbf08-114">Read-only.</span></span>
| <span data-ttu-id="bbf08-115">**データ**</span><span class="sxs-lookup"><span data-stu-id="bbf08-115">**data**</span></span>                | <span data-ttu-id="bbf08-116">[sitePageData][]</span><span class="sxs-lookup"><span data-stu-id="bbf08-116">[sitePageData][]</span></span> | <span data-ttu-id="bbf08-117">Web パーツ (web パーツによって異なります) に必要なプロパティ</span><span class="sxs-lookup"><span data-stu-id="bbf08-117">The required properties for the webPart (varies by webPart)</span></span>

[sitePageData]: sitepagedata.md

## <a name="remarks"></a><span data-ttu-id="bbf08-119">解説</span><span class="sxs-lookup"><span data-stu-id="bbf08-119">Remarks</span></span>

<span data-ttu-id="bbf08-120">Web パーツは、[**データ**の独自の必要なプロパティを定義できます。</span><span class="sxs-lookup"><span data-stu-id="bbf08-120">Web parts can define their own required properties under **data**.</span></span>

<span data-ttu-id="bbf08-121">ページの詳細については、 [sitePage](sitepage.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bbf08-121">For more information about pages, see [sitePage](sitepage.md).</span></span>
<!-- {
  "type": "#page.annotation",
  "description": "Defines a control resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Control"
} -->
