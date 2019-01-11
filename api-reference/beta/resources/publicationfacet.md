---
author: rgregg
ms.author: rgregg
ms.date: 09/10/2017
title: PublicationFacet
localization_priority: Normal
ms.openlocfilehash: 4cb3a56b5bdb4c3e7c9fc9fe69c0b34cae134a0d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27805608"
---
# <a name="publicationfacet-resource-type"></a><span data-ttu-id="6ec73-102">PublicationFacet リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6ec73-102">PublicationFacet resource type</span></span>

> <span data-ttu-id="6ec73-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6ec73-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6ec73-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6ec73-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6ec73-105">\*\*publicationFacet \*\*リソースは、[driveItemVersion](driveitemversion.md) または [driveItem](driveitem.md) リソースの公開ステータスの詳細情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="6ec73-105">The **publicationFacet** resource provides details on the published status of a [driveItemVersion](driveitemversion.md) or [driveItem](driveitem.md) resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="6ec73-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6ec73-106">JSON representation</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [  ],
  "@odata.type": "microsoft.graph.publicationFacet"
}-->

```json
{
  "level": "published | checkout",
  "versionId": "string"
}
```

## <a name="properties"></a><span data-ttu-id="6ec73-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6ec73-107">Properties</span></span>

|   <span data-ttu-id="6ec73-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6ec73-108">Property</span></span>    |  <span data-ttu-id="6ec73-109">種類</span><span class="sxs-lookup"><span data-stu-id="6ec73-109">Type</span></span>  | <span data-ttu-id="6ec73-110">説明</span><span class="sxs-lookup"><span data-stu-id="6ec73-110">Description</span></span> |
| :------------ | :----- | :---------- |
| <span data-ttu-id="6ec73-111">**level**</span><span class="sxs-lookup"><span data-stu-id="6ec73-111">**level**</span></span>     | <span data-ttu-id="6ec73-112">String</span><span class="sxs-lookup"><span data-stu-id="6ec73-112">String</span></span> | <span data-ttu-id="6ec73-113">このドキュメントの公開状況。</span><span class="sxs-lookup"><span data-stu-id="6ec73-113">The state of publication for this document.</span></span> <span data-ttu-id="6ec73-114">`published` または `checkout` のどちらかです。</span><span class="sxs-lookup"><span data-stu-id="6ec73-114">Either `published` or `checkout`.</span></span> <span data-ttu-id="6ec73-115">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="6ec73-115">Read-only.</span></span>  |
| <span data-ttu-id="6ec73-116">**versionId**</span><span class="sxs-lookup"><span data-stu-id="6ec73-116">**versionId**</span></span> | <span data-ttu-id="6ec73-117">String</span><span class="sxs-lookup"><span data-stu-id="6ec73-117">String</span></span> | <span data-ttu-id="6ec73-118">現在の呼び出し元に表示されているバージョンの一意識別子です。</span><span class="sxs-lookup"><span data-stu-id="6ec73-118">The unique identifier for the version that is visible to the current caller.</span></span> <span data-ttu-id="6ec73-119">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="6ec73-119">Read-only.</span></span>  |


<!-- {
  "type": "#page.annotation",
  "description": "The photo facet provides details about the camera and settings on the camera for photos.",
  "keywords": "camera make,camera model, exposure, f-stop, iso",
  "section": "documentation",
  "tocPath": "Facets/Photo"
} -->
