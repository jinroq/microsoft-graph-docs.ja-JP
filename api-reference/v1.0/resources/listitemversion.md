---
title: ListItemVersion リソースの種類
description: '**listItemVersion** リソースは、ListItem リソースの旧バージョンを表しています。'
localization_priority: Normal
ms.openlocfilehash: 41dcbeee3f098b6c156a7ddfe484ef42cca8b6d8
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27810683"
---
# <a name="listitemversion-resource-type"></a><span data-ttu-id="040d9-103">ListItemVersion リソースの種類</span><span class="sxs-lookup"><span data-stu-id="040d9-103">ListItemVersion resource type</span></span>

<span data-ttu-id="040d9-104">**listItemVersion** リソースは、[ListItem](listitem.md) リソースの旧バージョンを表しています。</span><span class="sxs-lookup"><span data-stu-id="040d9-104">The **listItemVersion** resource represents a previous version of a [ListItem](listitem.md) resource.</span></span>

## <a name="tasks-on-listitemversion-resources"></a><span data-ttu-id="040d9-105">ListItemVersion リソースのタスク</span><span class="sxs-lookup"><span data-stu-id="040d9-105">Tasks on ListItemVersion resources</span></span>

<span data-ttu-id="040d9-106">listItemVersion リソースで使用可能なタスクを次に示します。</span><span class="sxs-lookup"><span data-stu-id="040d9-106">The following tasks are available for listItemVersion resources.</span></span>

|            <span data-ttu-id="040d9-107">共通タスク</span><span class="sxs-lookup"><span data-stu-id="040d9-107">Common task</span></span>             |         <span data-ttu-id="040d9-108">HTTP メソッド</span><span class="sxs-lookup"><span data-stu-id="040d9-108">HTTP method</span></span>         |
| :--------------------------------- | :-------------------------- |
| <span data-ttu-id="040d9-109">[バージョンの一覧表示][version-list]</span><span class="sxs-lookup"><span data-stu-id="040d9-109">[List versions][version-list]</span></span>      | `GET /sites/{site-id}/items/{item-id}/versions`  |
| <span data-ttu-id="040d9-110">[バージョンの取得][version-get]</span><span class="sxs-lookup"><span data-stu-id="040d9-110">[Get version][version-get]</span></span>         | `GET /sites/{site-id}/items/{item-id}/versions/{version-id}`     |
| <span data-ttu-id="040d9-111">[バージョンの復元][version-restore]</span><span class="sxs-lookup"><span data-stu-id="040d9-111">[Restore version][version-restore]</span></span> | `POST /sites/{site-id}/items/{item-id}/versions/{version-id}/restore` |

[version-list]: ../api/listitem-list-versions.md
[version-get]: ../api/listitemversion-get.md
[version-restore]: ../api/listitemversion-restore.md


## <a name="json-representation"></a><span data-ttu-id="040d9-112">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="040d9-112">JSON representation</span></span>

<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.baseItemVersion",
  "@odata.type": "microsoft.graph.listItemVersion",
  "@type.aka": "oneDrive.baseItemVersion"
}-->

```json
{
  "fields": { "@odata.type": "microsoft.graph.fieldValueSet" },
  "id": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "2016-01-01T15:20:01.125Z",
  "published": { "@odata.type": "microsoft.graph.publicationFacet" }
}
```

## <a name="properties"></a><span data-ttu-id="040d9-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="040d9-113">Properties</span></span>

|      <span data-ttu-id="040d9-114">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="040d9-114">Property name</span></span>       |                         <span data-ttu-id="040d9-115">Type</span><span class="sxs-lookup"><span data-stu-id="040d9-115">Type</span></span>                         |                               <span data-ttu-id="040d9-116">説明</span><span class="sxs-lookup"><span data-stu-id="040d9-116">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="040d9-117">**id**</span><span class="sxs-lookup"><span data-stu-id="040d9-117">**id**</span></span>                   | <span data-ttu-id="040d9-118">string</span><span class="sxs-lookup"><span data-stu-id="040d9-118">string</span></span>                                               | <span data-ttu-id="040d9-119">バージョンの ID。</span><span class="sxs-lookup"><span data-stu-id="040d9-119">The ID of the version.</span></span> <span data-ttu-id="040d9-120">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="040d9-120">Read-only.</span></span>                                       |
| <span data-ttu-id="040d9-121">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="040d9-121">**lastModifiedBy**</span></span>       | [<span data-ttu-id="040d9-122">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="040d9-122">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="040d9-123">最後にバージョンを変更したユーザーの ID。</span><span class="sxs-lookup"><span data-stu-id="040d9-123">Identity of the user which last modified the version.</span></span> <span data-ttu-id="040d9-124">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="040d9-124">Read-only.</span></span>        |
| <span data-ttu-id="040d9-125">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="040d9-125">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="040d9-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="040d9-126">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="040d9-127">バージョンが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="040d9-127">Date and time the version was last modified.</span></span> <span data-ttu-id="040d9-128">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="040d9-128">Read-only.</span></span>                 |
| <span data-ttu-id="040d9-129">**published**</span><span class="sxs-lookup"><span data-stu-id="040d9-129">**published**</span></span>            | [<span data-ttu-id="040d9-130">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="040d9-130">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="040d9-131">特定のバージョンのパブリケーション ステータスを示します。</span><span class="sxs-lookup"><span data-stu-id="040d9-131">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="040d9-132">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="040d9-132">Read-only.</span></span> |


## <a name="relationships"></a><span data-ttu-id="040d9-133">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="040d9-133">Relationships</span></span>

<span data-ttu-id="040d9-134">次の表は、**driveItemVersion** リソースが他のリソースに対して持っているリレーションシップを定義しています。</span><span class="sxs-lookup"><span data-stu-id="040d9-134">The following table defines the relationships that the **driveItemVersion** resource has to other resources.</span></span>

| <span data-ttu-id="040d9-135">リレーションシップ名</span><span class="sxs-lookup"><span data-stu-id="040d9-135">Relationship name</span></span> |                      <span data-ttu-id="040d9-136">種類</span><span class="sxs-lookup"><span data-stu-id="040d9-136">Type</span></span>                      |                               <span data-ttu-id="040d9-137">説明</span><span class="sxs-lookup"><span data-stu-id="040d9-137">Description</span></span>                                |
| :---------------- | :--------------------------------------------- | :----------------------------------------------------------------------- |
| <span data-ttu-id="040d9-138">**fields**</span><span class="sxs-lookup"><span data-stu-id="040d9-138">**fields**</span></span>        | [<span data-ttu-id="040d9-139">FieldValueSet</span><span class="sxs-lookup"><span data-stu-id="040d9-139">FieldValueSet</span></span>](../resources/fieldvalueset.md) | <span data-ttu-id="040d9-140">このバージョンのリスト アイテムの、フィールドと値のコレクション。</span><span class="sxs-lookup"><span data-stu-id="040d9-140">A collection of the fields and values for this version of the list item.</span></span> |


<!-- {
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version"
} -->
