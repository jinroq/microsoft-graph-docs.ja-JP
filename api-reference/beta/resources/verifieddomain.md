---
title: verifiedDomain リソースの種類
description: テナントのドメインを指定します。組織 エンティティの **VerifiedDomains** プロパティは、**VerifiedDomain** のコレクションです。
localization_priority: Normal
ms.openlocfilehash: 01e2d174f47d08bea4de9d582ffd6126002e8f1f
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576872"
---
# <a name="verifieddomain-resource-type"></a><span data-ttu-id="592fa-104">verifiedDomain リソースの種類</span><span class="sxs-lookup"><span data-stu-id="592fa-104">verifiedDomain resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="592fa-p102">テナントのドメインを指定します。[組織](organization.md) エンティティの **VerifiedDomains** プロパティは、**VerifiedDomain** のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="592fa-p102">Specifies a domain for a tenant. The **verifiedDomains** property of the [organization](organization.md) entity is a collection of **VerifiedDomain**.</span></span>


## <a name="properties"></a><span data-ttu-id="592fa-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="592fa-107">Properties</span></span>
| <span data-ttu-id="592fa-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="592fa-108">Property</span></span>     | <span data-ttu-id="592fa-109">型</span><span class="sxs-lookup"><span data-stu-id="592fa-109">Type</span></span>   |<span data-ttu-id="592fa-110">説明</span><span class="sxs-lookup"><span data-stu-id="592fa-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="592fa-111">capabilities</span><span class="sxs-lookup"><span data-stu-id="592fa-111">capabilities</span></span>|<span data-ttu-id="592fa-112">String</span><span class="sxs-lookup"><span data-stu-id="592fa-112">String</span></span>|<span data-ttu-id="592fa-113">「電子メール」、「OfficeCommunicationsOnline」など。</span><span class="sxs-lookup"><span data-stu-id="592fa-113">For example, “Email”, “OfficeCommunicationsOnline”.</span></span>|
|<span data-ttu-id="592fa-114">isDefault</span><span class="sxs-lookup"><span data-stu-id="592fa-114">isDefault</span></span>|<span data-ttu-id="592fa-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="592fa-115">Boolean</span></span>|                <span data-ttu-id="592fa-116">これがテナントに関連付けられている既定のドメインの場合は **true**、それ以外の場合は **false**。</span><span class="sxs-lookup"><span data-stu-id="592fa-116">**true** if this is the default domain associated with the tenant; otherwise, **false**.</span></span>            |
|<span data-ttu-id="592fa-117">isInitial</span><span class="sxs-lookup"><span data-stu-id="592fa-117">isInitial</span></span>|<span data-ttu-id="592fa-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="592fa-118">Boolean</span></span>|<span data-ttu-id="592fa-119">これがテナントに関連付けられている初期ドメインの場合は **true**、それ以外の場合は **false**。</span><span class="sxs-lookup"><span data-stu-id="592fa-119">**true** if this is the initial domain associated with the tenant; otherwise, **false**</span></span>|
|<span data-ttu-id="592fa-120">name</span><span class="sxs-lookup"><span data-stu-id="592fa-120">name</span></span>|<span data-ttu-id="592fa-121">String</span><span class="sxs-lookup"><span data-stu-id="592fa-121">String</span></span>|<span data-ttu-id="592fa-122">ドメイン名。「contoso.onmicrosoft.com」など。</span><span class="sxs-lookup"><span data-stu-id="592fa-122">The domain name; for example, “contoso.onmicrosoft.com”</span></span>|
|<span data-ttu-id="592fa-123">type</span><span class="sxs-lookup"><span data-stu-id="592fa-123">type</span></span>|<span data-ttu-id="592fa-124">String</span><span class="sxs-lookup"><span data-stu-id="592fa-124">String</span></span>|<span data-ttu-id="592fa-125">「管理対象」など。</span><span class="sxs-lookup"><span data-stu-id="592fa-125">For example, “Managed”.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="592fa-126">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="592fa-126">JSON representation</span></span>

<span data-ttu-id="592fa-127">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="592fa-127">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.verifiedDomain"
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
