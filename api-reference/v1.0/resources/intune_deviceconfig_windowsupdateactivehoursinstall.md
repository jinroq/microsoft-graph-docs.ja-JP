# <a name="windowsupdateactivehoursinstall-resource-type"></a><span data-ttu-id="37954-101">windowsUpdateActiveHoursInstall リソースの種類</span><span class="sxs-lookup"><span data-stu-id="37954-101">windowsUpdateActiveHoursInstall resource type</span></span>

> <span data-ttu-id="37954-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="37954-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="37954-103">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="37954-103">Not yet documented</span></span>

<span data-ttu-id="37954-104">[windowsUpdateInstallScheduleType](../resources/intune_deviceconfig_windowsupdateinstallscheduletype.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="37954-104">Inherits from [windowsUpdateInstallScheduleType](../resources/intune_deviceconfig_windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="37954-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="37954-105">Properties</span></span>
|<span data-ttu-id="37954-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="37954-106">Property</span></span>|<span data-ttu-id="37954-107">型</span><span class="sxs-lookup"><span data-stu-id="37954-107">Type</span></span>|<span data-ttu-id="37954-108">説明</span><span class="sxs-lookup"><span data-stu-id="37954-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37954-109">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="37954-109">activeHoursStart</span></span>|<span data-ttu-id="37954-110">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="37954-110">TimeOfDay</span></span>|<span data-ttu-id="37954-111">アクティブ時間の開始</span><span class="sxs-lookup"><span data-stu-id="37954-111">Active Hours Start</span></span>|
|<span data-ttu-id="37954-112">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="37954-112">activeHoursEnd</span></span>|<span data-ttu-id="37954-113">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="37954-113">TimeOfDay</span></span>|<span data-ttu-id="37954-114">アクティブ時間の終了</span><span class="sxs-lookup"><span data-stu-id="37954-114">Active Hours End</span></span>|

## <a name="relationships"></a><span data-ttu-id="37954-115">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="37954-115">Relationships</span></span>
<span data-ttu-id="37954-116">なし</span><span class="sxs-lookup"><span data-stu-id="37954-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="37954-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="37954-117">JSON Representation</span></span>
<span data-ttu-id="37954-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="37954-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUpdateActiveHoursInstall"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdateActiveHoursInstall",
  "activeHoursStart": "String (time of day)",
  "activeHoursEnd": "String (time of day)"
}
```



