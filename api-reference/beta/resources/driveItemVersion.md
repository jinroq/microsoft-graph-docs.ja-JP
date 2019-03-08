---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/17/2017
title: DriveItemVersion
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 3be7cd044b65eccd2370a2848258b415c5e70b00
ms.sourcegitcommit: b877a8dc9aeaf74f975ca495b401ffff001d7699
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/08/2019
ms.locfileid: "30482365"
---
# <a name="driveitemversion-resource-type"></a><span data-ttu-id="2ff3f-102">DriveItemVersion リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2ff3f-102">DriveItemVersion resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2ff3f-103">**DriveItemVersion** リソースは、[DriveItem](driveitem.md) の特定のバージョンを表しています。</span><span class="sxs-lookup"><span data-stu-id="2ff3f-103">The **DriveItemVersion** resource represents a specific version of a [DriveItem](driveitem.md).</span></span>


## <a name="tasks-on-driveitemversion-resources"></a><span data-ttu-id="2ff3f-104">DriveItemVersion リソースのタスク</span><span class="sxs-lookup"><span data-stu-id="2ff3f-104">Tasks on DriveItemVersion resources</span></span>

<span data-ttu-id="2ff3f-105">driveItemVersion リソースで使用可能なタスクを次に示します。</span><span class="sxs-lookup"><span data-stu-id="2ff3f-105">The following tasks are available for driveItemVersion resources.</span></span>

|            <span data-ttu-id="2ff3f-106">共通タスク</span><span class="sxs-lookup"><span data-stu-id="2ff3f-106">Common task</span></span>             |         <span data-ttu-id="2ff3f-107">HTTP メソッド</span><span class="sxs-lookup"><span data-stu-id="2ff3f-107">HTTP method</span></span>         |
| :--------------------------------- | :-------------------------- |
| <span data-ttu-id="2ff3f-108">[バージョンの一覧表示][version-list]</span><span class="sxs-lookup"><span data-stu-id="2ff3f-108">[List versions][version-list]</span></span>      | `GET /drive/items/{item-id}/versions`  |
| <span data-ttu-id="2ff3f-109">[バージョンの取得][version-get]</span><span class="sxs-lookup"><span data-stu-id="2ff3f-109">[Get version][version-get]</span></span>         | `GET /drive/items/{item-id}/versions/{version-id}`     |
| <span data-ttu-id="2ff3f-110">[コンテンツの取得][content-get]</span><span class="sxs-lookup"><span data-stu-id="2ff3f-110">[Get contents][content-get]</span></span>        | `GET /drive/items/{item-id}/versions/{version-id}/content` |
| <span data-ttu-id="2ff3f-111">[バージョンの復元][version-restore]</span><span class="sxs-lookup"><span data-stu-id="2ff3f-111">[Restore version][version-restore]</span></span> | `POST /drive/items/{item-id}/versions/{version-id}/restoreversion` |

[version-list]: ../api/driveitem-list-versions.md
[version-get]: ../api/driveitemversion-get.md
[content-get]: ../api/driveitemversion-get-contents.md
[version-restore]: ../api/driveitemversion-restore.md

<span data-ttu-id="2ff3f-112">前の表では、例に `/drive` を使用していますが、他にも有効な要求が多数あります。</span><span class="sxs-lookup"><span data-stu-id="2ff3f-112">In the previous table, the examples use `/drive`, but there are many valid requests.</span></span>

## <a name="json-representation"></a><span data-ttu-id="2ff3f-113">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2ff3f-113">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.driveItemVersion", "@type.aka": "oneDrive.driveItemVersion" } -->

```json
{
  "content": { "@odata.type": "Edm.Stream" },
  "id": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "2016-01-01T15:20:01.125Z",
  "publication": { "@odata.type": "microsoft.graph.publicationFacet" }
}
```

## <a name="properties"></a><span data-ttu-id="2ff3f-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2ff3f-114">Properties</span></span>

|      <span data-ttu-id="2ff3f-115">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="2ff3f-115">Property name</span></span>       |                         <span data-ttu-id="2ff3f-116">種類</span><span class="sxs-lookup"><span data-stu-id="2ff3f-116">Type</span></span>                         |                               <span data-ttu-id="2ff3f-117">説明</span><span class="sxs-lookup"><span data-stu-id="2ff3f-117">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="2ff3f-118">**id**</span><span class="sxs-lookup"><span data-stu-id="2ff3f-118">**id**</span></span>                   | <span data-ttu-id="2ff3f-119">string</span><span class="sxs-lookup"><span data-stu-id="2ff3f-119">string</span></span>                                               | <span data-ttu-id="2ff3f-120">バージョンの ID。</span><span class="sxs-lookup"><span data-stu-id="2ff3f-120">The ID of the version.</span></span> <span data-ttu-id="2ff3f-121">値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="2ff3f-121">Read-only.</span></span>                                       |
| <span data-ttu-id="2ff3f-122">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="2ff3f-122">**lastModifiedBy**</span></span>       | [<span data-ttu-id="2ff3f-123">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="2ff3f-123">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="2ff3f-124">最後にバージョンを変更したユーザーの ID。</span><span class="sxs-lookup"><span data-stu-id="2ff3f-124">Identity of the user which last modified the version.</span></span> <span data-ttu-id="2ff3f-125">値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="2ff3f-125">Read-only.</span></span>        |
| <span data-ttu-id="2ff3f-126">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="2ff3f-126">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="2ff3f-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2ff3f-127">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="2ff3f-128">バージョンが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="2ff3f-128">Date and time the version was last modified.</span></span> <span data-ttu-id="2ff3f-129">値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="2ff3f-129">Read-only.</span></span>                 |
| <span data-ttu-id="2ff3f-130">**publication**</span><span class="sxs-lookup"><span data-stu-id="2ff3f-130">**publication**</span></span>          | [<span data-ttu-id="2ff3f-131">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="2ff3f-131">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="2ff3f-132">特定のバージョンのパブリケーション ステータスを示します。</span><span class="sxs-lookup"><span data-stu-id="2ff3f-132">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="2ff3f-133">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="2ff3f-133">Read-only.</span></span> |
| <span data-ttu-id="2ff3f-134">**size**</span><span class="sxs-lookup"><span data-stu-id="2ff3f-134">**size**</span></span>                 | <span data-ttu-id="2ff3f-135">Int64</span><span class="sxs-lookup"><span data-stu-id="2ff3f-135">Int64</span></span>                                                | <span data-ttu-id="2ff3f-136">アイテムのこのバージョンのコンテンツ ストリームのサイズを示します。</span><span class="sxs-lookup"><span data-stu-id="2ff3f-136">Indicates the size of the content stream for this version of the item.</span></span>  |

## <a name="relationships"></a><span data-ttu-id="2ff3f-137">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2ff3f-137">Relationships</span></span>

<span data-ttu-id="2ff3f-138">次の表は、**driveItemVersion** リソースが他のリソースに対して持っているリレーションシップを定義しています。</span><span class="sxs-lookup"><span data-stu-id="2ff3f-138">The following table defines the relationships that the **driveItemVersion** resource has to other resources.</span></span>

| <span data-ttu-id="2ff3f-139">リレーションシップ名</span><span class="sxs-lookup"><span data-stu-id="2ff3f-139">Relationship name</span></span> |  <span data-ttu-id="2ff3f-140">種類</span><span class="sxs-lookup"><span data-stu-id="2ff3f-140">Type</span></span>  |            <span data-ttu-id="2ff3f-141">説明</span><span class="sxs-lookup"><span data-stu-id="2ff3f-141">Description</span></span>             |
| :---------------- | :----- | :--------------------------------- |
| <span data-ttu-id="2ff3f-142">**content**</span><span class="sxs-lookup"><span data-stu-id="2ff3f-142">**content**</span></span>       | <span data-ttu-id="2ff3f-143">ストリーム</span><span class="sxs-lookup"><span data-stu-id="2ff3f-143">Stream</span></span> | <span data-ttu-id="2ff3f-144">バージョンのコンテンツ ストリーム。</span><span class="sxs-lookup"><span data-stu-id="2ff3f-144">The content stream of the version.</span></span> |

<!--
{
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version",
  "suppressions": [
    "Error: /api-reference/beta/resources/driveItemVersion.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
