---
title: verifiedDomain リソースの種類
description: テナントのドメインを指定します。 組織エンティティの**verifiedDomains**プロパティは、 **VerifiedDomain**のコレクションです。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 091bb8e6c1a14f6c173d18acf68679feb6c88eaf
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964228"
---
# <a name="verifieddomain-resource-type"></a><span data-ttu-id="681df-104">verifiedDomain リソースの種類</span><span class="sxs-lookup"><span data-stu-id="681df-104">verifiedDomain resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="681df-105">テナントのドメインを指定します。</span><span class="sxs-lookup"><span data-stu-id="681df-105">Specifies a domain for a tenant.</span></span> <span data-ttu-id="681df-106">[組織](organization.md)エンティティの**verifiedDomains**プロパティは、 **VerifiedDomain**のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="681df-106">The **verifiedDomains** property of the [organization](organization.md) entity is a collection of **VerifiedDomain**.</span></span>


## <a name="properties"></a><span data-ttu-id="681df-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="681df-107">Properties</span></span>
| <span data-ttu-id="681df-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="681df-108">Property</span></span>     | <span data-ttu-id="681df-109">型</span><span class="sxs-lookup"><span data-stu-id="681df-109">Type</span></span>   |<span data-ttu-id="681df-110">説明</span><span class="sxs-lookup"><span data-stu-id="681df-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="681df-111">capabilities</span><span class="sxs-lookup"><span data-stu-id="681df-111">capabilities</span></span>|<span data-ttu-id="681df-112">String</span><span class="sxs-lookup"><span data-stu-id="681df-112">String</span></span>|<span data-ttu-id="681df-113">「電子メール」、「OfficeCommunicationsOnline」など。</span><span class="sxs-lookup"><span data-stu-id="681df-113">For example, “Email”, “OfficeCommunicationsOnline”.</span></span>|
|<span data-ttu-id="681df-114">isDefault</span><span class="sxs-lookup"><span data-stu-id="681df-114">isDefault</span></span>|<span data-ttu-id="681df-115">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="681df-115">Boolean</span></span>|                <span data-ttu-id="681df-116">これがテナントに関連付けられている既定のドメインの場合は **true**、それ以外の場合は **false**。</span><span class="sxs-lookup"><span data-stu-id="681df-116">**true** if this is the default domain associated with the tenant; otherwise, **false**.</span></span>            |
|<span data-ttu-id="681df-117">isInitial</span><span class="sxs-lookup"><span data-stu-id="681df-117">isInitial</span></span>|<span data-ttu-id="681df-118">ブール値</span><span class="sxs-lookup"><span data-stu-id="681df-118">Boolean</span></span>|<span data-ttu-id="681df-119">これがテナントに関連付けられている初期ドメインの場合は **true**、それ以外の場合は **false**。</span><span class="sxs-lookup"><span data-stu-id="681df-119">**true** if this is the initial domain associated with the tenant; otherwise, **false**</span></span>|
|<span data-ttu-id="681df-120">name</span><span class="sxs-lookup"><span data-stu-id="681df-120">name</span></span>|<span data-ttu-id="681df-121">String</span><span class="sxs-lookup"><span data-stu-id="681df-121">String</span></span>|<span data-ttu-id="681df-122">ドメイン名。「contoso.onmicrosoft.com」など。</span><span class="sxs-lookup"><span data-stu-id="681df-122">The domain name; for example, “contoso.onmicrosoft.com”</span></span>|
|<span data-ttu-id="681df-123">type</span><span class="sxs-lookup"><span data-stu-id="681df-123">type</span></span>|<span data-ttu-id="681df-124">String</span><span class="sxs-lookup"><span data-stu-id="681df-124">String</span></span>|<span data-ttu-id="681df-125">「管理対象」など。</span><span class="sxs-lookup"><span data-stu-id="681df-125">For example, “Managed”.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="681df-126">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="681df-126">JSON representation</span></span>

<span data-ttu-id="681df-127">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="681df-127">Here is a JSON representation of the resource</span></span>

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
