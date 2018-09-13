# <a name="hostsecuritystate-resource-type"></a><span data-ttu-id="d82f8-101">hostSecurityState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d82f8-101">hostSecurityState resource type</span></span>

<span data-ttu-id="d82f8-102">ホストに関するステートフルな情報 (デバイス、コンピューターなど) が含まれます。</span><span class="sxs-lookup"><span data-stu-id="d82f8-102">Contains stateful information about the host (including devices, computers, and so on).</span></span>

## <a name="properties"></a><span data-ttu-id="d82f8-103">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d82f8-103">Properties</span></span>

| <span data-ttu-id="d82f8-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d82f8-104">Property</span></span>   | <span data-ttu-id="d82f8-105">型</span><span class="sxs-lookup"><span data-stu-id="d82f8-105">Type</span></span>|<span data-ttu-id="d82f8-106">説明</span><span class="sxs-lookup"><span data-stu-id="d82f8-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d82f8-107">FQDN</span><span class="sxs-lookup"><span data-stu-id="d82f8-107">FQDN</span></span>|<span data-ttu-id="d82f8-108">文字列</span><span class="sxs-lookup"><span data-stu-id="d82f8-108">String</span></span>|<span data-ttu-id="d82f8-109">ホスト FQDN (完全修飾ドメイン名) (たとえば、 `machine.company.com`)。</span><span class="sxs-lookup"><span data-stu-id="d82f8-109">Host FQDN (Fully Qualified Domain Name) (for example, `machine.company.com`).</span></span>|
|<span data-ttu-id="d82f8-110">isAzureAadJoined</span><span class="sxs-lookup"><span data-stu-id="d82f8-110">isAzureAadJoined</span></span>|<span data-ttu-id="d82f8-111">ブール値</span><span class="sxs-lookup"><span data-stu-id="d82f8-111">Boolean</span></span>|<span data-ttu-id="d82f8-112">ホストが Azure Active Directory ドメイン サービスに参加しているドメインである場合は true。</span><span class="sxs-lookup"><span data-stu-id="d82f8-112">True if the host is domain joined to Azure Active Directory Domain Services.</span></span>|
|<span data-ttu-id="d82f8-113">isAzureAadRegistered</span><span class="sxs-lookup"><span data-stu-id="d82f8-113">isAzureAadRegistered</span></span>|<span data-ttu-id="d82f8-114">ブール値</span><span class="sxs-lookup"><span data-stu-id="d82f8-114">Boolean</span></span>|<span data-ttu-id="d82f8-115">Azure Active Directory Device Registration (BYOD デバイスは、起業によって完全に管理されていません) で登録されたホストの場合は true。</span><span class="sxs-lookup"><span data-stu-id="d82f8-115">True if the host registered with Azure Active Directory Device Registration (BYOD devices - that is, not fully managed by enterprise).</span></span>|
|<span data-ttu-id="d82f8-116">isHybridAzureDomainJoined</span><span class="sxs-lookup"><span data-stu-id="d82f8-116">isHybridAzureDomainJoined</span></span>|<span data-ttu-id="d82f8-117">ブール値</span><span class="sxs-lookup"><span data-stu-id="d82f8-117">Boolean</span></span>|<span data-ttu-id="d82f8-118">ホストが、オンプレミスの Active Directory ドメインに参加しているドメインである場合は true。</span><span class="sxs-lookup"><span data-stu-id="d82f8-118">True if the host is domain joined to an on-premises Active Directory domain.</span></span>|
|<span data-ttu-id="d82f8-119">netBiosName</span><span class="sxs-lookup"><span data-stu-id="d82f8-119">netBiosName</span></span>|<span data-ttu-id="d82f8-120">文字列</span><span class="sxs-lookup"><span data-stu-id="d82f8-120">String</span></span>|<span data-ttu-id="d82f8-121">DNS ドメイン名を持たないローカル ホスト名</span><span class="sxs-lookup"><span data-stu-id="d82f8-121">The local host name, without the DNS domain name.</span></span>|
|<span data-ttu-id="d82f8-122">os</span><span class="sxs-lookup"><span data-stu-id="d82f8-122">OS</span></span>|<span data-ttu-id="d82f8-123">文字列</span><span class="sxs-lookup"><span data-stu-id="d82f8-123">String</span></span>|<span data-ttu-id="d82f8-124">文字列</span><span class="sxs-lookup"><span data-stu-id="d82f8-124">Host Operating System.</span></span> <span data-ttu-id="d82f8-125">(たとえば、Windows10、MacOS、RHEL など)。</span><span class="sxs-lookup"><span data-stu-id="d82f8-125">(For example, Windows10, MacOS, RHEL, etc.).</span></span>|
|<span data-ttu-id="d82f8-126">privateIpAddress</span><span class="sxs-lookup"><span data-stu-id="d82f8-126">privateIpAddress</span></span>|<span data-ttu-id="d82f8-127">文字列</span><span class="sxs-lookup"><span data-stu-id="d82f8-127">String</span></span>|<span data-ttu-id="d82f8-128">警告時の (ルーティングできない) プライベート IPv4 または IPv6 アドレス ( [RFC 1918](https://tools.ietf.org/html/rfc1918) 参照)。</span><span class="sxs-lookup"><span data-stu-id="d82f8-128">Private (not routable) IPv4 or IPv6 address (see [RFC 1918](https://tools.ietf.org/html/rfc1918)) at the time of the alert.</span></span>|
|<span data-ttu-id="d82f8-129">publicIpAddress</span><span class="sxs-lookup"><span data-stu-id="d82f8-129">publicIpAddress</span></span>|<span data-ttu-id="d82f8-130">文字列</span><span class="sxs-lookup"><span data-stu-id="d82f8-130">String</span></span>|<span data-ttu-id="d82f8-131">警告時の公的にルーティング可能な IPv4 アドレスまたは IPv6 アドレス ( [RFC 1918](https://tools.ietf.org/html/rfc1918) 参照)。</span><span class="sxs-lookup"><span data-stu-id="d82f8-131">Publicly routable IPv4 or IPv6 address (see [RFC 1918](https://tools.ietf.org/html/rfc1918)) at time of the alert.</span></span>|
|<span data-ttu-id="d82f8-132">riskScore</span><span class="sxs-lookup"><span data-stu-id="d82f8-132">riskScore</span></span>|<span data-ttu-id="d82f8-133">文字列</span><span class="sxs-lookup"><span data-stu-id="d82f8-133">String</span></span>|<span data-ttu-id="d82f8-134">プロバイダーが生成 / 計算したホストのリスク スコアです。</span><span class="sxs-lookup"><span data-stu-id="d82f8-134">Provider-generated/calculated risk score of the host.</span></span>  <span data-ttu-id="d82f8-135">1 パーセンテージ相当する 0 - 1 の値の範囲を推奨します。</span><span class="sxs-lookup"><span data-stu-id="d82f8-135">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d82f8-136">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d82f8-136">JSON representation</span></span>

<span data-ttu-id="d82f8-137">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d82f8-137">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.hostSecurityState"
}-->

```json
{
  "fqdn": "String",
  "isAzureAadJoined": true,
  "isAzureAadRegistered": true,
  "isHybridAzureDomainJoined": true,
  "netBiosName": "String",
  "os": "String",
  "privateIpAddress": "String",
  "publicIpAddress": "String",
  "riskScore": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "hostSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
