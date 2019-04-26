---
title: DriveItemVersion リソースの種類
description: '**drive itemversion**リソースは、ドライブ項目の特定のバージョンを表します。'
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: fd6052464d40fcce86b83d93601282dda252c69b
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562686"
---
# <a name="driveitemversion-resource-type"></a><span data-ttu-id="ad421-103">DriveItemVersion リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ad421-103">DriveItemVersion resource type</span></span>

<span data-ttu-id="ad421-104">**DriveItemVersion** リソースは、[DriveItem](driveitem.md) の特定のバージョンを表しています。</span><span class="sxs-lookup"><span data-stu-id="ad421-104">The **DriveItemVersion** resource represents a specific version of a [DriveItem](driveitem.md).</span></span>


## <a name="tasks-on-driveitemversion-resources"></a><span data-ttu-id="ad421-105">DriveItemVersion リソースのタスク</span><span class="sxs-lookup"><span data-stu-id="ad421-105">Tasks on DriveItemVersion resources</span></span>

<span data-ttu-id="ad421-106">driveItemVersion リソースで使用可能なタスクを次に示します。</span><span class="sxs-lookup"><span data-stu-id="ad421-106">The following tasks are available for driveItemVersion resources.</span></span>

|            <span data-ttu-id="ad421-107">共通タスク</span><span class="sxs-lookup"><span data-stu-id="ad421-107">Common task</span></span>             |         <span data-ttu-id="ad421-108">HTTP メソッド</span><span class="sxs-lookup"><span data-stu-id="ad421-108">HTTP method</span></span>         |
| :--------------------------------- | :-------------------------- |
| <span data-ttu-id="ad421-109">[バージョンの一覧表示][version-list]</span><span class="sxs-lookup"><span data-stu-id="ad421-109">[List versions][version-list]</span></span>      | `GET /drive/items/{item-id}/versions`  |
| <span data-ttu-id="ad421-110">[バージョンの取得][version-get]</span><span class="sxs-lookup"><span data-stu-id="ad421-110">[Get version][version-get]</span></span>         | `GET /drive/items/{item-id}/versions/{version-id}`     |
| <span data-ttu-id="ad421-111">[コンテンツの取得][content-get]</span><span class="sxs-lookup"><span data-stu-id="ad421-111">[Get contents][content-get]</span></span>        | `GET /drive/items/{item-id}/versions/{version-id}/content` |
| <span data-ttu-id="ad421-112">[バージョンの復元][version-restore]</span><span class="sxs-lookup"><span data-stu-id="ad421-112">[Restore version][version-restore]</span></span> | `POST /drive/items/{item-id}/versions/{version-id}/restoreversion` |

[version-list]: ../api/driveitem-list-versions.md
[version-get]: ../api/driveitemversion-get.md
[content-get]: ../api/driveitemversion-get-contents.md
[version-restore]: ../api/driveitemversion-restore.md

<span data-ttu-id="ad421-113">前の表では、例に `/drive` を使用していますが、他にも有効な要求が多数あります。</span><span class="sxs-lookup"><span data-stu-id="ad421-113">In the previous table, the examples use `/drive`, but there are many valid requests.</span></span>

## <a name="json-representation"></a><span data-ttu-id="ad421-114">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ad421-114">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="ad421-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ad421-115">Properties</span></span>

|      <span data-ttu-id="ad421-116">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="ad421-116">Property name</span></span>       |                         <span data-ttu-id="ad421-117">種類</span><span class="sxs-lookup"><span data-stu-id="ad421-117">Type</span></span>                         |                               <span data-ttu-id="ad421-118">説明</span><span class="sxs-lookup"><span data-stu-id="ad421-118">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="ad421-119">**id**</span><span class="sxs-lookup"><span data-stu-id="ad421-119">**id**</span></span>                   | <span data-ttu-id="ad421-120">string</span><span class="sxs-lookup"><span data-stu-id="ad421-120">string</span></span>                                               | <span data-ttu-id="ad421-121">バージョンの ID。</span><span class="sxs-lookup"><span data-stu-id="ad421-121">The ID of the version.</span></span> <span data-ttu-id="ad421-122">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="ad421-122">Read-only.</span></span>                                       |
| <span data-ttu-id="ad421-123">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="ad421-123">**lastModifiedBy**</span></span>       | [<span data-ttu-id="ad421-124">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="ad421-124">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="ad421-125">最後にバージョンを変更したユーザーの ID。</span><span class="sxs-lookup"><span data-stu-id="ad421-125">Identity of the user which last modified the version.</span></span> <span data-ttu-id="ad421-126">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ad421-126">Read-only.</span></span>        |
| <span data-ttu-id="ad421-127">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="ad421-127">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="ad421-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ad421-128">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="ad421-129">バージョンが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="ad421-129">Date and time the version was last modified.</span></span> <span data-ttu-id="ad421-130">読み取り専用。</span><span class="sxs-lookup"><span data-stu-id="ad421-130">Read-only.</span></span>                 |
| <span data-ttu-id="ad421-131">**publication**</span><span class="sxs-lookup"><span data-stu-id="ad421-131">**publication**</span></span>          | [<span data-ttu-id="ad421-132">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="ad421-132">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="ad421-133">特定のバージョンのパブリケーション ステータスを示します。</span><span class="sxs-lookup"><span data-stu-id="ad421-133">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="ad421-134">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="ad421-134">Read-only.</span></span> |
| <span data-ttu-id="ad421-135">**size**</span><span class="sxs-lookup"><span data-stu-id="ad421-135">**size**</span></span>                 | <span data-ttu-id="ad421-136">Int64</span><span class="sxs-lookup"><span data-stu-id="ad421-136">Int64</span></span>                                                | <span data-ttu-id="ad421-137">アイテムのこのバージョンのコンテンツ ストリームのサイズを示します。</span><span class="sxs-lookup"><span data-stu-id="ad421-137">Indicates the size of the content stream for this version of the item.</span></span>  |
| <span data-ttu-id="ad421-138">**content**</span><span class="sxs-lookup"><span data-stu-id="ad421-138">**content**</span></span>              | <span data-ttu-id="ad421-139">ストリーム</span><span class="sxs-lookup"><span data-stu-id="ad421-139">Stream</span></span>                                               | <span data-ttu-id="ad421-140">アイテムのこのバージョンのコンテンツストリーム。</span><span class="sxs-lookup"><span data-stu-id="ad421-140">The content stream for this version of the item.</span></span>                        |

<!-- {
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version"
} -->
