# <a name="windowsupdatescheduledinstall-resource-type"></a><span data-ttu-id="183e8-101">windowsUpdateScheduledInstall リソースの種類</span><span class="sxs-lookup"><span data-stu-id="183e8-101">windowsUpdateScheduledInstall resource type</span></span>

> <span data-ttu-id="183e8-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="183e8-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="183e8-103">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="183e8-103">Not yet documented</span></span>

<span data-ttu-id="183e8-104">[windowsUpdateInstallScheduleType](../resources/intune_deviceconfig_windowsupdateinstallscheduletype.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="183e8-104">Inherits from [windowsUpdateInstallScheduleType](../resources/intune_deviceconfig_windowsupdateinstallscheduletype.md)</span></span>

## <a name="properties"></a><span data-ttu-id="183e8-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="183e8-105">Properties</span></span>
|<span data-ttu-id="183e8-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="183e8-106">Property</span></span>|<span data-ttu-id="183e8-107">型</span><span class="sxs-lookup"><span data-stu-id="183e8-107">Type</span></span>|<span data-ttu-id="183e8-108">説明</span><span class="sxs-lookup"><span data-stu-id="183e8-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="183e8-109">scheduledInstallDay</span><span class="sxs-lookup"><span data-stu-id="183e8-109">scheduledInstallDay</span></span>|<span data-ttu-id="183e8-110">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="183e8-110">String</span></span>|<span data-ttu-id="183e8-111">スケジュールされたインストール日 (曜日)。可能な値: `userDefined`、`everyday`、`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday`、`saturday`。</span><span class="sxs-lookup"><span data-stu-id="183e8-111">Scheduled Install Day in week Possible values are: `userDefined`, `everyday`, `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="183e8-112">scheduledInstallTime</span><span class="sxs-lookup"><span data-stu-id="183e8-112">scheduledInstallTime</span></span>|<span data-ttu-id="183e8-113">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="183e8-113">TimeOfDay</span></span>|<span data-ttu-id="183e8-114">スケジュールされたインストール時刻</span><span class="sxs-lookup"><span data-stu-id="183e8-114">Scheduled Install Time during day</span></span>|

## <a name="relationships"></a><span data-ttu-id="183e8-115">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="183e8-115">Relationships</span></span>
<span data-ttu-id="183e8-116">なし</span><span class="sxs-lookup"><span data-stu-id="183e8-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="183e8-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="183e8-117">JSON Representation</span></span>
<span data-ttu-id="183e8-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="183e8-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.windowsUpdateScheduledInstall"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsUpdateScheduledInstall",
  "scheduledInstallDay": "String",
  "scheduledInstallTime": "String (time of day)"
}
```



