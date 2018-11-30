---
author: rgregg
ms.author: rgregg
ms.date: 09/17/2017
title: ListItemVersion
ms.openlocfilehash: 7cda16159c6e5e58a0f60aef3c60198c7615f9e0
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066560"
---
# <a name="listitemversion-resource-type"></a><span data-ttu-id="6bdaf-102">ListItemVersion リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6bdaf-102">ListItemVersion resource type</span></span>

> <span data-ttu-id="6bdaf-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6bdaf-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6bdaf-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6bdaf-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6bdaf-105">**listItemVersion** リソースは、[ListItem](listitem.md) リソースの旧バージョンを表しています。</span><span class="sxs-lookup"><span data-stu-id="6bdaf-105">The **listItemVersion** resource represents a previous version of a [ListItem](listitem.md) resource.</span></span>

## <a name="tasks-on-listitemversion-resources"></a><span data-ttu-id="6bdaf-106">ListItemVersion リソースのタスク</span><span class="sxs-lookup"><span data-stu-id="6bdaf-106">Tasks on ListItemVersion resources</span></span>

<span data-ttu-id="6bdaf-107">listItemVersion リソースで使用可能なタスクを次に示します。</span><span class="sxs-lookup"><span data-stu-id="6bdaf-107">The following tasks are available for listItemVersion resources.</span></span>

|            <span data-ttu-id="6bdaf-108">共通タスク</span><span class="sxs-lookup"><span data-stu-id="6bdaf-108">Common task</span></span>             |         <span data-ttu-id="6bdaf-109">HTTP メソッド</span><span class="sxs-lookup"><span data-stu-id="6bdaf-109">HTTP method</span></span>         |
| :--------------------------------- | :-------------------------- |
| <span data-ttu-id="6bdaf-110">[バージョンの一覧表示][version-list]</span><span class="sxs-lookup"><span data-stu-id="6bdaf-110">[List versions][version-list]</span></span>      | `GET /sites/{site-id}/items/{item-id}/versions`  |
| <span data-ttu-id="6bdaf-111">[バージョンの取得][version-get]</span><span class="sxs-lookup"><span data-stu-id="6bdaf-111">[Get version][version-get]</span></span>         | `GET /sites/{site-id}/items/versions/{version-id}`     |
| <span data-ttu-id="6bdaf-112">[バージョンの復元][version-restore]</span><span class="sxs-lookup"><span data-stu-id="6bdaf-112">[Restore version][version-restore]</span></span> | `POST /sites/{site-id}/items/versions/{version-id}/restore` |

[version-list]: ../api/listitem-list-versions.md
[version-get]: ../api/listitemversion-get.md
[version-restore]: ../api/listitemversion-restore.md


## <a name="json-representation"></a><span data-ttu-id="6bdaf-113">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6bdaf-113">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.listItemVersion", "@type.aka": "oneDrive.baseItemVersion" } -->

```json
{
  "content": { "@odata.type": "Edm.Stream" },
  "fields": { "@odata.type": "microsoft.graph.fieldValueSet" },
  "id": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "2016-01-01T15:20:01.125Z",
  "published": { "@odata.type": "microsoft.graph.publicationFacet" }
}
```

## <a name="properties"></a><span data-ttu-id="6bdaf-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6bdaf-114">Properties</span></span>

|      <span data-ttu-id="6bdaf-115">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="6bdaf-115">Property name</span></span>       |                         <span data-ttu-id="6bdaf-116">型</span><span class="sxs-lookup"><span data-stu-id="6bdaf-116">Type</span></span>                         |                               <span data-ttu-id="6bdaf-117">説明</span><span class="sxs-lookup"><span data-stu-id="6bdaf-117">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="6bdaf-118">**id**</span><span class="sxs-lookup"><span data-stu-id="6bdaf-118">**id**</span></span>                   | <span data-ttu-id="6bdaf-119">string</span><span class="sxs-lookup"><span data-stu-id="6bdaf-119">string</span></span>                                               | <span data-ttu-id="6bdaf-120">バージョンの ID。</span><span class="sxs-lookup"><span data-stu-id="6bdaf-120">The ID of the version.</span></span> <span data-ttu-id="6bdaf-121">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="6bdaf-121">Read-only.</span></span>                                       |
| <span data-ttu-id="6bdaf-122">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="6bdaf-122">**lastModifiedBy**</span></span>       | [<span data-ttu-id="6bdaf-123">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="6bdaf-123">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="6bdaf-124">最後にバージョンを変更したユーザーの ID。</span><span class="sxs-lookup"><span data-stu-id="6bdaf-124">Identity of the user which last modified the version.</span></span> <span data-ttu-id="6bdaf-125">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="6bdaf-125">Read-only.</span></span>        |
| <span data-ttu-id="6bdaf-126">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="6bdaf-126">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="6bdaf-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6bdaf-127">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="6bdaf-128">バージョンが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="6bdaf-128">Date and time the version was last modified.</span></span> <span data-ttu-id="6bdaf-129">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="6bdaf-129">Read-only.</span></span>                 |
| <span data-ttu-id="6bdaf-130">**published**</span><span class="sxs-lookup"><span data-stu-id="6bdaf-130">**published**</span></span>            | [<span data-ttu-id="6bdaf-131">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="6bdaf-131">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="6bdaf-132">特定のバージョンのパブリケーション ステータスを示します。</span><span class="sxs-lookup"><span data-stu-id="6bdaf-132">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="6bdaf-133">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="6bdaf-133">Read-only.</span></span> |


## <a name="relationships"></a><span data-ttu-id="6bdaf-134">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6bdaf-134">Relationships</span></span>

<span data-ttu-id="6bdaf-135">次の表は、**driveItemVersion** リソースが他のリソースに対して持っているリレーションシップを定義しています。</span><span class="sxs-lookup"><span data-stu-id="6bdaf-135">The following table defines the relationships that the **driveItemVersion** resource has to other resources.</span></span>

| <span data-ttu-id="6bdaf-136">リレーションシップ名</span><span class="sxs-lookup"><span data-stu-id="6bdaf-136">Relationship name</span></span> |                      <span data-ttu-id="6bdaf-137">種類</span><span class="sxs-lookup"><span data-stu-id="6bdaf-137">Type</span></span>                      |                               <span data-ttu-id="6bdaf-138">説明</span><span class="sxs-lookup"><span data-stu-id="6bdaf-138">Description</span></span>                                |
| :---------------- | :--------------------------------------------- | :----------------------------------------------------------------------- |
| <span data-ttu-id="6bdaf-139">**fields**</span><span class="sxs-lookup"><span data-stu-id="6bdaf-139">**fields**</span></span>        | [<span data-ttu-id="6bdaf-140">FieldValueSet</span><span class="sxs-lookup"><span data-stu-id="6bdaf-140">FieldValueSet</span></span>](../resources/fieldvalueset.md) | <span data-ttu-id="6bdaf-141">このバージョンのリスト アイテムの、フィールドと値のコレクション。</span><span class="sxs-lookup"><span data-stu-id="6bdaf-141">A collection of the fields and values for this version of the list item.</span></span> |


<!-- {
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version"
} -->