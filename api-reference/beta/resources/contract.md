---
title: コントラクト リソース型
description: パートナー テナントがカスタマー テナントとの間で持つ、既存のパートナーシップを表します。
localization_priority: Normal
ms.openlocfilehash: e502c72003c6d65305430bc1bf5a539d7235b5ef
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27815324"
---
# <a name="contract-resource-type"></a><span data-ttu-id="cb6f9-103">コントラクト リソース型</span><span class="sxs-lookup"><span data-stu-id="cb6f9-103">Contract resource type</span></span>

> <span data-ttu-id="cb6f9-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="cb6f9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cb6f9-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cb6f9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cb6f9-106">パートナー テナントがカスタマー テナントとの間で持つ、既存のパートナーシップを表します。</span><span class="sxs-lookup"><span data-stu-id="cb6f9-106">Represents an existing partnership that the partner tenant has with a customer tenant.</span></span>

> <span data-ttu-id="cb6f9-p102">**重要:** パートナー テナントにのみ存在します。パートナー テナントとは、[Microsoft クラウド ソリューション プロバイダー](https://partnercenter.microsoft.com/en-us/partner/programs)、Office 365 Syndication、Microsoft Advisor パートナー プログラムのいずれかに含まれている、Microsoft パートナーに所属する Azure AD テナントです。</span><span class="sxs-lookup"><span data-stu-id="cb6f9-p102">**Important:** Exists in partner tenants only. Partner tenants are Azure AD tenants that belong to Microsoft partners who are either part of [Microsoft Cloud Solution Provider](https://partnercenter.microsoft.com/en-us/partner/programs), Office 365 Syndication, or Microsoft Advisor partner programs.</span></span>

## <a name="methods"></a><span data-ttu-id="cb6f9-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="cb6f9-109">Methods</span></span>

| <span data-ttu-id="cb6f9-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="cb6f9-110">Method</span></span>   | <span data-ttu-id="cb6f9-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="cb6f9-111">Return Type</span></span> | <span data-ttu-id="cb6f9-112">説明</span><span class="sxs-lookup"><span data-stu-id="cb6f9-112">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="cb6f9-113">コントラクトを取得する</span><span class="sxs-lookup"><span data-stu-id="cb6f9-113">Get contract</span></span>](../api/contract-get.md) | <span data-ttu-id="cb6f9-114">コントラクト</span><span class="sxs-lookup"><span data-stu-id="cb6f9-114">Contract</span></span> |<span data-ttu-id="cb6f9-115">特定のコントラクト オブジェクトのプロパティを参照します。</span><span class="sxs-lookup"><span data-stu-id="cb6f9-115">Read properties of a specific contract object.</span></span> |
|[<span data-ttu-id="cb6f9-116">コントラクトを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="cb6f9-116">List contracts</span></span>](../api/contract-list.md) | <span data-ttu-id="cb6f9-117">コントラクト コレクション</span><span class="sxs-lookup"><span data-stu-id="cb6f9-117">Contract collection</span></span> | <span data-ttu-id="cb6f9-118">パートナー テナントのコントラクトの一覧です。</span><span class="sxs-lookup"><span data-stu-id="cb6f9-118">List of contracts in the partner tenant.</span></span> |

## <a name="properties"></a><span data-ttu-id="cb6f9-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cb6f9-119">Properties</span></span>
| <span data-ttu-id="cb6f9-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cb6f9-120">Property</span></span>   | <span data-ttu-id="cb6f9-121">種類</span><span class="sxs-lookup"><span data-stu-id="cb6f9-121">Type</span></span> | <span data-ttu-id="cb6f9-122">説明</span><span class="sxs-lookup"><span data-stu-id="cb6f9-122">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="cb6f9-123">contractType</span><span class="sxs-lookup"><span data-stu-id="cb6f9-123">contractType</span></span>|<span data-ttu-id="cb6f9-124">String</span><span class="sxs-lookup"><span data-stu-id="cb6f9-124">String</span></span>|<span data-ttu-id="cb6f9-125">コントラクトの型。</span><span class="sxs-lookup"><span data-stu-id="cb6f9-125">Type of contract.</span></span><br><br><span data-ttu-id="cb6f9-126">使用可能な値は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="cb6f9-126">Possible values are:</span></span><br> <span data-ttu-id="cb6f9-p103">*SyndicationPartner* - この顧客に対し O365 と Intune を排他的に再販し管理するパートナーです。再販し、顧客をサポートします。</span><span class="sxs-lookup"><span data-stu-id="cb6f9-p103">*SyndicationPartner* - Partner that exclusively resells and manages O365 and Intune for this customer. They resell and support their customers.</span></span><br> <span data-ttu-id="cb6f9-p104">*BreadthPartner* - この顧客に対し管理上のサポートを提供する能力を備えたパートナーです。ただし、パートナーが顧客に再販売することは許されていません。</span><span class="sxs-lookup"><span data-stu-id="cb6f9-p104">*BreadthPartner* - Partner has the ability to provide administrative support for this customer. However, the partner is not allowed to resell to the customer.</span></span><br><span data-ttu-id="cb6f9-p105">*ResellerPartner* - シンジケーション パートナーに類似していますが、テナントへの排他的アクセスを持たないパートナーです。シンジケーションの場合、顧客は Microsoft またはその他のパートナーから直接に追加のサブスクリプションを購入することはできません。</span><span class="sxs-lookup"><span data-stu-id="cb6f9-p105">*ResellerPartner* - Partner that is similar to a syndication partner, except that the partner doesn’t have exclusive access to a tenant. In the syndication case, the customer cannot buy additional direct subscriptions from Microsoft or from other partners.</span></span>|
|<span data-ttu-id="cb6f9-133">customerId</span><span class="sxs-lookup"><span data-stu-id="cb6f9-133">customerId</span></span>|<span data-ttu-id="cb6f9-134">Guid</span><span class="sxs-lookup"><span data-stu-id="cb6f9-134">Guid</span></span>|<span data-ttu-id="cb6f9-p106">このパートナーシップによって参照されるカスタマー テナントの一意識別子です。カスタマー テナントの組織リソースの ID プロパティに対応します。</span><span class="sxs-lookup"><span data-stu-id="cb6f9-p106">The unique identifier for the customer tenant referenced by this partnership. Corresponds to the id property of the customer tenant's organization resource.</span></span> |
|<span data-ttu-id="cb6f9-137">defaultDomainName</span><span class="sxs-lookup"><span data-stu-id="cb6f9-137">defaultDomainName</span></span>|<span data-ttu-id="cb6f9-138">String</span><span class="sxs-lookup"><span data-stu-id="cb6f9-138">String</span></span>|<span data-ttu-id="cb6f9-p107">カスタマー テナントの既定のドメイン名のコピーです。顧客とのパートナーシップが確立されるとコピーを作成します。カスタマー テナントの既定のドメイン名が変更された場合は、自動的には更新されません。</span><span class="sxs-lookup"><span data-stu-id="cb6f9-p107">A copy of the customer tenant's default domain name. The copy is made when the partnership with the customer is established. It is not automatically updated if the customer tenant's default domain name changes.</span></span>|
|<span data-ttu-id="cb6f9-142">displayName</span><span class="sxs-lookup"><span data-stu-id="cb6f9-142">displayName</span></span>|<span data-ttu-id="cb6f9-143">String</span><span class="sxs-lookup"><span data-stu-id="cb6f9-143">String</span></span>|<span data-ttu-id="cb6f9-p108">カスタマー テナントの表示名のコピーです。顧客とのパートナーシップが確立されるとコピーを作成します。カスタマー テナントの表示名が変更された場合は、自動的には更新されません。</span><span class="sxs-lookup"><span data-stu-id="cb6f9-p108">A copy of the customer tenant's display name. The copy is made when the partnership with the customer is established. It is not automatically updated if the customer tenant's display name changes.</span></span>|
|<span data-ttu-id="cb6f9-147">id</span><span class="sxs-lookup"><span data-stu-id="cb6f9-147">id</span></span>|<span data-ttu-id="cb6f9-148">String</span><span class="sxs-lookup"><span data-stu-id="cb6f9-148">String</span></span>| <span data-ttu-id="cb6f9-p109">パートナーシップの一意識別子です。キー、読み取り専用</span><span class="sxs-lookup"><span data-stu-id="cb6f9-p109">The unique identifier for the partnership. Key, read-only</span></span> |

## <a name="relationships"></a><span data-ttu-id="cb6f9-151">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="cb6f9-151">Relationships</span></span>
<span data-ttu-id="cb6f9-152">なし</span><span class="sxs-lookup"><span data-stu-id="cb6f9-152">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="cb6f9-153">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="cb6f9-153">JSON representation</span></span>
<span data-ttu-id="cb6f9-154">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="cb6f9-154">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "Contract resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
