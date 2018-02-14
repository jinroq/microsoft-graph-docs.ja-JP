# <a name="iosvppappassignmentsettings-resource-type"></a><span data-ttu-id="23019-101">iosVppAppAssignmentSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="23019-101">iosVppAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="23019-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="23019-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="23019-103">グループへの iOS VPP モバイル アプリの割り当てに使用されるプロパティが、含まれています。</span><span class="sxs-lookup"><span data-stu-id="23019-103">Contains properties used to assign an iOS VPP mobile app to a group.</span></span>

<span data-ttu-id="23019-104">[mobileAppAssignmentSettings](../resources/intune_apps_mobileappassignmentsettings.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="23019-104">Inherits from [mobileAppAssignmentSettings](../resources/intune_apps_mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="23019-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="23019-105">Properties</span></span>
|<span data-ttu-id="23019-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="23019-106">Property</span></span>|<span data-ttu-id="23019-107">型</span><span class="sxs-lookup"><span data-stu-id="23019-107">Type</span></span>|<span data-ttu-id="23019-108">説明</span><span class="sxs-lookup"><span data-stu-id="23019-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="23019-109">useDeviceLicensing</span><span class="sxs-lookup"><span data-stu-id="23019-109">useDeviceLicensing</span></span>|<span data-ttu-id="23019-110">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="23019-110">Boolean</span></span>|<span data-ttu-id="23019-111">デバイスのライセンスを使用するかどうか。</span><span class="sxs-lookup"><span data-stu-id="23019-111">Whether or not to use device licensing.</span></span>|
|<span data-ttu-id="23019-112">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="23019-112">vpnConfigurationId</span></span>|<span data-ttu-id="23019-113">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="23019-113">String</span></span>|<span data-ttu-id="23019-114">このアプリに適用するための VPN 構成 ID。</span><span class="sxs-lookup"><span data-stu-id="23019-114">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="23019-115">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="23019-115">Relationships</span></span>
<span data-ttu-id="23019-116">なし</span><span class="sxs-lookup"><span data-stu-id="23019-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="23019-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="23019-117">JSON Representation</span></span>
<span data-ttu-id="23019-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="23019-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosVppAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosVppAppAssignmentSettings",
  "useDeviceLicensing": true,
  "vpnConfigurationId": "String"
}
```



