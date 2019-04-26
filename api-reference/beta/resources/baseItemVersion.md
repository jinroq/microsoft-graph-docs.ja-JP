---
author: JeremyKelley
ms.author: JeremyKelley
ms.date: 09/17/2017
title: BaseItemVersion
localization_priority: Normal
ms.openlocfilehash: 735931e757297bd9846396d6f6c42988d8cb87fa
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33328245"
---
# <a name="baseitemversion-resource-type"></a><span data-ttu-id="8ce22-102">BaseItemVersion リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8ce22-102">BaseItemVersion resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8ce22-103">**baseItemVersion** リソースは、アイテムまたはエンティティの旧バージョンを表します。</span><span class="sxs-lookup"><span data-stu-id="8ce22-103">The **baseItemVersion** resource represents a previous version of an item or entity.</span></span>


## <a name="json-representation"></a><span data-ttu-id="8ce22-104">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8ce22-104">JSON representation</span></span>

<!-- { "blockType": "resource", "@odata.type": "microsoft.graph.baseItemVersion", "@type.aka": "oneDrive.baseItemVersion" } -->

```json
{
  "content": { "@odata.type": "Edm.Stream" },
  "id": "string",
  "lastModifiedBy": { "@odata.type": "microsoft.graph.identitySet" },
  "lastModifiedDateTime": "2016-01-01T15:20:01.125Z",
  "publication": { "@odata.type": "microsoft.graph.publicationFacet" }
}
```

## <a name="properties"></a><span data-ttu-id="8ce22-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8ce22-105">Properties</span></span>

|      <span data-ttu-id="8ce22-106">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="8ce22-106">Property name</span></span>       |                         <span data-ttu-id="8ce22-107">種類</span><span class="sxs-lookup"><span data-stu-id="8ce22-107">Type</span></span>                         |                               <span data-ttu-id="8ce22-108">説明</span><span class="sxs-lookup"><span data-stu-id="8ce22-108">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="8ce22-109">**id**</span><span class="sxs-lookup"><span data-stu-id="8ce22-109">**id**</span></span>                   | <span data-ttu-id="8ce22-110">string</span><span class="sxs-lookup"><span data-stu-id="8ce22-110">string</span></span>                                               | <span data-ttu-id="8ce22-111">バージョンの ID。</span><span class="sxs-lookup"><span data-stu-id="8ce22-111">The ID of the version.</span></span> <span data-ttu-id="8ce22-112">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="8ce22-112">Read-only.</span></span>                                       |
| <span data-ttu-id="8ce22-113">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="8ce22-113">**lastModifiedBy**</span></span>       | [<span data-ttu-id="8ce22-114">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="8ce22-114">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="8ce22-115">最後にバージョンを変更したユーザーの ID。</span><span class="sxs-lookup"><span data-stu-id="8ce22-115">Identity of the user which last modified the version.</span></span> <span data-ttu-id="8ce22-116">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="8ce22-116">Read-only.</span></span>        |
| <span data-ttu-id="8ce22-117">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="8ce22-117">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="8ce22-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8ce22-118">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="8ce22-119">バージョンが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="8ce22-119">Date and time the version was last modified.</span></span> <span data-ttu-id="8ce22-120">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="8ce22-120">Read-only.</span></span>                 |
| <span data-ttu-id="8ce22-121">**publication**</span><span class="sxs-lookup"><span data-stu-id="8ce22-121">**publication**</span></span>          | [<span data-ttu-id="8ce22-122">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="8ce22-122">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="8ce22-123">特定のバージョンのパブリケーション ステータスを示します。</span><span class="sxs-lookup"><span data-stu-id="8ce22-123">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="8ce22-124">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="8ce22-124">Read-only.</span></span> |


<!--
{
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version",
  "suppressions": []
}
-->
