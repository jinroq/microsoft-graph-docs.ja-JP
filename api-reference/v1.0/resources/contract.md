---
title: Contract リソースの種類
description: パートナーテナントと顧客テナントの間に存在する既存のパートナーシップを表します。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ca0c12d3f797a9dc3cd8b153fdbc8ef83a33ca24
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36029611"
---
# <a name="contract-resource-type"></a><span data-ttu-id="807ba-103">Contract リソースの種類</span><span class="sxs-lookup"><span data-stu-id="807ba-103">Contract resource type</span></span>
<span data-ttu-id="807ba-104">パートナーテナントと顧客テナントの間に存在する既存のパートナーシップを表します。</span><span class="sxs-lookup"><span data-stu-id="807ba-104">Represents an existing partnership that the partner tenant has with a customer tenant.</span></span>

> <span data-ttu-id="807ba-105">**重要:** パートナーテナントのみに存在します。</span><span class="sxs-lookup"><span data-stu-id="807ba-105">**Important:** Exists in partner tenants only.</span></span> <span data-ttu-id="807ba-106">パートナーテナントは、microsoft の[クラウドソリューションプロバイダー](https://partnercenter.microsoft.com/en-us/partner/programs)、Office 365 シンジケート、または microsoft Advisor パートナープログラムの一部である microsoft パートナーに属する Azure AD テナントです。</span><span class="sxs-lookup"><span data-stu-id="807ba-106">Partner tenants are Azure AD tenants that belong to Microsoft partners who are either part of [Microsoft Cloud Solution Provider](https://partnercenter.microsoft.com/en-us/partner/programs), Office 365 Syndication, or Microsoft Advisor partner programs.</span></span>

## <a name="methods"></a><span data-ttu-id="807ba-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="807ba-107">Methods</span></span>

| <span data-ttu-id="807ba-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="807ba-108">Method</span></span>   | <span data-ttu-id="807ba-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="807ba-109">Return Type</span></span> | <span data-ttu-id="807ba-110">説明</span><span class="sxs-lookup"><span data-stu-id="807ba-110">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="807ba-111">契約書を取得する</span><span class="sxs-lookup"><span data-stu-id="807ba-111">Get contract</span></span>](../api/contract-get.md) | <span data-ttu-id="807ba-112">縮小</span><span class="sxs-lookup"><span data-stu-id="807ba-112">Contract</span></span> |<span data-ttu-id="807ba-113">特定の contract オブジェクトのプロパティを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="807ba-113">Read properties of a specific contract object.</span></span> |
|[<span data-ttu-id="807ba-114">契約書を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="807ba-114">List contracts</span></span>](../api/contract-list.md) | <span data-ttu-id="807ba-115">Contract コレクション</span><span class="sxs-lookup"><span data-stu-id="807ba-115">Contract collection</span></span> | <span data-ttu-id="807ba-116">パートナーテナント内の契約のリスト。</span><span class="sxs-lookup"><span data-stu-id="807ba-116">List of contracts in the partner tenant.</span></span> |

## <a name="properties"></a><span data-ttu-id="807ba-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="807ba-117">Properties</span></span>
| <span data-ttu-id="807ba-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="807ba-118">Property</span></span>   | <span data-ttu-id="807ba-119">型</span><span class="sxs-lookup"><span data-stu-id="807ba-119">Type</span></span> | <span data-ttu-id="807ba-120">説明</span><span class="sxs-lookup"><span data-stu-id="807ba-120">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="807ba-121">contractType</span><span class="sxs-lookup"><span data-stu-id="807ba-121">contractType</span></span>|<span data-ttu-id="807ba-122">String</span><span class="sxs-lookup"><span data-stu-id="807ba-122">String</span></span>|<span data-ttu-id="807ba-123">契約の種類。</span><span class="sxs-lookup"><span data-stu-id="807ba-123">Type of contract.</span></span><br><br><span data-ttu-id="807ba-124">使用可能な値は次のいずれかです。</span><span class="sxs-lookup"><span data-stu-id="807ba-124">Possible values are:</span></span><br> <span data-ttu-id="807ba-125">*SyndicationPartner* -このお客様に対して O365 と Intune を排他的に resells して管理します。</span><span class="sxs-lookup"><span data-stu-id="807ba-125">*SyndicationPartner* - Partner that exclusively resells and manages O365 and Intune for this customer.</span></span> <span data-ttu-id="807ba-126">これらのユーザーは、お客様を再販し、サポートしています。</span><span class="sxs-lookup"><span data-stu-id="807ba-126">They resell and support their customers.</span></span><br> <span data-ttu-id="807ba-127">*BreadthPartner* -パートナーは、このお客様に対して管理サポートを提供することができます。</span><span class="sxs-lookup"><span data-stu-id="807ba-127">*BreadthPartner* - Partner has the ability to provide administrative support for this customer.</span></span> <span data-ttu-id="807ba-128">ただし、パートナーはお客様に再販することは許可されていません。</span><span class="sxs-lookup"><span data-stu-id="807ba-128">However, the partner is not allowed to resell to the customer.</span></span><br><span data-ttu-id="807ba-129">*ResellerPartner* -シンジケートパートナーに似ていますが、パートナーがテナントへの排他的なアクセス権を持っていない点が異なります。</span><span class="sxs-lookup"><span data-stu-id="807ba-129">*ResellerPartner* - Partner that is similar to a syndication partner, except that the partner doesn’t have exclusive access to a tenant.</span></span> <span data-ttu-id="807ba-130">シンジケーションの場合、お客様は、Microsoft や他のパートナーから追加の直接サブスクリプションを購入することはできません。</span><span class="sxs-lookup"><span data-stu-id="807ba-130">In the syndication case, the customer cannot buy additional direct subscriptions from Microsoft or from other partners.</span></span>|
|<span data-ttu-id="807ba-131">Id</span><span class="sxs-lookup"><span data-stu-id="807ba-131">customerId</span></span>|<span data-ttu-id="807ba-132">Guid</span><span class="sxs-lookup"><span data-stu-id="807ba-132">Guid</span></span>|<span data-ttu-id="807ba-133">このパートナーシップによって参照される顧客のテナントの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="807ba-133">The unique identifier for the customer tenant referenced by this partnership.</span></span> <span data-ttu-id="807ba-134">顧客テナントの組織リソースの id プロパティに対応します。</span><span class="sxs-lookup"><span data-stu-id="807ba-134">Corresponds to the id property of the customer tenant's organization resource.</span></span> |
|<span data-ttu-id="807ba-135">defaultDomainName</span><span class="sxs-lookup"><span data-stu-id="807ba-135">defaultDomainName</span></span>|<span data-ttu-id="807ba-136">String</span><span class="sxs-lookup"><span data-stu-id="807ba-136">String</span></span>|<span data-ttu-id="807ba-137">顧客テナントの既定のドメイン名のコピー。</span><span class="sxs-lookup"><span data-stu-id="807ba-137">A copy of the customer tenant's default domain name.</span></span> <span data-ttu-id="807ba-138">このコピーは、顧客とのパートナーシップが確立されたときに作成されます。</span><span class="sxs-lookup"><span data-stu-id="807ba-138">The copy is made when the partnership with the customer is established.</span></span> <span data-ttu-id="807ba-139">顧客のテナントの既定のドメイン名が変更されても、自動的には更新されません。</span><span class="sxs-lookup"><span data-stu-id="807ba-139">It is not automatically updated if the customer tenant's default domain name changes.</span></span>|
|<span data-ttu-id="807ba-140">displayName</span><span class="sxs-lookup"><span data-stu-id="807ba-140">displayName</span></span>|<span data-ttu-id="807ba-141">String</span><span class="sxs-lookup"><span data-stu-id="807ba-141">String</span></span>|<span data-ttu-id="807ba-142">顧客のテナントの表示名のコピー。</span><span class="sxs-lookup"><span data-stu-id="807ba-142">A copy of the customer tenant's display name.</span></span> <span data-ttu-id="807ba-143">このコピーは、顧客とのパートナーシップが確立されたときに作成されます。</span><span class="sxs-lookup"><span data-stu-id="807ba-143">The copy is made when the partnership with the customer is established.</span></span> <span data-ttu-id="807ba-144">顧客のテナントの表示名が変更されても、自動的には更新されません。</span><span class="sxs-lookup"><span data-stu-id="807ba-144">It is not automatically updated if the customer tenant's display name changes.</span></span>|
|<span data-ttu-id="807ba-145">id</span><span class="sxs-lookup"><span data-stu-id="807ba-145">id</span></span>|<span data-ttu-id="807ba-146">文字列</span><span class="sxs-lookup"><span data-stu-id="807ba-146">String</span></span>| <span data-ttu-id="807ba-147">パートナーシップの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="807ba-147">The unique identifier for the partnership.</span></span> <span data-ttu-id="807ba-148">キー、読み取り専用</span><span class="sxs-lookup"><span data-stu-id="807ba-148">Key, read-only</span></span> |

## <a name="relationships"></a><span data-ttu-id="807ba-149">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="807ba-149">Relationships</span></span>
<span data-ttu-id="807ba-150">なし</span><span class="sxs-lookup"><span data-stu-id="807ba-150">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="807ba-151">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="807ba-151">JSON representation</span></span>
<span data-ttu-id="807ba-152">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="807ba-152">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "openType": true,
  "optionalProperties": [],
  "keyProperty": "id",
  "baseType": "microsoft.graph.directoryObject",
  "@odata.type": "microsoft.graph.contract"
}-->

```json
{
  "contractType": "String",
  "customerId": "Guid",
  "defaultDomainName": "String",
  "displayName": "String",
  "id": "String (identifier)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Contract resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
