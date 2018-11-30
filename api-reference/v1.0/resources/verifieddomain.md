---
title: verifiedDomain リソースの種類
description: テナントのドメインを指定します。組織 エンティティの **VerifiedDomains** プロパティは、**VerifiedDomain** のコレクションです。
ms.openlocfilehash: 21b6dd89dcc8b990046952d9ae7abcfe8ce02bca
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27021563"
---
# <a name="verifieddomain-resource-type"></a><span data-ttu-id="60dfe-104">verifiedDomain リソースの種類</span><span class="sxs-lookup"><span data-stu-id="60dfe-104">verifiedDomain resource type</span></span>

<span data-ttu-id="60dfe-p102">テナントのドメインを指定します。[組織](organization.md) エンティティの **VerifiedDomains** プロパティは、**VerifiedDomain** のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="60dfe-p102">Specifies a domain for a tenant. The **verifiedDomains** property of the [organization](organization.md) entity is a collection of **VerifiedDomain**.</span></span>


## <a name="properties"></a><span data-ttu-id="60dfe-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="60dfe-107">Properties</span></span>
| <span data-ttu-id="60dfe-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="60dfe-108">Property</span></span>     | <span data-ttu-id="60dfe-109">型</span><span class="sxs-lookup"><span data-stu-id="60dfe-109">Type</span></span>   |<span data-ttu-id="60dfe-110">説明</span><span class="sxs-lookup"><span data-stu-id="60dfe-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="60dfe-111">capabilities</span><span class="sxs-lookup"><span data-stu-id="60dfe-111">capabilities</span></span>|<span data-ttu-id="60dfe-112">String</span><span class="sxs-lookup"><span data-stu-id="60dfe-112">String</span></span>|<span data-ttu-id="60dfe-113">「電子メール」、「OfficeCommunicationsOnline」など。</span><span class="sxs-lookup"><span data-stu-id="60dfe-113">For example, “Email”, “OfficeCommunicationsOnline”.</span></span>|
|<span data-ttu-id="60dfe-114">isDefault</span><span class="sxs-lookup"><span data-stu-id="60dfe-114">isDefault</span></span>|<span data-ttu-id="60dfe-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="60dfe-115">Boolean</span></span>|                <span data-ttu-id="60dfe-116">これがテナントに関連付けられている既定のドメインの場合は **true**、それ以外の場合は **false**。</span><span class="sxs-lookup"><span data-stu-id="60dfe-116">**true** if this is the default domain associated with the tenant; otherwise, **false**.</span></span>            |
|<span data-ttu-id="60dfe-117">isInitial</span><span class="sxs-lookup"><span data-stu-id="60dfe-117">isInitial</span></span>|<span data-ttu-id="60dfe-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="60dfe-118">Boolean</span></span>|<span data-ttu-id="60dfe-119">これがテナントに関連付けられている初期ドメインの場合は **true**、それ以外の場合は **false**。</span><span class="sxs-lookup"><span data-stu-id="60dfe-119">**true** if this is the initial domain associated with the tenant; otherwise, **false**</span></span>|
|<span data-ttu-id="60dfe-120">name</span><span class="sxs-lookup"><span data-stu-id="60dfe-120">name</span></span>|<span data-ttu-id="60dfe-121">String</span><span class="sxs-lookup"><span data-stu-id="60dfe-121">String</span></span>|<span data-ttu-id="60dfe-122">ドメイン名。「contoso.onmicrosoft.com」など。</span><span class="sxs-lookup"><span data-stu-id="60dfe-122">The domain name; for example, “contoso.onmicrosoft.com”</span></span>|
|<span data-ttu-id="60dfe-123">type</span><span class="sxs-lookup"><span data-stu-id="60dfe-123">type</span></span>|<span data-ttu-id="60dfe-124">String</span><span class="sxs-lookup"><span data-stu-id="60dfe-124">String</span></span>|<span data-ttu-id="60dfe-125">「管理対象」など。</span><span class="sxs-lookup"><span data-stu-id="60dfe-125">For example, “Managed”.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="60dfe-126">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="60dfe-126">JSON representation</span></span>

<span data-ttu-id="60dfe-127">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="60dfe-127">Here is a JSON representation of the resource</span></span>

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
