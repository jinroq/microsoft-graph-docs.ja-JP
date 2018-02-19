# <a name="devicemanagementsettings-resource-type"></a><span data-ttu-id="dcfb7-101">deviceManagementSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="dcfb7-101">deviceManagementSettings resource type</span></span>

> <span data-ttu-id="dcfb7-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="dcfb7-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dcfb7-103">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="dcfb7-103">Not yet documented</span></span>
## <a name="properties"></a><span data-ttu-id="dcfb7-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dcfb7-104">Properties</span></span>
|<span data-ttu-id="dcfb7-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dcfb7-105">Property</span></span>|<span data-ttu-id="dcfb7-106">型</span><span class="sxs-lookup"><span data-stu-id="dcfb7-106">Type</span></span>|<span data-ttu-id="dcfb7-107">説明</span><span class="sxs-lookup"><span data-stu-id="dcfb7-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dcfb7-108">deviceComplianceCheckinThresholdDays</span><span class="sxs-lookup"><span data-stu-id="dcfb7-108">deviceComplianceCheckinThresholdDays</span></span>|<span data-ttu-id="dcfb7-109">Int32</span><span class="sxs-lookup"><span data-stu-id="dcfb7-109">Int32</span></span>|<span data-ttu-id="dcfb7-110">デバイスがチェックインせずに移動し、準拠性を維持できる日数です。</span><span class="sxs-lookup"><span data-stu-id="dcfb7-110">The number of days a device is allowed to go without checking in to remain compliant.</span></span> <span data-ttu-id="dcfb7-111">有効な値は 0 から 120 までです</span><span class="sxs-lookup"><span data-stu-id="dcfb7-111">Valid values 0 to 120</span></span>|
|<span data-ttu-id="dcfb7-112">isScheduledActionEnabled</span><span class="sxs-lookup"><span data-stu-id="dcfb7-112">isScheduledActionEnabled</span></span>|<span data-ttu-id="dcfb7-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="dcfb7-113">Boolean</span></span>|<span data-ttu-id="dcfb7-114">ルールのスケジュール済みアクションの機能が有効かどうか。</span><span class="sxs-lookup"><span data-stu-id="dcfb7-114">Is feature enabled or not for scheduled action for rule.</span></span>|
|<span data-ttu-id="dcfb7-115">secureByDefault</span><span class="sxs-lookup"><span data-stu-id="dcfb7-115">secureByDefault</span></span>|<span data-ttu-id="dcfb7-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="dcfb7-116">Boolean</span></span>|<span data-ttu-id="dcfb7-117">これが true の場合に、対象となるコンプライアンス ポリシーがないと、デバイスは非準拠となります</span><span class="sxs-lookup"><span data-stu-id="dcfb7-117">Device should be noncompliant when there is no compliance policy targeted when this is true</span></span>|

## <a name="relationships"></a><span data-ttu-id="dcfb7-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="dcfb7-118">Relationships</span></span>
<span data-ttu-id="dcfb7-119">なし</span><span class="sxs-lookup"><span data-stu-id="dcfb7-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="dcfb7-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="dcfb7-120">JSON Representation</span></span>
<span data-ttu-id="dcfb7-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="dcfb7-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementSettings",
  "deviceComplianceCheckinThresholdDays": 1024,
  "isScheduledActionEnabled": true,
  "secureByDefault": true
}
```



