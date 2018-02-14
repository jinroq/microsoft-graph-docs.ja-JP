# <a name="devicemanagement-resource-type"></a><span data-ttu-id="33e54-101">deviceManagement リソースの種類</span><span class="sxs-lookup"><span data-stu-id="33e54-101">deviceManagement resource type</span></span>

> <span data-ttu-id="33e54-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="33e54-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="33e54-103">deviceManagement リソースは、Intune で事前設定されたテナントのコレクション デバイス ID と、事前登録構成をサポートするデバイス ID に割り当てられる登録プロファイルを表します。</span><span class="sxs-lookup"><span data-stu-id="33e54-103">The deviceManagement resource represents a tenant's collection device identities that have been pre-staged in Intune, and the enrollment profiles that may be assigned to device identities that support pre-enrollment configuration.</span></span>
## <a name="methods"></a><span data-ttu-id="33e54-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="33e54-104">Methods</span></span>
|<span data-ttu-id="33e54-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="33e54-105">Method</span></span>|<span data-ttu-id="33e54-106">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="33e54-106">Return Type</span></span>|<span data-ttu-id="33e54-107">説明</span><span class="sxs-lookup"><span data-stu-id="33e54-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="33e54-108">deviceManagement の取得</span><span class="sxs-lookup"><span data-stu-id="33e54-108">Get deviceManagement</span></span>](../api/intune_enrollment_devicemanagement_get.md)|[<span data-ttu-id="33e54-109">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="33e54-109">deviceManagement</span></span>](../resources/intune_enrollment_devicemanagement.md)|<span data-ttu-id="33e54-110">[deviceManagement](../resources/intune_enrollment_devicemanagement.md) オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="33e54-110">Read properties and relationships of [plannerTaskDetails](../resources/intune_enrollment_devicemanagement.md) object.</span></span>|
|[<span data-ttu-id="33e54-111">deviceManagement の更新</span><span class="sxs-lookup"><span data-stu-id="33e54-111">Update deviceManagement</span></span>](../api/intune_enrollment_devicemanagement_update.md)|[<span data-ttu-id="33e54-112">deviceManagement</span><span class="sxs-lookup"><span data-stu-id="33e54-112">deviceManagement</span></span>](../resources/intune_enrollment_devicemanagement.md)|<span data-ttu-id="33e54-113">[deviceManagement](../resources/intune_enrollment_devicemanagement.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="33e54-113">Update the properties of a [calendar](../resources/intune_enrollment_devicemanagement.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="33e54-114">プロパティ</span><span class="sxs-lookup"><span data-stu-id="33e54-114">Properties</span></span>
|<span data-ttu-id="33e54-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="33e54-115">Property</span></span>|<span data-ttu-id="33e54-116">型</span><span class="sxs-lookup"><span data-stu-id="33e54-116">Type</span></span>|<span data-ttu-id="33e54-117">説明</span><span class="sxs-lookup"><span data-stu-id="33e54-117">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="33e54-118">id</span><span class="sxs-lookup"><span data-stu-id="33e54-118">id</span></span>|<span data-ttu-id="33e54-119">文字列</span><span class="sxs-lookup"><span data-stu-id="33e54-119">String</span></span>|<span data-ttu-id="33e54-120">オブジェクトの GUID です。</span><span class="sxs-lookup"><span data-stu-id="33e54-120">The user GUID for the security object is not valid.</span></span>|

## <a name="relationships"></a><span data-ttu-id="33e54-121">関係</span><span class="sxs-lookup"><span data-stu-id="33e54-121">Relationships</span></span>
<span data-ttu-id="33e54-122">なし</span><span class="sxs-lookup"><span data-stu-id="33e54-122">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="33e54-123">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="33e54-123">JSON Representation</span></span>
<span data-ttu-id="33e54-124">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="33e54-124">Here is a JSON representation of the resource.</span></span>
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



