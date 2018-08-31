# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="37e5f-101">windowsUpdateScheduledInstall リソースの種類</span><span class="sxs-lookup"><span data-stu-id="37e5f-101">windowsUpdateScheduledInstall resource type</span></span>

> <span data-ttu-id="37e5f-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="37e5f-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="37e5f-103">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="37e5f-103">Not yet documented</span></span>

<span data-ttu-id="37e5f-104">[windowsUpdateInstallScheduleType](../resources/intune_deviceconfig_windowsupdateinstallscheduletype.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="37e5f-104">Inherits from [windowsUpdateInstallScheduleType](../resources/intune_deviceconfig_windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="37e5f-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="37e5f-105">Properties</span></span>
|<span data-ttu-id="37e5f-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="37e5f-106">Property</span></span>|<span data-ttu-id="37e5f-107">タイプ</span><span class="sxs-lookup"><span data-stu-id="37e5f-107">Type</span></span>|<span data-ttu-id="37e5f-108">説明</span><span class="sxs-lookup"><span data-stu-id="37e5f-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37e5f-109">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="37e5f-109">scheduledInstallDay</span></span>|[<span data-ttu-id="37e5f-110">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="37e5f-110">weeklySchedule</span></span>](../resources/intune_deviceconfig_weeklyschedule.md)|<span data-ttu-id="37e5f-111">スケジュールされたインストールの週の曜日です。</span><span class="sxs-lookup"><span data-stu-id="37e5f-111">Scheduled Install Day in week Possible values are: , , , , , , , , .</span></span> <span data-ttu-id="37e5f-112">可能な値は、`userDefined`、`everyday`、`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday`、`saturday` です。</span><span class="sxs-lookup"><span data-stu-id="37e5f-112">The possible values are `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`, , , or .</span></span>|
|<span data-ttu-id="37e5f-113">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="37e5f-113">scheduledInstallTime</span></span>|<span data-ttu-id="37e5f-114">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="37e5f-114">TimeOfDay</span></span>|<span data-ttu-id="37e5f-115">スケジュールされたインストール時刻</span><span class="sxs-lookup"><span data-stu-id="37e5f-115">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="37e5f-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="37e5f-116">Relationships</span></span>
<span data-ttu-id="37e5f-117">なし</span><span class="sxs-lookup"><span data-stu-id="37e5f-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="37e5f-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="37e5f-118">JSON Representation</span></span>
<span data-ttu-id="37e5f-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="37e5f-119">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.windowsUpdateInstallScheduleType",
  "@odata.type": "microsoft.graph.windowsUpdateScheduledInstall"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdateScheduledInstall",
  "scheduledInstallDay": "String",
  "scheduledInstallTime": "String (time of day)"
}
```



