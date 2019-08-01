---
title: BaseItemVersion リソースの種類
description: '**baseItemVersion** リソースは、アイテムまたはエンティティの旧バージョンを表します。'
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 03b18712e62a37e546fb8f9e3d031eeedace0208
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033069"
---
# <a name="baseitemversion-resource-type"></a><span data-ttu-id="96b89-103">BaseItemVersion リソースの種類</span><span class="sxs-lookup"><span data-stu-id="96b89-103">BaseItemVersion resource type</span></span>

<span data-ttu-id="96b89-104">**baseItemVersion** リソースは、アイテムまたはエンティティの旧バージョンを表します。</span><span class="sxs-lookup"><span data-stu-id="96b89-104">The **baseItemVersion** resource represents a previous version of an item or entity.</span></span>


## <a name="json-representation"></a><span data-ttu-id="96b89-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="96b89-105">JSON representation</span></span>

<!--{
  "blockType": "resource",
  "abstract": true,
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.baseItemVersion",
  "@type.aka": "oneDrive.baseItemVersion"
}-->

```json
{
  "id": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "2016-01-01T15:20:01.125Z",
  "publication": { "@odata.type": "microsoft.graph.publicationFacet" }
}
```

## <a name="properties"></a><span data-ttu-id="96b89-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="96b89-106">Properties</span></span>

|      <span data-ttu-id="96b89-107">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="96b89-107">Property name</span></span>       |                         <span data-ttu-id="96b89-108">種類</span><span class="sxs-lookup"><span data-stu-id="96b89-108">Type</span></span>                         |                               <span data-ttu-id="96b89-109">説明</span><span class="sxs-lookup"><span data-stu-id="96b89-109">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="96b89-110">**id**</span><span class="sxs-lookup"><span data-stu-id="96b89-110">**id**</span></span>                   | <span data-ttu-id="96b89-111">string</span><span class="sxs-lookup"><span data-stu-id="96b89-111">string</span></span>                                               | <span data-ttu-id="96b89-112">バージョンの ID。</span><span class="sxs-lookup"><span data-stu-id="96b89-112">The ID of the version.</span></span> <span data-ttu-id="96b89-113">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="96b89-113">Read-only.</span></span>                                       |
| <span data-ttu-id="96b89-114">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="96b89-114">**lastModifiedBy**</span></span>       | [<span data-ttu-id="96b89-115">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="96b89-115">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="96b89-116">最後にバージョンを変更したユーザーの ID。</span><span class="sxs-lookup"><span data-stu-id="96b89-116">Identity of the user which last modified the version.</span></span> <span data-ttu-id="96b89-117">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="96b89-117">Read-only.</span></span>        |
| <span data-ttu-id="96b89-118">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="96b89-118">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="96b89-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="96b89-119">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="96b89-120">バージョンが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="96b89-120">Date and time the version was last modified.</span></span> <span data-ttu-id="96b89-121">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="96b89-121">Read-only.</span></span>                 |
| <span data-ttu-id="96b89-122">**publication**</span><span class="sxs-lookup"><span data-stu-id="96b89-122">**publication**</span></span>          | [<span data-ttu-id="96b89-123">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="96b89-123">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="96b89-124">特定のバージョンのパブリケーション ステータスを示します。</span><span class="sxs-lookup"><span data-stu-id="96b89-124">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="96b89-125">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="96b89-125">Read-only.</span></span> |


<!-- {
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version"
} -->
