---
author: rgregg
ms.author: rgregg
ms.date: 09/17/2017
title: DriveItemVersion
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 3f33c59da4a748c176c6044e4db3bac70eac71cb
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27923615"
---
# <a name="driveitemversion-resource-type"></a><span data-ttu-id="163d6-102">DriveItemVersion リソースの種類</span><span class="sxs-lookup"><span data-stu-id="163d6-102">DriveItemVersion resource type</span></span>

> <span data-ttu-id="163d6-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="163d6-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="163d6-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="163d6-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="163d6-105">**DriveItemVersion** リソースは、[DriveItem](driveitem.md) の特定のバージョンを表しています。</span><span class="sxs-lookup"><span data-stu-id="163d6-105">The **DriveItemVersion** resource represents a specific version of a [DriveItem](driveitem.md).</span></span>


## <a name="tasks-on-driveitemversion-resources"></a><span data-ttu-id="163d6-106">DriveItemVersion リソースのタスク</span><span class="sxs-lookup"><span data-stu-id="163d6-106">Tasks on DriveItemVersion resources</span></span>

<span data-ttu-id="163d6-107">driveItemVersion リソースで使用可能なタスクを次に示します。</span><span class="sxs-lookup"><span data-stu-id="163d6-107">The following tasks are available for driveItemVersion resources.</span></span>

|            <span data-ttu-id="163d6-108">共通タスク</span><span class="sxs-lookup"><span data-stu-id="163d6-108">Common task</span></span>             |         <span data-ttu-id="163d6-109">HTTP メソッド</span><span class="sxs-lookup"><span data-stu-id="163d6-109">HTTP method</span></span>         |
| :--------------------------------- | :-------------------------- |
| <span data-ttu-id="163d6-110">[バージョンの一覧表示][version-list]</span><span class="sxs-lookup"><span data-stu-id="163d6-110">[List versions][version-list]</span></span>      | `GET /drive/items/{item-id}/versions`  |
| <span data-ttu-id="163d6-111">[バージョンの取得][version-get]</span><span class="sxs-lookup"><span data-stu-id="163d6-111">[Get version][version-get]</span></span>         | `GET /drive/items/{item-id}/versions/{version-id}`     |
| <span data-ttu-id="163d6-112">[コンテンツの取得][content-get]</span><span class="sxs-lookup"><span data-stu-id="163d6-112">[Get contents][content-get]</span></span>        | `GET /drive/items/{item-id}/versions/{version-id}/content` |
| <span data-ttu-id="163d6-113">[バージョンの復元][version-restore]</span><span class="sxs-lookup"><span data-stu-id="163d6-113">[Restore version][version-restore]</span></span> | `POST /drive/items/{item-id}/versions/{version-id}/restore` |

[version-list]: ../api/driveitem-list-versions.md
[version-get]: ../api/driveitemversion-get.md
[content-get]: ../api/driveitemversion-get-contents.md
[version-restore]: ../api/driveitemversion-restore.md

<span data-ttu-id="163d6-114">前の表では、例に `/drive` を使用していますが、他にも有効な要求が多数あります。</span><span class="sxs-lookup"><span data-stu-id="163d6-114">In the previous table, the examples use `/drive`, but there are many valid requests.</span></span>

## <a name="json-representation"></a><span data-ttu-id="163d6-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="163d6-115">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="163d6-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="163d6-116">Properties</span></span>

|      <span data-ttu-id="163d6-117">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="163d6-117">Property name</span></span>       |                         <span data-ttu-id="163d6-118">型</span><span class="sxs-lookup"><span data-stu-id="163d6-118">Type</span></span>                         |                               <span data-ttu-id="163d6-119">説明</span><span class="sxs-lookup"><span data-stu-id="163d6-119">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="163d6-120">**id**</span><span class="sxs-lookup"><span data-stu-id="163d6-120">**id**</span></span>                   | <span data-ttu-id="163d6-121">string</span><span class="sxs-lookup"><span data-stu-id="163d6-121">string</span></span>                                               | <span data-ttu-id="163d6-122">バージョンの ID。</span><span class="sxs-lookup"><span data-stu-id="163d6-122">The ID of the version.</span></span> <span data-ttu-id="163d6-123">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="163d6-123">Read-only.</span></span>                                       |
| <span data-ttu-id="163d6-124">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="163d6-124">**lastModifiedBy**</span></span>       | [<span data-ttu-id="163d6-125">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="163d6-125">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="163d6-126">最後にバージョンを変更したユーザーの ID。</span><span class="sxs-lookup"><span data-stu-id="163d6-126">Identity of the user which last modified the version.</span></span> <span data-ttu-id="163d6-127">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="163d6-127">Read-only.</span></span>        |
| <span data-ttu-id="163d6-128">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="163d6-128">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="163d6-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="163d6-129">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="163d6-130">バージョンが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="163d6-130">Date and time the version was last modified.</span></span> <span data-ttu-id="163d6-131">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="163d6-131">Read-only.</span></span>                 |
| <span data-ttu-id="163d6-132">**publication**</span><span class="sxs-lookup"><span data-stu-id="163d6-132">**publication**</span></span>          | [<span data-ttu-id="163d6-133">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="163d6-133">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="163d6-134">特定のバージョンのパブリケーション ステータスを示します。</span><span class="sxs-lookup"><span data-stu-id="163d6-134">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="163d6-135">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="163d6-135">Read-only.</span></span> |
| <span data-ttu-id="163d6-136">**size**</span><span class="sxs-lookup"><span data-stu-id="163d6-136">**size**</span></span>                 | <span data-ttu-id="163d6-137">Int64</span><span class="sxs-lookup"><span data-stu-id="163d6-137">Int64</span></span>                                                | <span data-ttu-id="163d6-138">アイテムのこのバージョンのコンテンツ ストリームのサイズを示します。</span><span class="sxs-lookup"><span data-stu-id="163d6-138">Indicates the size of the content stream for this version of the item.</span></span>  |

## <a name="relationships"></a><span data-ttu-id="163d6-139">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="163d6-139">Relationships</span></span>

<span data-ttu-id="163d6-140">次の表は、**driveItemVersion** リソースが他のリソースに対して持っているリレーションシップを定義しています。</span><span class="sxs-lookup"><span data-stu-id="163d6-140">The following table defines the relationships that the **driveItemVersion** resource has to other resources.</span></span>

| <span data-ttu-id="163d6-141">リレーションシップ名</span><span class="sxs-lookup"><span data-stu-id="163d6-141">Relationship name</span></span> |  <span data-ttu-id="163d6-142">種類</span><span class="sxs-lookup"><span data-stu-id="163d6-142">Type</span></span>  |            <span data-ttu-id="163d6-143">説明</span><span class="sxs-lookup"><span data-stu-id="163d6-143">Description</span></span>             |
| :---------------- | :----- | :--------------------------------- |
| <span data-ttu-id="163d6-144">**content**</span><span class="sxs-lookup"><span data-stu-id="163d6-144">**content**</span></span>       | <span data-ttu-id="163d6-145">ストリーム</span><span class="sxs-lookup"><span data-stu-id="163d6-145">Stream</span></span> | <span data-ttu-id="163d6-146">バージョンのコンテンツ ストリーム。</span><span class="sxs-lookup"><span data-stu-id="163d6-146">The content stream of the version.</span></span> |

<!-- {
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version"
} -->
