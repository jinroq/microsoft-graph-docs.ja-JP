# <a name="cloudappsecuritystate-resource-type"></a><span data-ttu-id="22ef1-101">cloudAppSecurityState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="22ef1-101">cloudAppSecurityState resource type</span></span>

<span data-ttu-id="22ef1-102">ステートフル (destinationServiceName、destinationServiceIp) は、クラウド アプリケーションについてを説明します。</span><span class="sxs-lookup"><span data-stu-id="22ef1-102">Contains stateful information about the cloud application (destinationServiceName, destinationServiceIp).</span></span>

## <a name="properties"></a><span data-ttu-id="22ef1-103">プロパティ</span><span class="sxs-lookup"><span data-stu-id="22ef1-103">Properties</span></span>

| <span data-ttu-id="22ef1-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="22ef1-104">Property</span></span>     | <span data-ttu-id="22ef1-105">型</span><span class="sxs-lookup"><span data-stu-id="22ef1-105">Type</span></span>        | <span data-ttu-id="22ef1-106">説明</span><span class="sxs-lookup"><span data-stu-id="22ef1-106">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="22ef1-107">destinationServiceIp</span><span class="sxs-lookup"><span data-stu-id="22ef1-107">destinationServiceIp</span></span>|<span data-ttu-id="22ef1-108">文字列</span><span class="sxs-lookup"><span data-stu-id="22ef1-108">String</span></span>|<span data-ttu-id="22ef1-109">クラウド アプリケーションやサービスへの接続の宛先の IP アドレス。</span><span class="sxs-lookup"><span data-stu-id="22ef1-109">Destination IP Address of the connection to the cloud application/service.</span></span>|
|<span data-ttu-id="22ef1-110">destinationServiceName</span><span class="sxs-lookup"><span data-stu-id="22ef1-110">destinationServiceName</span></span>|<span data-ttu-id="22ef1-111">文字列</span><span class="sxs-lookup"><span data-stu-id="22ef1-111">String</span></span>|<span data-ttu-id="22ef1-112">クラウド アプリケーションとサービスの名前 (たとえば「Salesforce」、「ドロップ ボックス」など)。</span><span class="sxs-lookup"><span data-stu-id="22ef1-112">Cloud application/service name (for example "Salesforce", "DropBox", etc.).</span></span>|
|<span data-ttu-id="22ef1-113">riskScore</span><span class="sxs-lookup"><span data-stu-id="22ef1-113">riskScore</span></span>|<span data-ttu-id="22ef1-114">文字列</span><span class="sxs-lookup"><span data-stu-id="22ef1-114">String</span></span>|<span data-ttu-id="22ef1-115">プロバイダーによって生成されると計算されるリスク スコア クラウド アプリケーションとサービスのです。</span><span class="sxs-lookup"><span data-stu-id="22ef1-115">Provider-generated/calculated risk score of the Cloud Application/Service.</span></span> <span data-ttu-id="22ef1-116">1 パーセンテージ相当する 0 - 1 の値の範囲を推奨します。</span><span class="sxs-lookup"><span data-stu-id="22ef1-116">Recommended value range of 0-1, which equates to a percentage.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="22ef1-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="22ef1-117">JSON representation</span></span>

<span data-ttu-id="22ef1-118">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="22ef1-118">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.cloudAppSecurityState"
}-->

```json
{
  "destinationServiceIp": "String",
  "destinationServiceName": "String",
  "riskScore": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "cloudAppSecurityState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->