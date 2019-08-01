---
title: DriveItemVersion リソースの種類
description: '**Drive Itemversion**リソースは、ドライブ項目の特定のバージョンを表します。'
localization_priority: Normal
ms.prod: sharepoint
author: ''
doc_type: resourcePageType
ms.openlocfilehash: e9521eb549bf84b900e6c49c4dedc5f2199de317
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029401"
---
# <a name="driveitemversion-resource-type"></a><span data-ttu-id="8d9b1-103">DriveItemVersion リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8d9b1-103">DriveItemVersion resource type</span></span>

<span data-ttu-id="8d9b1-104">**DriveItemVersion** リソースは、[DriveItem](driveitem.md) の特定のバージョンを表しています。</span><span class="sxs-lookup"><span data-stu-id="8d9b1-104">The **DriveItemVersion** resource represents a specific version of a [DriveItem](driveitem.md).</span></span>


## <a name="tasks-on-driveitemversion-resources"></a><span data-ttu-id="8d9b1-105">DriveItemVersion リソースのタスク</span><span class="sxs-lookup"><span data-stu-id="8d9b1-105">Tasks on DriveItemVersion resources</span></span>

<span data-ttu-id="8d9b1-106">driveItemVersion リソースで使用可能なタスクを次に示します。</span><span class="sxs-lookup"><span data-stu-id="8d9b1-106">The following tasks are available for driveItemVersion resources.</span></span>

|            <span data-ttu-id="8d9b1-107">共通タスク</span><span class="sxs-lookup"><span data-stu-id="8d9b1-107">Common task</span></span>             |         <span data-ttu-id="8d9b1-108">HTTP メソッド</span><span class="sxs-lookup"><span data-stu-id="8d9b1-108">HTTP method</span></span>         |
| :--------------------------------- | :-------------------------- |
| <span data-ttu-id="8d9b1-109">[バージョンを一覧表示する][version-list]</span><span class="sxs-lookup"><span data-stu-id="8d9b1-109">[List versions][version-list]</span></span>      | `GET /drive/items/{item-id}/versions`  |
| <span data-ttu-id="8d9b1-110">[バージョンの取得][version-get]</span><span class="sxs-lookup"><span data-stu-id="8d9b1-110">[Get version][version-get]</span></span>         | `GET /drive/items/{item-id}/versions/{version-id}`     |
| <span data-ttu-id="8d9b1-111">[コンテンツの取得][content-get]</span><span class="sxs-lookup"><span data-stu-id="8d9b1-111">[Get contents][content-get]</span></span>        | `GET /drive/items/{item-id}/versions/{version-id}/content` |
| <span data-ttu-id="8d9b1-112">[バージョンの復元][version-restore]</span><span class="sxs-lookup"><span data-stu-id="8d9b1-112">[Restore version][version-restore]</span></span> | `POST /drive/items/{item-id}/versions/{version-id}/restoreversion` |

[version-list]: ../api/driveitem-list-versions.md
[version-get]: ../api/driveitemversion-get.md
[content-get]: ../api/driveitemversion-get-contents.md
[version-restore]: ../api/driveitemversion-restore.md

<span data-ttu-id="8d9b1-113">前の表では、例に `/drive` を使用していますが、他にも有効な要求が多数あります。</span><span class="sxs-lookup"><span data-stu-id="8d9b1-113">In the previous table, the examples use `/drive`, but there are many valid requests.</span></span>

## <a name="json-representation"></a><span data-ttu-id="8d9b1-114">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8d9b1-114">JSON representation</span></span>

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.baseItemVersion",
  "@odata.type": "microsoft.graph.driveItemVersion",
  "@type.aka": "oneDrive.driveItemVersion"
}-->

```json
{
  "content": { "@odata.type": "Edm.Stream" },
  "id": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "2016-01-01T15:20:01.125Z",
  "publication": { "@odata.type": "microsoft.graph.publicationFacet" },
  "size": 12356
}
```

## <a name="properties"></a><span data-ttu-id="8d9b1-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8d9b1-115">Properties</span></span>

|      <span data-ttu-id="8d9b1-116">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="8d9b1-116">Property name</span></span>       |                         <span data-ttu-id="8d9b1-117">種類</span><span class="sxs-lookup"><span data-stu-id="8d9b1-117">Type</span></span>                         |                               <span data-ttu-id="8d9b1-118">説明</span><span class="sxs-lookup"><span data-stu-id="8d9b1-118">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="8d9b1-119">**id**</span><span class="sxs-lookup"><span data-stu-id="8d9b1-119">**id**</span></span>                   | <span data-ttu-id="8d9b1-120">string</span><span class="sxs-lookup"><span data-stu-id="8d9b1-120">string</span></span>                                               | <span data-ttu-id="8d9b1-121">バージョンの ID。</span><span class="sxs-lookup"><span data-stu-id="8d9b1-121">The ID of the version.</span></span> <span data-ttu-id="8d9b1-122">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="8d9b1-122">Read-only.</span></span>                                       |
| <span data-ttu-id="8d9b1-123">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="8d9b1-123">**lastModifiedBy**</span></span>       | [<span data-ttu-id="8d9b1-124">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="8d9b1-124">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="8d9b1-125">最後にバージョンを変更したユーザーの ID。</span><span class="sxs-lookup"><span data-stu-id="8d9b1-125">Identity of the user which last modified the version.</span></span> <span data-ttu-id="8d9b1-126">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="8d9b1-126">Read-only.</span></span>        |
| <span data-ttu-id="8d9b1-127">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="8d9b1-127">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="8d9b1-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8d9b1-128">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="8d9b1-129">バージョンが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="8d9b1-129">Date and time the version was last modified.</span></span> <span data-ttu-id="8d9b1-130">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="8d9b1-130">Read-only.</span></span>                 |
| <span data-ttu-id="8d9b1-131">**publication**</span><span class="sxs-lookup"><span data-stu-id="8d9b1-131">**publication**</span></span>          | [<span data-ttu-id="8d9b1-132">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="8d9b1-132">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="8d9b1-133">特定のバージョンのパブリケーション ステータスを示します。</span><span class="sxs-lookup"><span data-stu-id="8d9b1-133">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="8d9b1-134">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="8d9b1-134">Read-only.</span></span> |
| <span data-ttu-id="8d9b1-135">**size**</span><span class="sxs-lookup"><span data-stu-id="8d9b1-135">**size**</span></span>                 | <span data-ttu-id="8d9b1-136">Int64</span><span class="sxs-lookup"><span data-stu-id="8d9b1-136">Int64</span></span>                                                | <span data-ttu-id="8d9b1-137">アイテムのこのバージョンのコンテンツ ストリームのサイズを示します。</span><span class="sxs-lookup"><span data-stu-id="8d9b1-137">Indicates the size of the content stream for this version of the item.</span></span>  |
| <span data-ttu-id="8d9b1-138">**content**</span><span class="sxs-lookup"><span data-stu-id="8d9b1-138">**content**</span></span>              | <span data-ttu-id="8d9b1-139">ストリーム</span><span class="sxs-lookup"><span data-stu-id="8d9b1-139">Stream</span></span>                                               | <span data-ttu-id="8d9b1-140">アイテムのこのバージョンのコンテンツストリーム。</span><span class="sxs-lookup"><span data-stu-id="8d9b1-140">The content stream for this version of the item.</span></span>                        |

<!-- {
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version"
} -->
