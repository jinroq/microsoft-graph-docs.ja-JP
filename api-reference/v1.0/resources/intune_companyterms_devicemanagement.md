# <a name="devicemanagement-resource-type"></a><span data-ttu-id="60b1d-101">deviceManagement リソースの種類</span><span class="sxs-lookup"><span data-stu-id="60b1d-101">deviceManagement resource type</span></span>

> <span data-ttu-id="60b1d-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="60b1d-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="60b1d-103">すべてのデバイス管理機能のコンテナーとして機能する単一のエンティティです。</span><span class="sxs-lookup"><span data-stu-id="60b1d-103">Singleton entity that acts as a container for all device management functionality.</span></span>
## <a name="methods"></a><span data-ttu-id="60b1d-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="60b1d-104">Methods</span></span>
|<span data-ttu-id="60b1d-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="60b1d-105">Method</span></span>|<span data-ttu-id="60b1d-106">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="60b1d-106">Return Type</span></span>|<span data-ttu-id="60b1d-107">説明</span><span class="sxs-lookup"><span data-stu-id="60b1d-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="60b1d-108">Get deviceManagement</span><span class="sxs-lookup"><span data-stu-id="60b1d-108">Get deviceManagement</span></span>](../api/intune_companyterms_devicemanagement_get.md)|[<span data-ttu-id="60b1d-109">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="60b1d-109">deviceManagement</span></span>](../resources/intune_companyterms_devicemanagement.md)|<span data-ttu-id="60b1d-110">[deviceManagement](../resources/intune_companyterms_devicemanagement.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="60b1d-110">Read properties and relationships of [plannerTaskDetails](../resources/intune_companyterms_devicemanagement.md) object.</span></span>|
|[<span data-ttu-id="60b1d-111">Update deviceManagement</span><span class="sxs-lookup"><span data-stu-id="60b1d-111">Update deviceManagement</span></span>](../api/intune_companyterms_devicemanagement_update.md)|[<span data-ttu-id="60b1d-112">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="60b1d-112">deviceManagement</span></span>](../resources/intune_companyterms_devicemanagement.md)|<span data-ttu-id="60b1d-113">[deviceManagement](../resources/intune_companyterms_devicemanagement.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="60b1d-113">Update the properties of a [calendar](../resources/intune_companyterms_devicemanagement.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="60b1d-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="60b1d-114">Properties</span></span>
|<span data-ttu-id="60b1d-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="60b1d-115">Property</span></span>|<span data-ttu-id="60b1d-116">型</span><span class="sxs-lookup"><span data-stu-id="60b1d-116">Type</span></span>|<span data-ttu-id="60b1d-117">説明</span><span class="sxs-lookup"><span data-stu-id="60b1d-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="60b1d-118">id</span><span class="sxs-lookup"><span data-stu-id="60b1d-118">id</span></span>|<span data-ttu-id="60b1d-119">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="60b1d-119">String</span></span>|<span data-ttu-id="60b1d-120">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="60b1d-120">Not yet documented</span></span>|

## <a name="relationships"></a><span data-ttu-id="60b1d-121">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="60b1d-121">Relationships</span></span>
|<span data-ttu-id="60b1d-122">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="60b1d-122">Relationship</span></span>|<span data-ttu-id="60b1d-123">型</span><span class="sxs-lookup"><span data-stu-id="60b1d-123">Type</span></span>|<span data-ttu-id="60b1d-124">説明</span><span class="sxs-lookup"><span data-stu-id="60b1d-124">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="60b1d-125">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="60b1d-125">termsAndConditions</span></span>|<span data-ttu-id="60b1d-126">[termsAndConditions](../resources/intune_companyterms_termsandconditions.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="60b1d-126">[termsAndConditions](../resources/intune_companyterms_termsandconditions.md) collection</span></span>|<span data-ttu-id="60b1d-127">対象の会社のデバイス管理に関連付けられている条項および条件。</span><span class="sxs-lookup"><span data-stu-id="60b1d-127">The terms and conditions associated with device management of the company.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="60b1d-128">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="60b1d-128">JSON Representation</span></span>
<span data-ttu-id="60b1d-129">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="60b1d-129">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagement"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagement",
  "id": "String (identifier)"
}
```



