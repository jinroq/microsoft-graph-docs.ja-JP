# <a name="iosnetworkusagerule-resource-type"></a><span data-ttu-id="a13c4-101">iosNetworkUsageRule リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a13c4-101">iosNetworkUsageRule resource type</span></span>

> <span data-ttu-id="a13c4-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="a13c4-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a13c4-103">ネットワーク使用規則により、企業は管理対象アプリで携帯電話会社の回線などのネットワークをどのように使用するかを指定できます。</span><span class="sxs-lookup"><span data-stu-id="a13c4-103">Network Usage Rules allow enterprises to specify how managed apps use networks, such as cellular data networks.</span></span>
## <a name="properties"></a><span data-ttu-id="a13c4-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a13c4-104">Properties</span></span>
|<span data-ttu-id="a13c4-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a13c4-105">Property</span></span>|<span data-ttu-id="a13c4-106">型</span><span class="sxs-lookup"><span data-stu-id="a13c4-106">Type</span></span>|<span data-ttu-id="a13c4-107">説明</span><span class="sxs-lookup"><span data-stu-id="a13c4-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a13c4-108">managedApps</span><span class="sxs-lookup"><span data-stu-id="a13c4-108">managedApps</span></span>|<span data-ttu-id="a13c4-109">[appListItem](../resources/intune_deviceconfig_applistitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a13c4-109">[appListItem](../resources/intune_deviceconfig_applistitem.md) collection</span></span>|<span data-ttu-id="a13c4-110">このルールが適用される管理対象アプリに関する情報です。</span><span class="sxs-lookup"><span data-stu-id="a13c4-110">Information about the managed apps that this rule is going to apply to.</span></span> <span data-ttu-id="a13c4-111">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="a13c4-111">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="a13c4-112">cellularDataBlockWhenRoaming</span><span class="sxs-lookup"><span data-stu-id="a13c4-112">cellularDataBlockWhenRoaming</span></span>|<span data-ttu-id="a13c4-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="a13c4-113">Boolean</span></span>|<span data-ttu-id="a13c4-114">true に設定すると、ローミングの際、対応する管理対象アプリで携帯電話データを使用できなくなります。</span><span class="sxs-lookup"><span data-stu-id="a13c4-114">If set to true, corresponding managed apps will not be allowed to use cellular data when roaming.</span></span>|
|<span data-ttu-id="a13c4-115">cellularDataBlocked</span><span class="sxs-lookup"><span data-stu-id="a13c4-115">cellularDataBlocked</span></span>|<span data-ttu-id="a13c4-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="a13c4-116">Boolean</span></span>|<span data-ttu-id="a13c4-117">true に設定すると、いかなる場合でも、対応する管理対象アプリで携帯電話データを使用できなくなります。</span><span class="sxs-lookup"><span data-stu-id="a13c4-117">If set to true, corresponding managed apps will not be allowed to use cellular data at any time.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a13c4-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a13c4-118">Relationships</span></span>
<span data-ttu-id="a13c4-119">なし</span><span class="sxs-lookup"><span data-stu-id="a13c4-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="a13c4-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a13c4-120">JSON Representation</span></span>
<span data-ttu-id="a13c4-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a13c4-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosNetworkUsageRule"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosNetworkUsageRule",
  "managedApps": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "String",
      "publisher": "String",
      "appStoreUrl": "String",
      "appId": "String"
    }
  ],
  "cellularDataBlockWhenRoaming": true,
  "cellularDataBlocked": true
}
```



