# <a name="securityvendorinformation-resource-type"></a><span data-ttu-id="db81a-101">securityVendorInformation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="db81a-101">securityVendorInformation resource type</span></span>

<span data-ttu-id="db81a-102">セキュリティ製品やサービスの仕入先、プロバイダー、および subprovider の詳細が含まれています (たとえば、ベンダー = Microsoft; プロバイダー = Windows Defender の分析ツールです。 subProvider AppLocker を =)。</span><span class="sxs-lookup"><span data-stu-id="db81a-102">Contains details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span>

## <a name="properties"></a><span data-ttu-id="db81a-103">プロパティ</span><span class="sxs-lookup"><span data-stu-id="db81a-103">Properties</span></span>

| <span data-ttu-id="db81a-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="db81a-104">Property</span></span>   | <span data-ttu-id="db81a-105">型</span><span class="sxs-lookup"><span data-stu-id="db81a-105">Type</span></span>|<span data-ttu-id="db81a-106">説明</span><span class="sxs-lookup"><span data-stu-id="db81a-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="db81a-107">プロバイダー</span><span class="sxs-lookup"><span data-stu-id="db81a-107">provider</span></span> |<span data-ttu-id="db81a-108">文字列</span><span class="sxs-lookup"><span data-stu-id="db81a-108">String</span></span>|<span data-ttu-id="db81a-109">特定のプロバイダー (製品やサービスの仕入先会社ではありません)。たとえば、WindowsDefenderATP です。</span><span class="sxs-lookup"><span data-stu-id="db81a-109">Specific provider (product/service - not vendor company); for example, WindowsDefenderATP.</span></span>|
|<span data-ttu-id="db81a-110">providerVersion</span><span class="sxs-lookup"><span data-stu-id="db81a-110">providerVersion</span></span>|<span data-ttu-id="db81a-111">文字列</span><span class="sxs-lookup"><span data-stu-id="db81a-111">String</span></span>|<span data-ttu-id="db81a-112">Subprovider、それが存在する場合は、アラートを生成したプロバイダーのバージョンです。</span><span class="sxs-lookup"><span data-stu-id="db81a-112">Version of the provider or subprovider, if it exists, that generated the alert.</span></span> <span data-ttu-id="db81a-113">*Required*</span><span class="sxs-lookup"><span data-stu-id="db81a-113">*Required*</span></span>|
|<span data-ttu-id="db81a-114">subProvider</span><span class="sxs-lookup"><span data-stu-id="db81a-114">subProvider</span></span>|<span data-ttu-id="db81a-115">文字列</span><span class="sxs-lookup"><span data-stu-id="db81a-115">String</span></span>|<span data-ttu-id="db81a-116">特定の subprovider 下にあるプロバイダーを集約)。たとえば、WindowsDefenderATP.SmartScreen です。</span><span class="sxs-lookup"><span data-stu-id="db81a-116">Specific subprovider (under aggregating provider); for example, WindowsDefenderATP.SmartScreen.</span></span>|
|<span data-ttu-id="db81a-117">仕入先</span><span class="sxs-lookup"><span data-stu-id="db81a-117">vendor</span></span> |<span data-ttu-id="db81a-118">文字列</span><span class="sxs-lookup"><span data-stu-id="db81a-118">String</span></span>|<span data-ttu-id="db81a-119">アラート ベンダー (マイクロソフトでは、Dell の FireEye など) の名前。</span><span class="sxs-lookup"><span data-stu-id="db81a-119">Name of the alert vendor (for example, Microsoft, Dell, FireEye).</span></span> <span data-ttu-id="db81a-120">*Required*</span><span class="sxs-lookup"><span data-stu-id="db81a-120">*Required*</span></span>|


## <a name="json-representation"></a><span data-ttu-id="db81a-121">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="db81a-121">JSON representation</span></span>

<span data-ttu-id="db81a-122">次は、リソースの JSON 表現です。</span><span class="sxs-lookup"><span data-stu-id="db81a-122">The folllowing is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.securityVendorInformation"
}-->

```json
{
  "provider": "String",
  "providerVersion": "String",
  "subProvider": "String",
  "vendor": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "securityVendorInformation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
