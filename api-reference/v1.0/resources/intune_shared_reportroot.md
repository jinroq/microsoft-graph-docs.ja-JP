# <a name="reportroot-resource-type"></a><span data-ttu-id="d0902-101">reportRoot リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d0902-101">reportRoot resource type</span></span>

> <span data-ttu-id="d0902-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="d0902-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d0902-103">履歴レポートのインスタンスを表すリソースです。</span><span class="sxs-lookup"><span data-stu-id="d0902-103">The resource that represents an instance of History Reports.</span></span>
## <a name="methods"></a><span data-ttu-id="d0902-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="d0902-104">Methods</span></span>
|<span data-ttu-id="d0902-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="d0902-105">Method</span></span>|<span data-ttu-id="d0902-106">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="d0902-106">Return Type</span></span>|<span data-ttu-id="d0902-107">説明</span><span class="sxs-lookup"><span data-stu-id="d0902-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d0902-108">ReportRoot の取得</span><span class="sxs-lookup"><span data-stu-id="d0902-108">Get reportRoot</span></span>](../api/intune_shared_reportroot_get.md)|[<span data-ttu-id="d0902-109">reportRoot</span><span class="sxs-lookup"><span data-stu-id="d0902-109">reportRoot</span></span>](../resources/intune_shared_reportroot.md)|<span data-ttu-id="d0902-110">[reportRoot](../resources/intune_shared_reportroot.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="d0902-110">Read properties and relationships of the [reportRoot](../resources/intune_shared_reportroot.md) object.</span></span>|
|[<span data-ttu-id="d0902-111">reportRoot の更新</span><span class="sxs-lookup"><span data-stu-id="d0902-111">Update reportRoot</span></span>](../api/intune_shared_reportroot_update.md)|[<span data-ttu-id="d0902-112">reportRoot</span><span class="sxs-lookup"><span data-stu-id="d0902-112">reportRoot</span></span>](../resources/intune_shared_reportroot.md)|<span data-ttu-id="d0902-113">[reportRoot](../resources/intune_shared_reportroot.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="d0902-113">Update the properties of a [reportRoot](../resources/intune_shared_reportroot.md) object.</span></span>|
|<span data-ttu-id="d0902-114">**デバイス構成**</span><span class="sxs-lookup"><span data-stu-id="d0902-114">**Device configuration**</span></span>|
|[<span data-ttu-id="d0902-115">deviceConfigurationDeviceActivity 関数</span><span class="sxs-lookup"><span data-stu-id="d0902-115">deviceConfigurationDeviceActivity function</span></span>](../api/intune_shared_reportroot_deviceconfigurationdeviceactivity.md)|[<span data-ttu-id="d0902-116">レポート</span><span class="sxs-lookup"><span data-stu-id="d0902-116">report</span></span>](../resources/intune_shared_report.md)|<span data-ttu-id="d0902-117">デバイス構成のデバイス アクティビティ レポートのメタデータ</span><span class="sxs-lookup"><span data-stu-id="d0902-117">Metadata for the device configuration device activity report</span></span>|
|[<span data-ttu-id="d0902-118">deviceConfigurationUserActivity 関数</span><span class="sxs-lookup"><span data-stu-id="d0902-118">deviceConfigurationUserActivity function</span></span>](../api/intune_shared_reportroot_deviceconfigurationuseractivity.md)|[<span data-ttu-id="d0902-119">レポート</span><span class="sxs-lookup"><span data-stu-id="d0902-119">report</span></span>](../resources/intune_shared_report.md)|<span data-ttu-id="d0902-120">デバイス構成のユーザー アクティビティ レポートのメタデータ</span><span class="sxs-lookup"><span data-stu-id="d0902-120">Metadata for the device configuration user activity report</span></span>|
|<span data-ttu-id="d0902-121">**トラブルシューティング**</span><span class="sxs-lookup"><span data-stu-id="d0902-121">**Troubleshooting**</span></span>|
|[<span data-ttu-id="d0902-122">managedDeviceEnrollmentFailureDetails 関数</span><span class="sxs-lookup"><span data-stu-id="d0902-122">managedDeviceEnrollmentFailureDetails function</span></span>](../api/intune_shared_reportroot_manageddeviceenrollmentfailuredetails.md)|[<span data-ttu-id="d0902-123">レポート</span><span class="sxs-lookup"><span data-stu-id="d0902-123">report</span></span>](../resources/intune_shared_report.md)|<span data-ttu-id="d0902-124">まだ文書化されていません。</span><span class="sxs-lookup"><span data-stu-id="d0902-124">Not yet documented</span></span>|
|[<span data-ttu-id="d0902-125">managedDeviceEnrollmentTopFailures 関数</span><span class="sxs-lookup"><span data-stu-id="d0902-125">managedDeviceEnrollmentTopFailures function</span></span>](../api/intune_shared_reportroot_manageddeviceenrollmenttopfailures.md)|[<span data-ttu-id="d0902-126">レポート</span><span class="sxs-lookup"><span data-stu-id="d0902-126">report</span></span>](../resources/intune_shared_report.md)|<span data-ttu-id="d0902-127">まだ文書化されていません。</span><span class="sxs-lookup"><span data-stu-id="d0902-127">Not yet documented</span></span>|


## <a name="properties"></a><span data-ttu-id="d0902-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d0902-128">Properties</span></span>
|<span data-ttu-id="d0902-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d0902-129">Property</span></span>|<span data-ttu-id="d0902-130">型</span><span class="sxs-lookup"><span data-stu-id="d0902-130">Type</span></span>|<span data-ttu-id="d0902-131">説明</span><span class="sxs-lookup"><span data-stu-id="d0902-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d0902-132">ID</span><span class="sxs-lookup"><span data-stu-id="d0902-132">id</span></span>|<span data-ttu-id="d0902-133">文字列</span><span class="sxs-lookup"><span data-stu-id="d0902-133">String</span></span>|<span data-ttu-id="d0902-134">このエンティティの一意識別子です。</span><span class="sxs-lookup"><span data-stu-id="d0902-134">The unique identifier for this entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d0902-135">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d0902-135">Relationships</span></span>
<span data-ttu-id="d0902-136">なし</span><span class="sxs-lookup"><span data-stu-id="d0902-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d0902-137">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d0902-137">JSON Representation</span></span>
<span data-ttu-id="d0902-138">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d0902-138">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.reportRoot"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.reportRoot",
  "id": "String (identifier)"
}
```

## <a name="example"></a><span data-ttu-id="d0902-139">例</span><span class="sxs-lookup"><span data-stu-id="d0902-139">Example</span></span>

<!--{"blockType": "request"}-->
```http
GET https://graph.microsoft.com/v1.0/reports
```

<!--{"blockType": "response", "truncated": true, "@odata.type": "microsoft.graph.reportRoot"}-->
```json
HTTP/1.1 200 OK
Content-Type: application/json

{
}
```