---
title: verifiedDomain リソースの種類
description: テナントのドメインを指定します。 組織エンティティの**verifiedDomains**プロパティは、 **VerifiedDomain**のコレクションです。
localization_priority: Normal
ms.openlocfilehash: 088687d4450a5134c53bca6134039f7ba34a7597
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345097"
---
# <a name="verifieddomain-resource-type"></a><span data-ttu-id="49cba-104">verifiedDomain リソースの種類</span><span class="sxs-lookup"><span data-stu-id="49cba-104">verifiedDomain resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="49cba-105">テナントのドメインを指定します。</span><span class="sxs-lookup"><span data-stu-id="49cba-105">Specifies a domain for a tenant.</span></span> <span data-ttu-id="49cba-106">[組織](organization.md)エンティティの**verifiedDomains**プロパティは、 **VerifiedDomain**のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="49cba-106">The **verifiedDomains** property of the [organization](organization.md) entity is a collection of **VerifiedDomain**.</span></span>


## <a name="properties"></a><span data-ttu-id="49cba-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="49cba-107">Properties</span></span>
| <span data-ttu-id="49cba-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="49cba-108">Property</span></span>     | <span data-ttu-id="49cba-109">型</span><span class="sxs-lookup"><span data-stu-id="49cba-109">Type</span></span>   |<span data-ttu-id="49cba-110">説明</span><span class="sxs-lookup"><span data-stu-id="49cba-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="49cba-111">capabilities</span><span class="sxs-lookup"><span data-stu-id="49cba-111">capabilities</span></span>|<span data-ttu-id="49cba-112">String</span><span class="sxs-lookup"><span data-stu-id="49cba-112">String</span></span>|<span data-ttu-id="49cba-113">「電子メール」、「OfficeCommunicationsOnline」など。</span><span class="sxs-lookup"><span data-stu-id="49cba-113">For example, “Email”, “OfficeCommunicationsOnline”.</span></span>|
|<span data-ttu-id="49cba-114">isDefault</span><span class="sxs-lookup"><span data-stu-id="49cba-114">isDefault</span></span>|<span data-ttu-id="49cba-115">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="49cba-115">Boolean</span></span>|                <span data-ttu-id="49cba-116">これがテナントに関連付けられている既定のドメインの場合は **true**、それ以外の場合は **false**。</span><span class="sxs-lookup"><span data-stu-id="49cba-116">**true** if this is the default domain associated with the tenant; otherwise, **false**.</span></span>            |
|<span data-ttu-id="49cba-117">isinitial</span><span class="sxs-lookup"><span data-stu-id="49cba-117">isInitial</span></span>|<span data-ttu-id="49cba-118">ブール値</span><span class="sxs-lookup"><span data-stu-id="49cba-118">Boolean</span></span>|<span data-ttu-id="49cba-119">これがテナントに関連付けられている初期ドメインの場合は **true**、それ以外の場合は **false**。</span><span class="sxs-lookup"><span data-stu-id="49cba-119">**true** if this is the initial domain associated with the tenant; otherwise, **false**</span></span>|
|<span data-ttu-id="49cba-120">name</span><span class="sxs-lookup"><span data-stu-id="49cba-120">name</span></span>|<span data-ttu-id="49cba-121">String</span><span class="sxs-lookup"><span data-stu-id="49cba-121">String</span></span>|<span data-ttu-id="49cba-122">ドメイン名。「contoso.onmicrosoft.com」など。</span><span class="sxs-lookup"><span data-stu-id="49cba-122">The domain name; for example, “contoso.onmicrosoft.com”</span></span>|
|<span data-ttu-id="49cba-123">type</span><span class="sxs-lookup"><span data-stu-id="49cba-123">type</span></span>|<span data-ttu-id="49cba-124">String</span><span class="sxs-lookup"><span data-stu-id="49cba-124">String</span></span>|<span data-ttu-id="49cba-125">「管理対象」など。</span><span class="sxs-lookup"><span data-stu-id="49cba-125">For example, “Managed”.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="49cba-126">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="49cba-126">JSON representation</span></span>

<span data-ttu-id="49cba-127">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="49cba-127">Here is a JSON representation of the resource</span></span>

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
  "suppressions": []
}
-->
