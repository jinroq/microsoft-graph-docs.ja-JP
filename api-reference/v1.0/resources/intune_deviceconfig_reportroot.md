# <a name="reportroot-resource-type"></a><span data-ttu-id="b8047-101">reportRoot リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b8047-101">reportRoot resource type</span></span>

> <span data-ttu-id="b8047-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b8047-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b8047-103">履歴レポートのインスタンスを表すリソースです。</span><span class="sxs-lookup"><span data-stu-id="b8047-103">The resource that represents an instance of History Reports.</span></span>
## <a name="methods"></a><span data-ttu-id="b8047-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="b8047-104">Methods</span></span>
|<span data-ttu-id="b8047-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="b8047-105">Method</span></span>|<span data-ttu-id="b8047-106">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="b8047-106">Return Type</span></span>|<span data-ttu-id="b8047-107">説明</span><span class="sxs-lookup"><span data-stu-id="b8047-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b8047-108">ReportRoot の取得</span><span class="sxs-lookup"><span data-stu-id="b8047-108">Get reportRoot</span></span>](../api/intune_deviceconfig_reportroot_get.md)|[<span data-ttu-id="b8047-109">reportRoot</span><span class="sxs-lookup"><span data-stu-id="b8047-109">reportRoot</span></span>](../resources/intune_deviceconfig_reportroot.md)|<span data-ttu-id="b8047-110">[reportRoot](../resources/intune_deviceconfig_reportroot.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="b8047-110">Read properties and relationships of the [reportRoot](../resources/intune_deviceconfig_reportroot.md) object.</span></span>|
|[<span data-ttu-id="b8047-111">reportRoot の更新</span><span class="sxs-lookup"><span data-stu-id="b8047-111">Update reportRoot</span></span>](../api/intune_deviceconfig_reportroot_update.md)|[<span data-ttu-id="b8047-112">reportRoot</span><span class="sxs-lookup"><span data-stu-id="b8047-112">reportRoot</span></span>](../resources/intune_deviceconfig_reportroot.md)|<span data-ttu-id="b8047-113">[reportRoot](../resources/intune_deviceconfig_reportroot.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="b8047-113">Update the properties of a [reportRoot](../resources/intune_deviceconfig_reportroot.md) object.</span></span>|
|[<span data-ttu-id="b8047-114">deviceConfigurationUserActivity function</span><span class="sxs-lookup"><span data-stu-id="b8047-114">deviceConfigurationUserActivity function</span></span>](../api/intune_deviceconfig_reportroot_deviceconfigurationuseractivity.md)|[<span data-ttu-id="b8047-115">レポート</span><span class="sxs-lookup"><span data-stu-id="b8047-115">report</span></span>](../resources/intune_deviceconfig_report.md)|<span data-ttu-id="b8047-116">デバイス構成のユーザー アクティビティ レポートのメタデータ</span><span class="sxs-lookup"><span data-stu-id="b8047-116">Metadata for the device configuration user activity report</span></span>|
|[<span data-ttu-id="b8047-117">deviceConfigurationDeviceActivity function</span><span class="sxs-lookup"><span data-stu-id="b8047-117">deviceConfigurationDeviceActivity function</span></span>](../api/intune_deviceconfig_reportroot_deviceconfigurationdeviceactivity.md)|[<span data-ttu-id="b8047-118">レポート</span><span class="sxs-lookup"><span data-stu-id="b8047-118">report</span></span>](../resources/intune_deviceconfig_report.md)|<span data-ttu-id="b8047-119">デバイス構成のデバイス アクティビティ レポートのメタデータ</span><span class="sxs-lookup"><span data-stu-id="b8047-119">Metadata for the device configuration device activity report</span></span>|

## <a name="relationships"></a><span data-ttu-id="b8047-120">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b8047-120">Relationships</span></span>
<span data-ttu-id="b8047-121">なし</span><span class="sxs-lookup"><span data-stu-id="b8047-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="b8047-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b8047-122">JSON Representation</span></span>
<span data-ttu-id="b8047-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b8047-123">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.reportRoot"
}-->
``` json
{
}
```

## <a name="example"></a><span data-ttu-id="b8047-124">例</span><span class="sxs-lookup"><span data-stu-id="b8047-124">Example</span></span>

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
