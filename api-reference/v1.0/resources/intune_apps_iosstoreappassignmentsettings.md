# <a name="iosstoreappassignmentsettings-resource-type"></a><span data-ttu-id="a349e-101">iosStoreAppAssignmentSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a349e-101">iosStoreAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="a349e-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="a349e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a349e-103">グループへの iOS ストア モバイル アプリの割り当てに使用されるプロパティが、含まれています。</span><span class="sxs-lookup"><span data-stu-id="a349e-103">Contains properties used to assign an iOS Store mobile app to a group.</span></span>

<span data-ttu-id="a349e-104">[mobileAppAssignmentSettings](../resources/intune_apps_mobileappassignmentsettings.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="a349e-104">Inherits from [mobileAppAssignmentSettings](../resources/intune_apps_mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="a349e-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a349e-105">Properties</span></span>
|<span data-ttu-id="a349e-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a349e-106">Property</span></span>|<span data-ttu-id="a349e-107">型</span><span class="sxs-lookup"><span data-stu-id="a349e-107">Type</span></span>|<span data-ttu-id="a349e-108">説明</span><span class="sxs-lookup"><span data-stu-id="a349e-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a349e-109">vpnConfigurationId</span><span class="sxs-lookup"><span data-stu-id="a349e-109">vpnConfigurationId</span></span>|<span data-ttu-id="a349e-110">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="a349e-110">String</span></span>|<span data-ttu-id="a349e-111">このアプリに適用するための VPN 構成 ID。</span><span class="sxs-lookup"><span data-stu-id="a349e-111">The VPN Configuration Id to apply for this app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a349e-112">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a349e-112">Relationships</span></span>
<span data-ttu-id="a349e-113">なし</span><span class="sxs-lookup"><span data-stu-id="a349e-113">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a349e-114">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a349e-114">JSON Representation</span></span>
<span data-ttu-id="a349e-115">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a349e-115">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosStoreAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosStoreAppAssignmentSettings",
  "vpnConfigurationId": "String"
}
```



