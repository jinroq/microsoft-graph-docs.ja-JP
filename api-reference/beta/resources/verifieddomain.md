---
title: verifiedDomain リソースの種類
description: テナントのドメインを指定します。組織 エンティティの **VerifiedDomains** プロパティは、**VerifiedDomain** のコレクションです。
localization_priority: Normal
ms.openlocfilehash: d912103f95677491d88bcb3f0b556bb1678c3049
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27810445"
---
# <a name="verifieddomain-resource-type"></a><span data-ttu-id="cb624-104">verifiedDomain リソースの種類</span><span class="sxs-lookup"><span data-stu-id="cb624-104">verifiedDomain resource type</span></span>

> <span data-ttu-id="cb624-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="cb624-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cb624-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cb624-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cb624-p103">テナントのドメインを指定します。[組織](organization.md) エンティティの **VerifiedDomains** プロパティは、**VerifiedDomain** のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="cb624-p103">Specifies a domain for a tenant. The **verifiedDomains** property of the [organization](organization.md) entity is a collection of **VerifiedDomain**.</span></span>


## <a name="properties"></a><span data-ttu-id="cb624-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cb624-109">Properties</span></span>
| <span data-ttu-id="cb624-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cb624-110">Property</span></span>     | <span data-ttu-id="cb624-111">種類</span><span class="sxs-lookup"><span data-stu-id="cb624-111">Type</span></span>   |<span data-ttu-id="cb624-112">説明</span><span class="sxs-lookup"><span data-stu-id="cb624-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cb624-113">capabilities</span><span class="sxs-lookup"><span data-stu-id="cb624-113">capabilities</span></span>|<span data-ttu-id="cb624-114">String</span><span class="sxs-lookup"><span data-stu-id="cb624-114">String</span></span>|<span data-ttu-id="cb624-115">「電子メール」、「OfficeCommunicationsOnline」など。</span><span class="sxs-lookup"><span data-stu-id="cb624-115">For example, “Email”, “OfficeCommunicationsOnline”.</span></span>|
|<span data-ttu-id="cb624-116">isDefault</span><span class="sxs-lookup"><span data-stu-id="cb624-116">isDefault</span></span>|<span data-ttu-id="cb624-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="cb624-117">Boolean</span></span>|                <span data-ttu-id="cb624-118">これがテナントに関連付けられている既定のドメインの場合は **true**、それ以外の場合は **false**。</span><span class="sxs-lookup"><span data-stu-id="cb624-118">**true** if this is the default domain associated with the tenant; otherwise, **false**.</span></span>            |
|<span data-ttu-id="cb624-119">isInitial</span><span class="sxs-lookup"><span data-stu-id="cb624-119">isInitial</span></span>|<span data-ttu-id="cb624-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="cb624-120">Boolean</span></span>|<span data-ttu-id="cb624-121">これがテナントに関連付けられている初期ドメインの場合は **true**、それ以外の場合は **false**。</span><span class="sxs-lookup"><span data-stu-id="cb624-121">**true** if this is the initial domain associated with the tenant; otherwise, **false**</span></span>|
|<span data-ttu-id="cb624-122">name</span><span class="sxs-lookup"><span data-stu-id="cb624-122">name</span></span>|<span data-ttu-id="cb624-123">String</span><span class="sxs-lookup"><span data-stu-id="cb624-123">String</span></span>|<span data-ttu-id="cb624-124">ドメイン名。「contoso.onmicrosoft.com」など。</span><span class="sxs-lookup"><span data-stu-id="cb624-124">The domain name; for example, “contoso.onmicrosoft.com”</span></span>|
|<span data-ttu-id="cb624-125">type</span><span class="sxs-lookup"><span data-stu-id="cb624-125">type</span></span>|<span data-ttu-id="cb624-126">String</span><span class="sxs-lookup"><span data-stu-id="cb624-126">String</span></span>|<span data-ttu-id="cb624-127">「管理対象」など。</span><span class="sxs-lookup"><span data-stu-id="cb624-127">For example, “Managed”.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cb624-128">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="cb624-128">JSON representation</span></span>

<span data-ttu-id="cb624-129">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="cb624-129">Here is a JSON representation of the resource</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "verifiedDomain resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
