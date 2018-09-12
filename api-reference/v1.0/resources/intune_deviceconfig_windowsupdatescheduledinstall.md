# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="d72c5-101">windowsUpdateScheduledInstall リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d72c5-101">windowsUpdateScheduledInstall resource type</span></span>

> <span data-ttu-id="d72c5-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="d72c5-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d72c5-103">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="d72c5-103">Not yet documented</span></span>

<span data-ttu-id="d72c5-104">[windowsUpdateInstallScheduleType](../resources/intune_deviceconfig_windowsupdateinstallscheduletype.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="d72c5-104">Inherits from [windowsUpdateInstallScheduleType](../resources/intune_deviceconfig_windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="d72c5-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d72c5-105">Properties</span></span>
|<span data-ttu-id="d72c5-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d72c5-106">Property</span></span>|<span data-ttu-id="d72c5-107">タイプ</span><span class="sxs-lookup"><span data-stu-id="d72c5-107">Type</span></span>|<span data-ttu-id="d72c5-108">説明</span><span class="sxs-lookup"><span data-stu-id="d72c5-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d72c5-109">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="d72c5-109">scheduledInstallDay</span></span>|[<span data-ttu-id="d72c5-110">weeklySchedule</span><span class="sxs-lookup"><span data-stu-id="d72c5-110">weeklySchedule</span></span>](../resources/intune_deviceconfig_weeklyschedule.md)|<span data-ttu-id="d72c5-p101">スケジュールされたインストール日 (曜日)。可能な値は `userDefined`、`everyday`、`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday`、`saturday` です。</span><span class="sxs-lookup"><span data-stu-id="d72c5-p101">Scheduled Install Day in week Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="d72c5-113">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="d72c5-113">scheduledInstallTime</span></span>|<span data-ttu-id="d72c5-114">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="d72c5-114">TimeOfDay</span></span>|<span data-ttu-id="d72c5-115">スケジュールされたインストール時刻</span><span class="sxs-lookup"><span data-stu-id="d72c5-115">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="d72c5-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d72c5-116">Relationships</span></span>
<span data-ttu-id="d72c5-117">なし</span><span class="sxs-lookup"><span data-stu-id="d72c5-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d72c5-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d72c5-118">JSON Representation</span></span>
<span data-ttu-id="d72c5-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d72c5-119">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsUpdateScheduledInstall"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdateScheduledInstall",
  "scheduledInstallDay": "String",
  "scheduledInstallTime": "String (time of day)"
}
```








