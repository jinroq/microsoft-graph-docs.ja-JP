# <a name="contract-resource-type"></a><span data-ttu-id="f37b1-101">コントラクト リソース型</span><span class="sxs-lookup"><span data-stu-id="f37b1-101">Contract resource type</span></span>
<span data-ttu-id="f37b1-102">パートナー テナントがカスタマー テナントとの間で持つ、既存のパートナーシップを表します。</span><span class="sxs-lookup"><span data-stu-id="f37b1-102">Represents an existing partnership that the partner tenant has with a customer tenant.</span></span>

> <span data-ttu-id="f37b1-p101">**重要:** パートナー テナントにのみ存在します。パートナー テナントとは、[Microsoft クラウド ソリューション プロバイダー](https://partnercenter.microsoft.com/en-us/partner/programs)、Office 365 Syndication、Microsoft Advisor パートナー プログラムのいずれかに含まれている、Microsoft パートナーに所属する Azure AD テナントです。</span><span class="sxs-lookup"><span data-stu-id="f37b1-p101">**Important:** Exists in partner tenants only. Partner tenants are Azure AD tenants that belong to Microsoft partners who are either part of [Microsoft Cloud Solution Provider](https://partnercenter.microsoft.com/en-us/partner/programs), Office 365 Syndication, or Microsoft Advisor partner programs.</span></span>

## <a name="methods"></a><span data-ttu-id="f37b1-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="f37b1-105">Methods</span></span>

| <span data-ttu-id="f37b1-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="f37b1-106">Method</span></span>   | <span data-ttu-id="f37b1-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="f37b1-107">Return Type</span></span> | <span data-ttu-id="f37b1-108">説明</span><span class="sxs-lookup"><span data-stu-id="f37b1-108">Description</span></span> |
|:---------------|:--------|:----------|
|[<span data-ttu-id="f37b1-109">コントラクトを取得する</span><span class="sxs-lookup"><span data-stu-id="f37b1-109">Get contract</span></span>](../api/contract_get.md) | <span data-ttu-id="f37b1-110">コントラクト</span><span class="sxs-lookup"><span data-stu-id="f37b1-110">Contract</span></span> |<span data-ttu-id="f37b1-111">特定のコントラクト オブジェクトのプロパティを参照します。</span><span class="sxs-lookup"><span data-stu-id="f37b1-111">Read properties of a specific contract object.</span></span> |
|[<span data-ttu-id="f37b1-112">コントラクトを一覧表示する</span><span class="sxs-lookup"><span data-stu-id="f37b1-112">List contracts</span></span>](../api/contract_list.md) | <span data-ttu-id="f37b1-113">コントラクト コレクション</span><span class="sxs-lookup"><span data-stu-id="f37b1-113">Contract collection</span></span> | <span data-ttu-id="f37b1-114">パートナー テナントのコントラクトの一覧です。</span><span class="sxs-lookup"><span data-stu-id="f37b1-114">List of contracts in the partner tenant.</span></span> |

## <a name="properties"></a><span data-ttu-id="f37b1-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f37b1-115">Properties</span></span>
| <span data-ttu-id="f37b1-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f37b1-116">Property</span></span>   | <span data-ttu-id="f37b1-117">タイプ</span><span class="sxs-lookup"><span data-stu-id="f37b1-117">Type</span></span> | <span data-ttu-id="f37b1-118">説明</span><span class="sxs-lookup"><span data-stu-id="f37b1-118">Description</span></span> |
|:---------------|:--------|:----------|
|<span data-ttu-id="f37b1-119">contractType</span><span class="sxs-lookup"><span data-stu-id="f37b1-119">contractType</span></span>|<span data-ttu-id="f37b1-120">文字列</span><span class="sxs-lookup"><span data-stu-id="f37b1-120">String</span></span>|<span data-ttu-id="f37b1-121">コントラクトの型。</span><span class="sxs-lookup"><span data-stu-id="f37b1-121">Type of contract.</span></span><br><br><span data-ttu-id="f37b1-122">使用可能な値は次のとおりです。</span><span class="sxs-lookup"><span data-stu-id="f37b1-122">Possible values are:</span></span><br> <span data-ttu-id="f37b1-p102">*SyndicationPartner* - この顧客に対し O365 と Intune を排他的に再販し管理するパートナーです。再販し、顧客をサポートします。</span><span class="sxs-lookup"><span data-stu-id="f37b1-p102">*SyndicationPartner* - Partner that exclusively resells and manages O365 and Intune for this customer. They resell and support their customers.</span></span><br> <span data-ttu-id="f37b1-p103">*BreadthPartner* - この顧客に対し管理上のサポートを提供する能力を備えたパートナーです。ただし、パートナーが顧客に再販売することは許されていません。</span><span class="sxs-lookup"><span data-stu-id="f37b1-p103">*BreadthPartner* - Partner has the ability to provide administrative support for this customer. However, the partner is not allowed to resell to the customer.</span></span><br><span data-ttu-id="f37b1-p104">*ResellerPartner* - シンジケーション パートナーに類似していますが、テナントへの排他的アクセスを持たないパートナーです。シンジケーションの場合、顧客は Microsoft またはその他のパートナーから直接に追加のサブスクリプションを購入することはできません。</span><span class="sxs-lookup"><span data-stu-id="f37b1-p104">*ResellerPartner* - Partner that is similar to a syndication partner, except that the partner doesn’t have exclusive access to a tenant. In the syndication case, the customer cannot buy additional direct subscriptions from Microsoft or from other partners.</span></span>|
|<span data-ttu-id="f37b1-129">customerId</span><span class="sxs-lookup"><span data-stu-id="f37b1-129">customerId</span></span>|<span data-ttu-id="f37b1-130">Guid</span><span class="sxs-lookup"><span data-stu-id="f37b1-130">Guid</span></span>|<span data-ttu-id="f37b1-p105">このパートナーシップによって参照されるカスタマー テナントの一意識別子です。カスタマー テナントの組織リソースの ID プロパティに対応します。</span><span class="sxs-lookup"><span data-stu-id="f37b1-p105">The unique identifier for the customer tenant referenced by this partnership. Corresponds to the id property of the customer tenant's organization resource.</span></span> |
|<span data-ttu-id="f37b1-133">defaultDomainName</span><span class="sxs-lookup"><span data-stu-id="f37b1-133">defaultDomainName</span></span>|<span data-ttu-id="f37b1-134">文字列</span><span class="sxs-lookup"><span data-stu-id="f37b1-134">String</span></span>|<span data-ttu-id="f37b1-p106">カスタマー テナントの既定のドメイン名のコピーです。顧客とのパートナーシップが確立されるとコピーを作成します。カスタマー テナントの既定のドメイン名が変更された場合は、自動的には更新されません。</span><span class="sxs-lookup"><span data-stu-id="f37b1-p106">A copy of the customer tenant's default domain name. The copy is made when the partnership with the customer is established. It is not automatically updated if the customer tenant's default domain name changes.</span></span>|
|<span data-ttu-id="f37b1-138">displayName</span><span class="sxs-lookup"><span data-stu-id="f37b1-138">displayName</span></span>|<span data-ttu-id="f37b1-139">文字列</span><span class="sxs-lookup"><span data-stu-id="f37b1-139">String</span></span>|<span data-ttu-id="f37b1-p107">カスタマー テナントの表示名のコピーです。顧客とのパートナーシップが確立されるとコピーを作成します。カスタマー テナントの表示名が変更された場合は、自動的には更新されません。</span><span class="sxs-lookup"><span data-stu-id="f37b1-p107">A copy of the customer tenant's display name. The copy is made when the partnership with the customer is established. It is not automatically updated if the customer tenant's display name changes.</span></span>|
|<span data-ttu-id="f37b1-143">id</span><span class="sxs-lookup"><span data-stu-id="f37b1-143">id</span></span>|<span data-ttu-id="f37b1-144">文字列</span><span class="sxs-lookup"><span data-stu-id="f37b1-144">String</span></span>| <span data-ttu-id="f37b1-p108">パートナーシップの一意識別子です。キー、読み取り専用</span><span class="sxs-lookup"><span data-stu-id="f37b1-p108">The unique identifier for the partnership. Key, read-only</span></span> |

## <a name="relationships"></a><span data-ttu-id="f37b1-147">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f37b1-147">Relationships</span></span>
<span data-ttu-id="f37b1-148">なし</span><span class="sxs-lookup"><span data-stu-id="f37b1-148">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="f37b1-149">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f37b1-149">JSON representation</span></span>
<span data-ttu-id="f37b1-150">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f37b1-150">Here is a JSON representation of the resource.</span></span>

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