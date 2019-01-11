---
title: BaseItemVersion リソースの種類
description: '**baseItemVersion** リソースは、アイテムまたはエンティティの旧バージョンを表します。'
localization_priority: Normal
ms.openlocfilehash: bd28f9c8dc5be2bc6422aca2eb756aba78b8e393
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876966"
---
# <a name="baseitemversion-resource-type"></a><span data-ttu-id="b2e53-103">BaseItemVersion リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b2e53-103">BaseItemVersion resource type</span></span>

<span data-ttu-id="b2e53-104">**baseItemVersion** リソースは、アイテムまたはエンティティの旧バージョンを表します。</span><span class="sxs-lookup"><span data-stu-id="b2e53-104">The **baseItemVersion** resource represents a previous version of an item or entity.</span></span>


## <a name="json-representation"></a><span data-ttu-id="b2e53-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b2e53-105">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="b2e53-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b2e53-106">Properties</span></span>

|      <span data-ttu-id="b2e53-107">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="b2e53-107">Property name</span></span>       |                         <span data-ttu-id="b2e53-108">Type</span><span class="sxs-lookup"><span data-stu-id="b2e53-108">Type</span></span>                         |                               <span data-ttu-id="b2e53-109">説明</span><span class="sxs-lookup"><span data-stu-id="b2e53-109">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="b2e53-110">**id**</span><span class="sxs-lookup"><span data-stu-id="b2e53-110">**id**</span></span>                   | <span data-ttu-id="b2e53-111">string</span><span class="sxs-lookup"><span data-stu-id="b2e53-111">string</span></span>                                               | <span data-ttu-id="b2e53-112">バージョンの ID。</span><span class="sxs-lookup"><span data-stu-id="b2e53-112">The ID of the version.</span></span> <span data-ttu-id="b2e53-113">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b2e53-113">Read-only.</span></span>                                       |
| <span data-ttu-id="b2e53-114">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="b2e53-114">**lastModifiedBy**</span></span>       | [<span data-ttu-id="b2e53-115">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="b2e53-115">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="b2e53-116">最後にバージョンを変更したユーザーの ID。</span><span class="sxs-lookup"><span data-stu-id="b2e53-116">Identity of the user which last modified the version.</span></span> <span data-ttu-id="b2e53-117">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b2e53-117">Read-only.</span></span>        |
| <span data-ttu-id="b2e53-118">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="b2e53-118">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="b2e53-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b2e53-119">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="b2e53-120">バージョンが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="b2e53-120">Date and time the version was last modified.</span></span> <span data-ttu-id="b2e53-121">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b2e53-121">Read-only.</span></span>                 |
| <span data-ttu-id="b2e53-122">**publication**</span><span class="sxs-lookup"><span data-stu-id="b2e53-122">**publication**</span></span>          | [<span data-ttu-id="b2e53-123">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="b2e53-123">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="b2e53-124">特定のバージョンのパブリケーション ステータスを示します。</span><span class="sxs-lookup"><span data-stu-id="b2e53-124">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="b2e53-125">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="b2e53-125">Read-only.</span></span> |


<!-- {
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version"
} -->
