---
title: BaseItemVersion リソースの種類
description: '**baseItemVersion** リソースは、アイテムまたはエンティティの旧バージョンを表します。'
ms.openlocfilehash: c4fc95fd419bf8b2f20ab202874ca31a2b1d63f6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27021696"
---
# <a name="baseitemversion-resource-type"></a><span data-ttu-id="23afa-103">BaseItemVersion リソースの種類</span><span class="sxs-lookup"><span data-stu-id="23afa-103">BaseItemVersion resource type</span></span>

<span data-ttu-id="23afa-104">**baseItemVersion** リソースは、アイテムまたはエンティティの旧バージョンを表します。</span><span class="sxs-lookup"><span data-stu-id="23afa-104">The **baseItemVersion** resource represents a previous version of an item or entity.</span></span>


## <a name="json-representation"></a><span data-ttu-id="23afa-105">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="23afa-105">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="23afa-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="23afa-106">Properties</span></span>

|      <span data-ttu-id="23afa-107">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="23afa-107">Property name</span></span>       |                         <span data-ttu-id="23afa-108">型</span><span class="sxs-lookup"><span data-stu-id="23afa-108">Type</span></span>                         |                               <span data-ttu-id="23afa-109">説明</span><span class="sxs-lookup"><span data-stu-id="23afa-109">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="23afa-110">**id**</span><span class="sxs-lookup"><span data-stu-id="23afa-110">**id**</span></span>                   | <span data-ttu-id="23afa-111">string</span><span class="sxs-lookup"><span data-stu-id="23afa-111">string</span></span>                                               | <span data-ttu-id="23afa-112">バージョンの ID。</span><span class="sxs-lookup"><span data-stu-id="23afa-112">The ID of the version.</span></span> <span data-ttu-id="23afa-113">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="23afa-113">Read-only.</span></span>                                       |
| <span data-ttu-id="23afa-114">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="23afa-114">**lastModifiedBy**</span></span>       | [<span data-ttu-id="23afa-115">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="23afa-115">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="23afa-116">最後にバージョンを変更したユーザーの ID。</span><span class="sxs-lookup"><span data-stu-id="23afa-116">Identity of the user which last modified the version.</span></span> <span data-ttu-id="23afa-117">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="23afa-117">Read-only.</span></span>        |
| <span data-ttu-id="23afa-118">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="23afa-118">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="23afa-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="23afa-119">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="23afa-120">バージョンが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="23afa-120">Date and time the version was last modified.</span></span> <span data-ttu-id="23afa-121">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="23afa-121">Read-only.</span></span>                 |
| <span data-ttu-id="23afa-122">**publication**</span><span class="sxs-lookup"><span data-stu-id="23afa-122">**publication**</span></span>          | [<span data-ttu-id="23afa-123">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="23afa-123">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="23afa-124">特定のバージョンのパブリケーション ステータスを示します。</span><span class="sxs-lookup"><span data-stu-id="23afa-124">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="23afa-125">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="23afa-125">Read-only.</span></span> |


<!-- {
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version"
} -->
