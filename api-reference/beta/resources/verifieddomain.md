---
title: verifiedDomain リソースの種類
description: テナントのドメインを指定します。組織 エンティティの **VerifiedDomains** プロパティは、**VerifiedDomain** のコレクションです。
localization_priority: Normal
ms.openlocfilehash: c13c3b3da39b762c26d637deaddafbee5da40160
ms.sourcegitcommit: d95f6d39a0479da6e531f3734c4029dc596b9a3f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/30/2019
ms.locfileid: "29641324"
---
# <a name="verifieddomain-resource-type"></a><span data-ttu-id="21030-104">verifiedDomain リソースの種類</span><span class="sxs-lookup"><span data-stu-id="21030-104">verifiedDomain resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="21030-p102">テナントのドメインを指定します。[組織](organization.md) エンティティの **VerifiedDomains** プロパティは、**VerifiedDomain** のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="21030-p102">Specifies a domain for a tenant. The **verifiedDomains** property of the [organization](organization.md) entity is a collection of **VerifiedDomain**.</span></span>


## <a name="properties"></a><span data-ttu-id="21030-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="21030-107">Properties</span></span>
| <span data-ttu-id="21030-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="21030-108">Property</span></span>     | <span data-ttu-id="21030-109">型</span><span class="sxs-lookup"><span data-stu-id="21030-109">Type</span></span>   |<span data-ttu-id="21030-110">説明</span><span class="sxs-lookup"><span data-stu-id="21030-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="21030-111">capabilities</span><span class="sxs-lookup"><span data-stu-id="21030-111">capabilities</span></span>|<span data-ttu-id="21030-112">String</span><span class="sxs-lookup"><span data-stu-id="21030-112">String</span></span>|<span data-ttu-id="21030-113">「電子メール」、「OfficeCommunicationsOnline」など。</span><span class="sxs-lookup"><span data-stu-id="21030-113">For example, “Email”, “OfficeCommunicationsOnline”.</span></span>|
|<span data-ttu-id="21030-114">isDefault</span><span class="sxs-lookup"><span data-stu-id="21030-114">isDefault</span></span>|<span data-ttu-id="21030-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="21030-115">Boolean</span></span>|                <span data-ttu-id="21030-116">これがテナントに関連付けられている既定のドメインの場合は **true**、それ以外の場合は **false**。</span><span class="sxs-lookup"><span data-stu-id="21030-116">**true** if this is the default domain associated with the tenant; otherwise, **false**.</span></span>            |
|<span data-ttu-id="21030-117">isInitial</span><span class="sxs-lookup"><span data-stu-id="21030-117">isInitial</span></span>|<span data-ttu-id="21030-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="21030-118">Boolean</span></span>|<span data-ttu-id="21030-119">これがテナントに関連付けられている初期ドメインの場合は **true**、それ以外の場合は **false**。</span><span class="sxs-lookup"><span data-stu-id="21030-119">**true** if this is the initial domain associated with the tenant; otherwise, **false**</span></span>|
|<span data-ttu-id="21030-120">name</span><span class="sxs-lookup"><span data-stu-id="21030-120">name</span></span>|<span data-ttu-id="21030-121">String</span><span class="sxs-lookup"><span data-stu-id="21030-121">String</span></span>|<span data-ttu-id="21030-122">ドメイン名。「contoso.onmicrosoft.com」など。</span><span class="sxs-lookup"><span data-stu-id="21030-122">The domain name; for example, “contoso.onmicrosoft.com”</span></span>|
|<span data-ttu-id="21030-123">type</span><span class="sxs-lookup"><span data-stu-id="21030-123">type</span></span>|<span data-ttu-id="21030-124">String</span><span class="sxs-lookup"><span data-stu-id="21030-124">String</span></span>|<span data-ttu-id="21030-125">「管理対象」など。</span><span class="sxs-lookup"><span data-stu-id="21030-125">For example, “Managed”.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="21030-126">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="21030-126">JSON representation</span></span>

<span data-ttu-id="21030-127">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="21030-127">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.verifieddomain"
}-->

```json
{
  "capabilities": "string",
  "isDefault": true,
  "isInitial": true,
  "name": "string",
  "type": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "verifiedDomain resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/verifieddomain.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
