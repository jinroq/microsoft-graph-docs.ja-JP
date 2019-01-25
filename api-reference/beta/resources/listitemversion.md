---
author: rgregg
ms.author: rgregg
ms.date: 09/17/2017
title: listItemVersion
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 1d153a8ae8291e0299d1a470db6c8c7e0c8bd3e4
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524752"
---
# <a name="listitemversion-resource-type"></a><span data-ttu-id="32941-102">ListItemVersion リソースの種類</span><span class="sxs-lookup"><span data-stu-id="32941-102">ListItemVersion resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="32941-103">**listItemVersion** リソースは、[ListItem](listitem.md) リソースの旧バージョンを表しています。</span><span class="sxs-lookup"><span data-stu-id="32941-103">The **listItemVersion** resource represents a previous version of a [ListItem](listitem.md) resource.</span></span>

## <a name="tasks-on-listitemversion-resources"></a><span data-ttu-id="32941-104">ListItemVersion リソースのタスク</span><span class="sxs-lookup"><span data-stu-id="32941-104">Tasks on ListItemVersion resources</span></span>

<span data-ttu-id="32941-105">listItemVersion リソースで使用可能なタスクを次に示します。</span><span class="sxs-lookup"><span data-stu-id="32941-105">The following tasks are available for listItemVersion resources.</span></span>

|            <span data-ttu-id="32941-106">共通タスク</span><span class="sxs-lookup"><span data-stu-id="32941-106">Common task</span></span>             |         <span data-ttu-id="32941-107">HTTP メソッド</span><span class="sxs-lookup"><span data-stu-id="32941-107">HTTP method</span></span>         |
| :--------------------------------- | :-------------------------- |
| <span data-ttu-id="32941-108">[バージョンの一覧表示][version-list]</span><span class="sxs-lookup"><span data-stu-id="32941-108">[List versions][version-list]</span></span>      | `GET /sites/{site-id}/items/{item-id}/versions`  |
| <span data-ttu-id="32941-109">[バージョンの取得][version-get]</span><span class="sxs-lookup"><span data-stu-id="32941-109">[Get version][version-get]</span></span>         | `GET /sites/{site-id}/items/versions/{version-id}`     |
| <span data-ttu-id="32941-110">[バージョンの復元][version-restore]</span><span class="sxs-lookup"><span data-stu-id="32941-110">[Restore version][version-restore]</span></span> | `POST /sites/{site-id}/items/versions/{version-id}/restore` |

[version-list]: ../api/listitem-list-versions.md
[version-get]: ../api/listitemversion-get.md
[version-restore]: ../api/listitemversion-restore.md


## <a name="json-representation"></a><span data-ttu-id="32941-111">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="32941-111">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="32941-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="32941-112">Properties</span></span>

|      <span data-ttu-id="32941-113">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="32941-113">Property name</span></span>       |                         <span data-ttu-id="32941-114">種類</span><span class="sxs-lookup"><span data-stu-id="32941-114">Type</span></span>                         |                               <span data-ttu-id="32941-115">説明</span><span class="sxs-lookup"><span data-stu-id="32941-115">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="32941-116">**id**</span><span class="sxs-lookup"><span data-stu-id="32941-116">**id**</span></span>                   | <span data-ttu-id="32941-117">string</span><span class="sxs-lookup"><span data-stu-id="32941-117">string</span></span>                                               | <span data-ttu-id="32941-118">バージョンの ID。</span><span class="sxs-lookup"><span data-stu-id="32941-118">The ID of the version.</span></span> <span data-ttu-id="32941-119">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="32941-119">Read-only.</span></span>                                       |
| <span data-ttu-id="32941-120">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="32941-120">**lastModifiedBy**</span></span>       | [<span data-ttu-id="32941-121">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="32941-121">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="32941-122">最後にバージョンを変更したユーザーの ID。</span><span class="sxs-lookup"><span data-stu-id="32941-122">Identity of the user which last modified the version.</span></span> <span data-ttu-id="32941-123">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="32941-123">Read-only.</span></span>        |
| <span data-ttu-id="32941-124">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="32941-124">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="32941-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="32941-125">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="32941-126">バージョンが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="32941-126">Date and time the version was last modified.</span></span> <span data-ttu-id="32941-127">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="32941-127">Read-only.</span></span>                 |
| <span data-ttu-id="32941-128">**published**</span><span class="sxs-lookup"><span data-stu-id="32941-128">**published**</span></span>            | [<span data-ttu-id="32941-129">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="32941-129">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="32941-130">特定のバージョンのパブリケーション ステータスを示します。</span><span class="sxs-lookup"><span data-stu-id="32941-130">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="32941-131">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="32941-131">Read-only.</span></span> |


## <a name="relationships"></a><span data-ttu-id="32941-132">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="32941-132">Relationships</span></span>

<span data-ttu-id="32941-133">次の表は、**driveItemVersion** リソースが他のリソースに対して持っているリレーションシップを定義しています。</span><span class="sxs-lookup"><span data-stu-id="32941-133">The following table defines the relationships that the **driveItemVersion** resource has to other resources.</span></span>

| <span data-ttu-id="32941-134">リレーションシップ名</span><span class="sxs-lookup"><span data-stu-id="32941-134">Relationship name</span></span> |                      <span data-ttu-id="32941-135">種類</span><span class="sxs-lookup"><span data-stu-id="32941-135">Type</span></span>                      |                               <span data-ttu-id="32941-136">説明</span><span class="sxs-lookup"><span data-stu-id="32941-136">Description</span></span>                                |
| :---------------- | :--------------------------------------------- | :----------------------------------------------------------------------- |
| <span data-ttu-id="32941-137">**fields**</span><span class="sxs-lookup"><span data-stu-id="32941-137">**fields**</span></span>        | [<span data-ttu-id="32941-138">FieldValueSet</span><span class="sxs-lookup"><span data-stu-id="32941-138">FieldValueSet</span></span>](../resources/fieldvalueset.md) | <span data-ttu-id="32941-139">このバージョンのリスト アイテムの、フィールドと値のコレクション。</span><span class="sxs-lookup"><span data-stu-id="32941-139">A collection of the fields and values for this version of the list item.</span></span> |


<!--
{
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version",
  "suppressions": [
    "Error: /api-reference/beta/resources/listitemversion.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
