---
title: verifiedDomain リソースの種類
description: テナントのドメインを指定します。組織 エンティティの **VerifiedDomains** プロパティは、**VerifiedDomain** のコレクションです。
localization_priority: Normal
ms.openlocfilehash: 6eb6490ce8dac29f2617b7873230fad7c7b5c536
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876497"
---
# <a name="verifieddomain-resource-type"></a><span data-ttu-id="671d7-104">verifiedDomain リソースの種類</span><span class="sxs-lookup"><span data-stu-id="671d7-104">verifiedDomain resource type</span></span>

<span data-ttu-id="671d7-p102">テナントのドメインを指定します。[組織](organization.md) エンティティの **VerifiedDomains** プロパティは、**VerifiedDomain** のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="671d7-p102">Specifies a domain for a tenant. The **verifiedDomains** property of the [organization](organization.md) entity is a collection of **VerifiedDomain**.</span></span>


## <a name="properties"></a><span data-ttu-id="671d7-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="671d7-107">Properties</span></span>
| <span data-ttu-id="671d7-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="671d7-108">Property</span></span>     | <span data-ttu-id="671d7-109">種類</span><span class="sxs-lookup"><span data-stu-id="671d7-109">Type</span></span>   |<span data-ttu-id="671d7-110">説明</span><span class="sxs-lookup"><span data-stu-id="671d7-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="671d7-111">capabilities</span><span class="sxs-lookup"><span data-stu-id="671d7-111">capabilities</span></span>|<span data-ttu-id="671d7-112">String</span><span class="sxs-lookup"><span data-stu-id="671d7-112">String</span></span>|<span data-ttu-id="671d7-113">「電子メール」、「OfficeCommunicationsOnline」など。</span><span class="sxs-lookup"><span data-stu-id="671d7-113">For example, “Email”, “OfficeCommunicationsOnline”.</span></span>|
|<span data-ttu-id="671d7-114">isDefault</span><span class="sxs-lookup"><span data-stu-id="671d7-114">isDefault</span></span>|<span data-ttu-id="671d7-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="671d7-115">Boolean</span></span>|                <span data-ttu-id="671d7-116">これがテナントに関連付けられている既定のドメインの場合は **true**、それ以外の場合は **false**。</span><span class="sxs-lookup"><span data-stu-id="671d7-116">**true** if this is the default domain associated with the tenant; otherwise, **false**.</span></span>            |
|<span data-ttu-id="671d7-117">isInitial</span><span class="sxs-lookup"><span data-stu-id="671d7-117">isInitial</span></span>|<span data-ttu-id="671d7-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="671d7-118">Boolean</span></span>|<span data-ttu-id="671d7-119">これがテナントに関連付けられている初期ドメインの場合は **true**、それ以外の場合は **false**。</span><span class="sxs-lookup"><span data-stu-id="671d7-119">**true** if this is the initial domain associated with the tenant; otherwise, **false**</span></span>|
|<span data-ttu-id="671d7-120">name</span><span class="sxs-lookup"><span data-stu-id="671d7-120">name</span></span>|<span data-ttu-id="671d7-121">String</span><span class="sxs-lookup"><span data-stu-id="671d7-121">String</span></span>|<span data-ttu-id="671d7-122">ドメイン名。「contoso.onmicrosoft.com」など。</span><span class="sxs-lookup"><span data-stu-id="671d7-122">The domain name; for example, “contoso.onmicrosoft.com”</span></span>|
|<span data-ttu-id="671d7-123">type</span><span class="sxs-lookup"><span data-stu-id="671d7-123">type</span></span>|<span data-ttu-id="671d7-124">String</span><span class="sxs-lookup"><span data-stu-id="671d7-124">String</span></span>|<span data-ttu-id="671d7-125">「管理対象」など。</span><span class="sxs-lookup"><span data-stu-id="671d7-125">For example, “Managed”.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="671d7-126">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="671d7-126">JSON representation</span></span>

<span data-ttu-id="671d7-127">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="671d7-127">Here is a JSON representation of the resource</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "verifiedDomain resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
