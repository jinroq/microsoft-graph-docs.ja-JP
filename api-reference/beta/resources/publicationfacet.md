---
author: JeremyKelley
description: publicationFacet リソースは、driveItemVersion または driveItem リソースの公開ステータスの詳細情報を提供します。
ms.date: 09/10/2017
title: PublicationFacet
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
ms.openlocfilehash: 9c09f0863376e1569fb4af0acc0044fa1c7c8cfa
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36008860"
---
# <a name="publicationfacet-resource-type"></a><span data-ttu-id="64e33-103">PublicationFacet リソースの種類</span><span class="sxs-lookup"><span data-stu-id="64e33-103">PublicationFacet resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="64e33-104">\*\*publicationFacet \*\*リソースは、[driveItemVersion](driveitemversion.md) または [driveItem](driveitem.md) リソースの公開ステータスの詳細情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="64e33-104">The **publicationFacet** resource provides details on the published status of a [driveItemVersion](driveitemversion.md) or [driveItem](driveitem.md) resource.</span></span>

## <a name="json-representation"></a><span data-ttu-id="64e33-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="64e33-105">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="64e33-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="64e33-106">Properties</span></span>

|   <span data-ttu-id="64e33-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="64e33-107">Property</span></span>    |  <span data-ttu-id="64e33-108">型</span><span class="sxs-lookup"><span data-stu-id="64e33-108">Type</span></span>  | <span data-ttu-id="64e33-109">説明</span><span class="sxs-lookup"><span data-stu-id="64e33-109">Description</span></span> |
| :------------ | :----- | :---------- |
| <span data-ttu-id="64e33-110">**level**</span><span class="sxs-lookup"><span data-stu-id="64e33-110">**level**</span></span>     | <span data-ttu-id="64e33-111">String</span><span class="sxs-lookup"><span data-stu-id="64e33-111">String</span></span> | <span data-ttu-id="64e33-112">このドキュメントの公開状況。</span><span class="sxs-lookup"><span data-stu-id="64e33-112">The state of publication for this document.</span></span> <span data-ttu-id="64e33-113">`published` または `checkout` のどちらかです。</span><span class="sxs-lookup"><span data-stu-id="64e33-113">Either `published` or `checkout`.</span></span> <span data-ttu-id="64e33-114">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="64e33-114">Read-only.</span></span>  |
| <span data-ttu-id="64e33-115">**versionId**</span><span class="sxs-lookup"><span data-stu-id="64e33-115">**versionId**</span></span> | <span data-ttu-id="64e33-116">String</span><span class="sxs-lookup"><span data-stu-id="64e33-116">String</span></span> | <span data-ttu-id="64e33-117">現在の呼び出し元に表示されているバージョンの一意識別子です。</span><span class="sxs-lookup"><span data-stu-id="64e33-117">The unique identifier for the version that is visible to the current caller.</span></span> <span data-ttu-id="64e33-118">値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="64e33-118">Read-only.</span></span>  |


<!--
{
  "type": "#page.annotation",
  "description": "The photo facet provides details about the camera and settings on the camera for photos.",
  "keywords": "camera make,camera model, exposure, f-stop, iso",
  "section": "documentation",
  "tocPath": "Facets/Photo",
  "suppressions": []
}
-->
