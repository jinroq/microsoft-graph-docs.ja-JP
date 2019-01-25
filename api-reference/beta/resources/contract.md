---
title: コントラクト リソース型
description: パートナー テナントがカスタマー テナントとの間で持つ、既存のパートナーシップを表します。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 6309dfc370d414ccb66065fe4048d7cece51f018
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29509701"
---
# <a name="contract-resource-type"></a><span data-ttu-id="2e3f6-103">コントラクト リソース型</span><span class="sxs-lookup"><span data-stu-id="2e3f6-103">Contract resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2e3f6-104">パートナー テナントがカスタマー テナントとの間で持つ、既存のパートナーシップを表します。</span><span class="sxs-lookup"><span data-stu-id="2e3f6-104">Represents an existing partnership that the partner tenant has with a customer tenant.</span></span>

> <span data-ttu-id="2e3f6-p101">**重要:** パートナー テナントにのみ存在します。パートナー テナントとは、[Microsoft クラウド ソリューション プロバイダー](https://partnercenter.microsoft.com/en-us/partner/programs)、Office 365 Syndication、Microsoft Advisor パートナー プログラムのいずれかに含まれている、Microsoft パートナーに所属する Azure AD テナントです。</span><span class="sxs-lookup"><span data-stu-id="2e3f6-p101">**Important:** Exists in partner tenants only. Partner tenants are Azure AD tenants that belong to Microsoft partners who are either part of [Microsoft Cloud Solution Provider](https://partnercenter.microsoft.com/en-us/partner/programs), Office 365 Syndication, or Microsoft Advisor partner programs.</span></span>

## <a name="methods"></a><span data-ttu-id="2e3f6-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="2e3f6-107">Methods</span></span>

| <span data-ttu-id="2e3f6-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="2e3f6-108">Method</span></span>   | <span data-ttu-id="2e3f6-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="2e3f6-109">Return Type</span></span> | <span data-ttu-id="2e3f6-110">説明</span><span class="sxs-lookup"><span data-stu-id="2e3f6-110">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="2e3f6-111">コントラクトを取得する</span><span class="sxs-lookup"><span data-stu-id="2e3f6-111">Get contract</span></span>](../api/contract-get.md) | <span data-ttu-id="2e3f6-112">コントラクト</span><span class="sxs-lookup"><span data-stu-id="2e3f6-112">Contract</span></span> |<span data-ttu-id="2e3f6-113">特定のコントラクト オブジェクトのプロパティを参照します。</span><span class="sxs-lookup"><span data-stu-id="2e3f6-113">Read properties of a specific contract object.</span></span> |
|[<span data-ttu-id="2e3f6-114">コントラクトを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="2e3f6-114">List contracts</span></span>](../api/contract-list.md) | <span data-ttu-id="2e3f6-115">コントラクト コレクション</span><span class="sxs-lookup"><span data-stu-id="2e3f6-115">Contract collection</span></span> | <span data-ttu-id="2e3f6-116">パートナー テナントのコントラクトの一覧です。</span><span class="sxs-lookup"><span data-stu-id="2e3f6-116">List of contracts in the partner tenant.</span></span> |

## <a name="properties"></a><span data-ttu-id="2e3f6-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2e3f6-117">Properties</span></span>
| <span data-ttu-id="2e3f6-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2e3f6-118">Property</span></span>   | <span data-ttu-id="2e3f6-119">型</span><span class="sxs-lookup"><span data-stu-id="2e3f6-119">Type</span></span> | <span data-ttu-id="2e3f6-120">説明</span><span class="sxs-lookup"><span data-stu-id="2e3f6-120">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="2e3f6-121">contractType</span><span class="sxs-lookup"><span data-stu-id="2e3f6-121">contractType</span></span>|<span data-ttu-id="2e3f6-122">String</span><span class="sxs-lookup"><span data-stu-id="2e3f6-122">String</span></span>|<span data-ttu-id="2e3f6-123">コントラクトの型。</span><span class="sxs-lookup"><span data-stu-id="2e3f6-123">Type of contract.</span></span><br><br><span data-ttu-id="2e3f6-124">使用可能な値は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="2e3f6-124">Possible values are:</span></span><br> <span data-ttu-id="2e3f6-p102">*SyndicationPartner* - この顧客に対し O365 と Intune を排他的に再販し管理するパートナーです。再販し、顧客をサポートします。</span><span class="sxs-lookup"><span data-stu-id="2e3f6-p102">*SyndicationPartner* - Partner that exclusively resells and manages O365 and Intune for this customer. They resell and support their customers.</span></span><br> <span data-ttu-id="2e3f6-p103">*BreadthPartner* - この顧客に対し管理上のサポートを提供する能力を備えたパートナーです。ただし、パートナーが顧客に再販売することは許されていません。</span><span class="sxs-lookup"><span data-stu-id="2e3f6-p103">*BreadthPartner* - Partner has the ability to provide administrative support for this customer. However, the partner is not allowed to resell to the customer.</span></span><br><span data-ttu-id="2e3f6-p104">*ResellerPartner* - シンジケーション パートナーに類似していますが、テナントへの排他的アクセスを持たないパートナーです。シンジケーションの場合、顧客は Microsoft またはその他のパートナーから直接に追加のサブスクリプションを購入することはできません。</span><span class="sxs-lookup"><span data-stu-id="2e3f6-p104">*ResellerPartner* - Partner that is similar to a syndication partner, except that the partner doesn’t have exclusive access to a tenant. In the syndication case, the customer cannot buy additional direct subscriptions from Microsoft or from other partners.</span></span>|
|<span data-ttu-id="2e3f6-131">customerId</span><span class="sxs-lookup"><span data-stu-id="2e3f6-131">customerId</span></span>|<span data-ttu-id="2e3f6-132">Guid</span><span class="sxs-lookup"><span data-stu-id="2e3f6-132">Guid</span></span>|<span data-ttu-id="2e3f6-p105">このパートナーシップによって参照されるカスタマー テナントの一意識別子です。カスタマー テナントの組織リソースの ID プロパティに対応します。</span><span class="sxs-lookup"><span data-stu-id="2e3f6-p105">The unique identifier for the customer tenant referenced by this partnership. Corresponds to the id property of the customer tenant's organization resource.</span></span> |
|<span data-ttu-id="2e3f6-135">defaultDomainName</span><span class="sxs-lookup"><span data-stu-id="2e3f6-135">defaultDomainName</span></span>|<span data-ttu-id="2e3f6-136">String</span><span class="sxs-lookup"><span data-stu-id="2e3f6-136">String</span></span>|<span data-ttu-id="2e3f6-p106">カスタマー テナントの既定のドメイン名のコピーです。顧客とのパートナーシップが確立されるとコピーを作成します。カスタマー テナントの既定のドメイン名が変更された場合は、自動的には更新されません。</span><span class="sxs-lookup"><span data-stu-id="2e3f6-p106">A copy of the customer tenant's default domain name. The copy is made when the partnership with the customer is established. It is not automatically updated if the customer tenant's default domain name changes.</span></span>|
|<span data-ttu-id="2e3f6-140">displayName</span><span class="sxs-lookup"><span data-stu-id="2e3f6-140">displayName</span></span>|<span data-ttu-id="2e3f6-141">String</span><span class="sxs-lookup"><span data-stu-id="2e3f6-141">String</span></span>|<span data-ttu-id="2e3f6-p107">カスタマー テナントの表示名のコピーです。顧客とのパートナーシップが確立されるとコピーを作成します。カスタマー テナントの表示名が変更された場合は、自動的には更新されません。</span><span class="sxs-lookup"><span data-stu-id="2e3f6-p107">A copy of the customer tenant's display name. The copy is made when the partnership with the customer is established. It is not automatically updated if the customer tenant's display name changes.</span></span>|
|<span data-ttu-id="2e3f6-145">id</span><span class="sxs-lookup"><span data-stu-id="2e3f6-145">id</span></span>|<span data-ttu-id="2e3f6-146">String</span><span class="sxs-lookup"><span data-stu-id="2e3f6-146">String</span></span>| <span data-ttu-id="2e3f6-p108">パートナーシップの一意識別子です。キー、読み取り専用</span><span class="sxs-lookup"><span data-stu-id="2e3f6-p108">The unique identifier for the partnership. Key, read-only</span></span> |

## <a name="relationships"></a><span data-ttu-id="2e3f6-149">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2e3f6-149">Relationships</span></span>
<span data-ttu-id="2e3f6-150">なし</span><span class="sxs-lookup"><span data-stu-id="2e3f6-150">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="2e3f6-151">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2e3f6-151">JSON representation</span></span>
<span data-ttu-id="2e3f6-152">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2e3f6-152">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.Contract"
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
<!--
{
  "type": "#page.annotation",
  "description": "Contract resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/contract.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
