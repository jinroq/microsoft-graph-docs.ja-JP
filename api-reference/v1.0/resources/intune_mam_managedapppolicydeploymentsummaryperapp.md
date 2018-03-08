# <a name="managedapppolicydeploymentsummaryperapp-resource-type"></a><span data-ttu-id="8aeac-101">managedAppPolicyDeploymentSummaryPerApp リソースの種類</span><span class="sxs-lookup"><span data-stu-id="8aeac-101">managedAppPolicyDeploymentSummaryPerApp resource type</span></span>

> <span data-ttu-id="8aeac-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="8aeac-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8aeac-103">アプリごとのポリシーの展開の概要を表します。</span><span class="sxs-lookup"><span data-stu-id="8aeac-103">Represents policy deployment summary per app.</span></span>
## <a name="properties"></a><span data-ttu-id="8aeac-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8aeac-104">Properties</span></span>
|<span data-ttu-id="8aeac-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8aeac-105">Property</span></span>|<span data-ttu-id="8aeac-106">型</span><span class="sxs-lookup"><span data-stu-id="8aeac-106">Type</span></span>|<span data-ttu-id="8aeac-107">説明</span><span class="sxs-lookup"><span data-stu-id="8aeac-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8aeac-108">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="8aeac-108">mobileAppIdentifier</span></span>|[<span data-ttu-id="8aeac-109">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="8aeac-109">mobileAppIdentifier</span></span>](../resources/intune_mam_mobileappidentifier.md)|<span data-ttu-id="8aeac-110">アプリの展開</span><span class="sxs-lookup"><span data-stu-id="8aeac-110">Deployment of an app.</span></span>|
|<span data-ttu-id="8aeac-111">configurationAppliedUserCount</span><span class="sxs-lookup"><span data-stu-id="8aeac-111">configurationAppliedUserCount</span></span>|<span data-ttu-id="8aeac-112">Int32</span><span class="sxs-lookup"><span data-stu-id="8aeac-112">Int32</span></span>|<span data-ttu-id="8aeac-113">ポリシーが適用されているユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="8aeac-113">Number of users the policy is applied.</span></span>|

## <a name="relationships"></a><span data-ttu-id="8aeac-114">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="8aeac-114">Relationships</span></span>
<span data-ttu-id="8aeac-115">なし</span><span class="sxs-lookup"><span data-stu-id="8aeac-115">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="8aeac-116">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="8aeac-116">JSON Representation</span></span>
<span data-ttu-id="8aeac-117">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="8aeac-117">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppPolicyDeploymentSummaryPerApp"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppPolicyDeploymentSummaryPerApp",
  "mobileAppIdentifier": {
    "@odata.type": "microsoft.graph.mobileAppIdentifier"
  },
  "configurationAppliedUserCount": 1024
}
```


