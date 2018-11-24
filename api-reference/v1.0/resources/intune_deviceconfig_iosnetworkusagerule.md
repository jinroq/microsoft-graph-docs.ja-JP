# <a name="iosnetworkusagerule-resource-type"></a><span data-ttu-id="069ef-101">iosNetworkUsageRule リソースの種類</span><span class="sxs-lookup"><span data-stu-id="069ef-101">iosNetworkUsageRule resource type</span></span>

> <span data-ttu-id="069ef-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="069ef-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="069ef-103">ネットワーク使用規則により、企業は管理対象アプリで携帯電話会社の回線などのネットワークをどのように使用するかを指定できます。</span><span class="sxs-lookup"><span data-stu-id="069ef-103">Network Usage Rules allow enterprises to specify how managed apps use networks, such as cellular data networks.</span></span>
## <a name="properties"></a><span data-ttu-id="069ef-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="069ef-104">Properties</span></span>
|<span data-ttu-id="069ef-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="069ef-105">Property</span></span>|<span data-ttu-id="069ef-106">型</span><span class="sxs-lookup"><span data-stu-id="069ef-106">Type</span></span>|<span data-ttu-id="069ef-107">説明</span><span class="sxs-lookup"><span data-stu-id="069ef-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="069ef-108">managedApps</span><span class="sxs-lookup"><span data-stu-id="069ef-108">managedApps</span></span>|<span data-ttu-id="069ef-109">[appListItem](../resources/intune_deviceconfig_applistitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="069ef-109">[appListItem](../resources/intune_deviceconfig_applistitem.md) collection</span></span>|<span data-ttu-id="069ef-110">このルールが適用される管理対象アプリに関する情報です。</span><span class="sxs-lookup"><span data-stu-id="069ef-110">Information about the managed apps that this rule is going to apply to.</span></span> <span data-ttu-id="069ef-111">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="069ef-111">This collection can contain a maximum of 500 elements.</span></span>|
|<span data-ttu-id="069ef-112">cellularDataBlockWhenRoaming</span><span class="sxs-lookup"><span data-stu-id="069ef-112">cellularDataBlockWhenRoaming</span></span>|<span data-ttu-id="069ef-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="069ef-113">Boolean</span></span>|<span data-ttu-id="069ef-114">true に設定すると、ローミングの際、対応する管理対象アプリで携帯電話データを使用できなくなります。</span><span class="sxs-lookup"><span data-stu-id="069ef-114">If set to true, corresponding managed apps will not be allowed to use cellular data when roaming.</span></span>|
|<span data-ttu-id="069ef-115">cellularDataBlocked</span><span class="sxs-lookup"><span data-stu-id="069ef-115">cellularDataBlocked</span></span>|<span data-ttu-id="069ef-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="069ef-116">Boolean</span></span>|<span data-ttu-id="069ef-117">true に設定すると、いかなる場合でも、対応する管理対象アプリで携帯電話データを使用できなくなります。</span><span class="sxs-lookup"><span data-stu-id="069ef-117">If set to true, corresponding managed apps will not be allowed to use cellular data at any time.</span></span>|

## <a name="relationships"></a><span data-ttu-id="069ef-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="069ef-118">Relationships</span></span>
<span data-ttu-id="069ef-119">なし</span><span class="sxs-lookup"><span data-stu-id="069ef-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="069ef-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="069ef-120">JSON Representation</span></span>
<span data-ttu-id="069ef-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="069ef-121">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
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



