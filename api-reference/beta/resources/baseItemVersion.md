---
author: rgregg
ms.author: rgregg
ms.date: 09/17/2017
title: BaseItemVersion
ms.openlocfilehash: dfda19af6057bc1d6e1757d24f6a2c99979a8622
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066474"
---
# <a name="baseitemversion-resource-type"></a><span data-ttu-id="c1c48-102">BaseItemVersion リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c1c48-102">BaseItemVersion resource type</span></span>

> <span data-ttu-id="c1c48-103">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c1c48-103">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c1c48-104">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c1c48-104">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c1c48-105">**baseItemVersion** リソースは、アイテムまたはエンティティの旧バージョンを表します。</span><span class="sxs-lookup"><span data-stu-id="c1c48-105">The **baseItemVersion** resource represents a previous version of an item or entity.</span></span>


## <a name="json-representation"></a><span data-ttu-id="c1c48-106">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c1c48-106">JSON representation</span></span>

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

## <a name="properties"></a><span data-ttu-id="c1c48-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c1c48-107">Properties</span></span>

|      <span data-ttu-id="c1c48-108">プロパティ名</span><span class="sxs-lookup"><span data-stu-id="c1c48-108">Property name</span></span>       |                         <span data-ttu-id="c1c48-109">型</span><span class="sxs-lookup"><span data-stu-id="c1c48-109">Type</span></span>                         |                               <span data-ttu-id="c1c48-110">説明</span><span class="sxs-lookup"><span data-stu-id="c1c48-110">Description</span></span>                               |
| :----------------------- | :--------------------------------------------------- | :---------------------------------------------------------------------- |
| <span data-ttu-id="c1c48-111">**id**</span><span class="sxs-lookup"><span data-stu-id="c1c48-111">**id**</span></span>                   | <span data-ttu-id="c1c48-112">string</span><span class="sxs-lookup"><span data-stu-id="c1c48-112">string</span></span>                                               | <span data-ttu-id="c1c48-113">バージョンの ID。</span><span class="sxs-lookup"><span data-stu-id="c1c48-113">The ID of the version.</span></span> <span data-ttu-id="c1c48-114">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="c1c48-114">Read-only.</span></span>                                       |
| <span data-ttu-id="c1c48-115">**lastModifiedBy**</span><span class="sxs-lookup"><span data-stu-id="c1c48-115">**lastModifiedBy**</span></span>       | [<span data-ttu-id="c1c48-116">IdentitySet</span><span class="sxs-lookup"><span data-stu-id="c1c48-116">IdentitySet</span></span>](../resources/identityset.md)           | <span data-ttu-id="c1c48-117">最後にバージョンを変更したユーザーの ID。</span><span class="sxs-lookup"><span data-stu-id="c1c48-117">Identity of the user which last modified the version.</span></span> <span data-ttu-id="c1c48-118">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="c1c48-118">Read-only.</span></span>        |
| <span data-ttu-id="c1c48-119">**lastModifiedDateTime**</span><span class="sxs-lookup"><span data-stu-id="c1c48-119">**lastModifiedDateTime**</span></span> | [<span data-ttu-id="c1c48-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c1c48-120">DateTimeOffset</span></span>](../resources/timestamp.md)          | <span data-ttu-id="c1c48-121">バージョンが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="c1c48-121">Date and time the version was last modified.</span></span> <span data-ttu-id="c1c48-122">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="c1c48-122">Read-only.</span></span>                 |
| <span data-ttu-id="c1c48-123">**publication**</span><span class="sxs-lookup"><span data-stu-id="c1c48-123">**publication**</span></span>          | [<span data-ttu-id="c1c48-124">PublicationFacet</span><span class="sxs-lookup"><span data-stu-id="c1c48-124">PublicationFacet</span></span>](../resources/publicationfacet.md) | <span data-ttu-id="c1c48-125">特定のバージョンのパブリケーション ステータスを示します。</span><span class="sxs-lookup"><span data-stu-id="c1c48-125">Indicates the publication status of this particular version.</span></span> <span data-ttu-id="c1c48-126">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="c1c48-126">Read-only.</span></span> |


<!-- {
  "type": "#page.annotation",
  "description": "The version facet provides information about the properties of a file version.",
  "keywords": "version,versions,version-history,history",
  "section": "documentation",
  "tocPath": "Facets/Version"
} -->