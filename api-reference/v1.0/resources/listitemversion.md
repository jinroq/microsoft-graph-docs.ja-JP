---
title: ListItemVersion リソースの種類
description: '**listItemVersion** リソースは、ListItem リソースの旧バージョンを表しています。'
localization_priority: Normal
ms.prod: sharepoint
ms.openlocfilehash: 6e21be59b71a8f348931603c799ebbbe225e5d3f
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27951846"
---
# <a name="listitemversion-resource-type"></a><span data-ttu-id="fd612-103">ListItemVersion リソースの種類</span><span class="sxs-lookup"><span data-stu-id="fd612-103">ListItemVersion resource type</span></span>

<span data-ttu-id="fd612-104">**listItemVersion** リソースは、[ListItem](listitem.md) リソースの旧バージョンを表しています。</span><span class="sxs-lookup"><span data-stu-id="fd612-104">The **listItemVersion** resource represents a previous version of a [ListItem](listitem.md) resource.</span></span>

## <a name="tasks-on-listitemversion-resources"></a><span data-ttu-id="fd612-105">ListItemVersion リソースのタスク</span><span class="sxs-lookup"><span data-stu-id="fd612-105">Tasks on ListItemVersion resources</span></span>

<span data-ttu-id="fd612-106">listItemVersion リソースで使用可能なタスクを次に示します。</span><span class="sxs-lookup"><span data-stu-id="fd612-106">The following tasks are available for listItemVersion resources.</span></span>

|            <span data-ttu-id="fd612-107">共通タスク</span><span class="sxs-lookup"><span data-stu-id="fd612-107">Common task</span></span>             |         <span data-ttu-id="fd612-108">HTTP メソッド</span><span class="sxs-lookup"><span data-stu-id="fd612-108">HTTP method</span></span>         |
| :--------------------------------- | :-------------------------- |
| <span data-ttu-id="fd612-109">[バージョンの一覧表示][version-list]</span><span class="sxs-lookup"><span data-stu-id="fd612-109">[List versions][version-list]</span></span>      | `GET /sites/{site-id}/items/{item-id}/versions`  |
| <span data-ttu-id="fd612-110">[バージョンの取得][version-get]</span><span class="sxs-lookup"><span data-stu-id="fd612-110">[Get version][version-get]</span></span>         | `GET /sites/{site-id}/items/{item-id}/versions/{version-id}`     |
| <span data-ttu-id="fd612-111">[バージョンの復元][version-restore]</span><span class="sxs-lookup"><span data-stu-id="fd612-111">[Restore version][version-restore]</span></span> | `POST /sites/{site-id}/items/{item-id}/versions/{version-id}/restore` |

[version-list]: ../api/listitem-list-versions.md
[version-get]: ../api/listitemversion-get.md
[version-restore]: ../api/listitemversion-restore.md


## <a name="json-representation"></a><span data-ttu-id="fd612-112">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="fd612-112">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="fd612-113">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fd612-113">Properties</span></span>

|      <span data-ttu-id="fd612-114">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="fd612-114">Property name</span></span>       |                         <span data-ttu-id="fd612-115">Type</span><span class="sxs-lookup"><span data-stu-id="fd612-115">Type</span></span>                         |                               <span data-ttu-id="fd612-116">説明</span><span class="sxs-lookup"><span data-stu-id="fd612-116">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="fd612-117">**id**</span><span class="sxs-lookup"><span data-stu-id="fd612-117">**id**</span></span>                   | <span data-ttu-id="fd612-118">string</span><span class="sxs-lookup"><span data-stu-id="fd612-118">string</span></span>                                               | <span data-ttu-id="fd612-119">バージョンの ID。</span><span class="sxs-lookup"><span data-stu-id="fd612-119">The ID of the version.</span></span> <span data-ttu-id="fd612-120">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="fd612-120">Read-only.</span></span>                                       |
| <span data-ttu-id="fd612-121">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="fd612-121">**lastModifiedBy**</span></span>       | [<span data-ttu-id="fd612-122">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="fd612-122">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="fd612-123">最後にバージョンを変更したユーザーの ID。</span><span class="sxs-lookup"><span data-stu-id="fd612-123">Identity of the user which last modified the version.</span></span> <span data-ttu-id="fd612-124">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="fd612-124">Read-only.</span></span>        |
| <span data-ttu-id="fd612-125">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="fd612-125">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="fd612-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fd612-126">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="fd612-127">バージョンが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="fd612-127">Date and time the version was last modified.</span></span> <span data-ttu-id="fd612-128">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="fd612-128">Read-only.</span></span>                 |
| <span data-ttu-id="fd612-129">**published**</span><span class="sxs-lookup"><span data-stu-id="fd612-129">**published**</span></span>            | [<span data-ttu-id="fd612-130">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="fd612-130">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="fd612-131">特定のバージョンのパブリケーション ステータスを示します。</span><span class="sxs-lookup"><span data-stu-id="fd612-131">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="fd612-132">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="fd612-132">Read-only.</span></span> |


## <a name="relationships"></a><span data-ttu-id="fd612-133">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="fd612-133">Relationships</span></span>

<span data-ttu-id="fd612-134">次の表は、**driveItemVersion** リソースが他のリソースに対して持っているリレーションシップを定義しています。</span><span class="sxs-lookup"><span data-stu-id="fd612-134">The following table defines the relationships that the **driveItemVersion** resource has to other resources.</span></span>

| <span data-ttu-id="fd612-135">リレーションシップ名</span><span class="sxs-lookup"><span data-stu-id="fd612-135">Relationship name</span></span> |                      <span data-ttu-id="fd612-136">種類</span><span class="sxs-lookup"><span data-stu-id="fd612-136">Type</span></span>                      |                               <span data-ttu-id="fd612-137">説明</span><span class="sxs-lookup"><span data-stu-id="fd612-137">Description</span></span>                                |
| :---------------- | :--------------------------------------------- | :----------------------------------------------------------------------- |
| <span data-ttu-id="fd612-138">**fields**</span><span class="sxs-lookup"><span data-stu-id="fd612-138">**fields**</span></span>        | [<span data-ttu-id="fd612-139">FieldValueSet</span><span class="sxs-lookup"><span data-stu-id="fd612-139">FieldValueSet</span></span>](../resources/fieldvalueset.md) | <span data-ttu-id="fd612-140">このバージョンのリスト アイテムの、フィールドと値のコレクション。</span><span class="sxs-lookup"><span data-stu-id="fd612-140">A collection of the fields and values for this version of the list item.</span></span> |


<!-- {
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version"
} -->
