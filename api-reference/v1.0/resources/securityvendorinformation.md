# <a name="securityvendorinformation-resource-type"></a><span data-ttu-id="41c26-101">securityVendorInformation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="41c26-101">securityVendorInformation resource type</span></span>

<span data-ttu-id="41c26-102">セキュリティ製品、またはサービスの仕入先、サービス プロバイダー、およびサービス サブプロバイダーの詳細を含む複合型 (仕入先 = Microsoft、プロバイダー = Windows Defender ATP、サブプロバイダー = AppLocker など)。</span><span class="sxs-lookup"><span data-stu-id="41c26-102">Contains details about the security product/service vendor, provider, and subprovider (for example, vendor=Microsoft; provider=Windows Defender ATP; subProvider=AppLocker).</span></span>

## <a name="properties"></a><span data-ttu-id="41c26-103">プロパティ</span><span class="sxs-lookup"><span data-stu-id="41c26-103">Properties</span></span>

| <span data-ttu-id="41c26-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="41c26-104">Property</span></span>   | <span data-ttu-id="41c26-105">型</span><span class="sxs-lookup"><span data-stu-id="41c26-105">Type</span></span>|<span data-ttu-id="41c26-106">説明</span><span class="sxs-lookup"><span data-stu-id="41c26-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="41c26-107">プロバイダ</span><span class="sxs-lookup"><span data-stu-id="41c26-107">provider \*</span></span>|<span data-ttu-id="41c26-108">文字列</span><span class="sxs-lookup"><span data-stu-id="41c26-108">String</span></span>|<span data-ttu-id="41c26-109">特定のプロバイダー (製品やサービスの仕入先会社ではありません)。例えば、WindowsDefenderATP です。</span><span class="sxs-lookup"><span data-stu-id="41c26-109">Specific provider (product/service - not vendor company); for example, WindowsDefenderATP.</span></span>|
|<span data-ttu-id="41c26-110">providerVersion</span><span class="sxs-lookup"><span data-stu-id="41c26-110">providerVersion</span></span>|<span data-ttu-id="41c26-111">文字列</span><span class="sxs-lookup"><span data-stu-id="41c26-111">String</span></span>|<span data-ttu-id="41c26-112">Subprovider、それが存在する場合は、アラートを生成したプロバイダーのバージョンです。</span><span class="sxs-lookup"><span data-stu-id="41c26-112">Version of the provider or subprovider, if it exists, that generated the alert.</span></span>|
|<span data-ttu-id="41c26-113">subProvider</span><span class="sxs-lookup"><span data-stu-id="41c26-113">subProvider</span></span>|<span data-ttu-id="41c26-114">文字列</span><span class="sxs-lookup"><span data-stu-id="41c26-114">String</span></span>|<span data-ttu-id="41c26-115">特定の subprovider 下にあるプロバイダーを集約)。例えば、WindowsDefenderATP.SmartScreen です。</span><span class="sxs-lookup"><span data-stu-id="41c26-115">Specific subprovider (under aggregating provider); for example, WindowsDefenderATP.SmartScreen.</span></span>|
|<span data-ttu-id="41c26-116">仕入先＊</span><span class="sxs-lookup"><span data-stu-id="41c26-116">vendor \*</span></span>|<span data-ttu-id="41c26-117">文字列</span><span class="sxs-lookup"><span data-stu-id="41c26-117">String</span></span>|<span data-ttu-id="41c26-118">アラート ベンダー (Microsoft、Dell 、 FireEye など) の名前。</span><span class="sxs-lookup"><span data-stu-id="41c26-118">Name of the alert vendor (for example, Microsoft, Dell, FireEye).</span></span>|
<span data-ttu-id="41c26-119">(\* は、必須記入欄を表示します)。</span><span class="sxs-lookup"><span data-stu-id="41c26-119">(\* Indicates a mandatory field.)</span></span>

## <a name="json-representation"></a><span data-ttu-id="41c26-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="41c26-120">JSON representation</span></span>

<span data-ttu-id="41c26-121">次は、リソースの JSON 表現です。</span><span class="sxs-lookup"><span data-stu-id="41c26-121">The following is a JSON representation of the resource.</span></span>
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
