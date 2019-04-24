---
title: verifiedDomain リソースの種類
description: テナントのドメインを指定します。 組織エンティティの**verifiedDomains**プロパティは、 **VerifiedDomain**のコレクションです。
localization_priority: Normal
ms.openlocfilehash: 6eb6490ce8dac29f2617b7873230fad7c7b5c536
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32456907"
---
# <a name="verifieddomain-resource-type"></a><span data-ttu-id="50c1c-104">verifiedDomain リソースの種類</span><span class="sxs-lookup"><span data-stu-id="50c1c-104">verifiedDomain resource type</span></span>

<span data-ttu-id="50c1c-105">テナントのドメインを指定します。</span><span class="sxs-lookup"><span data-stu-id="50c1c-105">Specifies a domain for a tenant.</span></span> <span data-ttu-id="50c1c-106">[組織](organization.md)エンティティの**verifiedDomains**プロパティは、 **VerifiedDomain**のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="50c1c-106">The **verifiedDomains** property of the [organization](organization.md) entity is a collection of **VerifiedDomain**.</span></span>


## <a name="properties"></a><span data-ttu-id="50c1c-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="50c1c-107">Properties</span></span>
| <span data-ttu-id="50c1c-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="50c1c-108">Property</span></span>     | <span data-ttu-id="50c1c-109">型</span><span class="sxs-lookup"><span data-stu-id="50c1c-109">Type</span></span>   |<span data-ttu-id="50c1c-110">説明</span><span class="sxs-lookup"><span data-stu-id="50c1c-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="50c1c-111">capabilities</span><span class="sxs-lookup"><span data-stu-id="50c1c-111">capabilities</span></span>|<span data-ttu-id="50c1c-112">String</span><span class="sxs-lookup"><span data-stu-id="50c1c-112">String</span></span>|<span data-ttu-id="50c1c-113">「電子メール」、「OfficeCommunicationsOnline」など。</span><span class="sxs-lookup"><span data-stu-id="50c1c-113">For example, “Email”, “OfficeCommunicationsOnline”.</span></span>|
|<span data-ttu-id="50c1c-114">isDefault</span><span class="sxs-lookup"><span data-stu-id="50c1c-114">isDefault</span></span>|<span data-ttu-id="50c1c-115">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="50c1c-115">Boolean</span></span>|                <span data-ttu-id="50c1c-116">これがテナントに関連付けられている既定のドメインの場合は **true**、それ以外の場合は **false**。</span><span class="sxs-lookup"><span data-stu-id="50c1c-116">**true** if this is the default domain associated with the tenant; otherwise, **false**.</span></span>            |
|<span data-ttu-id="50c1c-117">isinitial</span><span class="sxs-lookup"><span data-stu-id="50c1c-117">isInitial</span></span>|<span data-ttu-id="50c1c-118">ブール値</span><span class="sxs-lookup"><span data-stu-id="50c1c-118">Boolean</span></span>|<span data-ttu-id="50c1c-119">これがテナントに関連付けられている初期ドメインの場合は **true**、それ以外の場合は **false**。</span><span class="sxs-lookup"><span data-stu-id="50c1c-119">**true** if this is the initial domain associated with the tenant; otherwise, **false**</span></span>|
|<span data-ttu-id="50c1c-120">name</span><span class="sxs-lookup"><span data-stu-id="50c1c-120">name</span></span>|<span data-ttu-id="50c1c-121">String</span><span class="sxs-lookup"><span data-stu-id="50c1c-121">String</span></span>|<span data-ttu-id="50c1c-122">ドメイン名。「contoso.onmicrosoft.com」など。</span><span class="sxs-lookup"><span data-stu-id="50c1c-122">The domain name; for example, “contoso.onmicrosoft.com”</span></span>|
|<span data-ttu-id="50c1c-123">type</span><span class="sxs-lookup"><span data-stu-id="50c1c-123">type</span></span>|<span data-ttu-id="50c1c-124">String</span><span class="sxs-lookup"><span data-stu-id="50c1c-124">String</span></span>|<span data-ttu-id="50c1c-125">「管理対象」など。</span><span class="sxs-lookup"><span data-stu-id="50c1c-125">For example, “Managed”.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="50c1c-126">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="50c1c-126">JSON representation</span></span>

<span data-ttu-id="50c1c-127">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="50c1c-127">Here is a JSON representation of the resource</span></span>

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
