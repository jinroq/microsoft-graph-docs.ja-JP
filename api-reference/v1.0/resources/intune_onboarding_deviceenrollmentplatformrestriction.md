# <a name="deviceenrollmentplatformrestriction-resource-type"></a><span data-ttu-id="e1920-101">deviceEnrollmentPlatformRestriction リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e1920-101">deviceEnrollmentPlatformRestriction resource type</span></span>

> <span data-ttu-id="e1920-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e1920-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e1920-103">プラットフォーム固有の登録の制限</span><span class="sxs-lookup"><span data-stu-id="e1920-103">Platform specific enrollment restrictions</span></span>
## <a name="properties"></a><span data-ttu-id="e1920-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e1920-104">Properties</span></span>
|<span data-ttu-id="e1920-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e1920-105">Property</span></span>|<span data-ttu-id="e1920-106">タイプ</span><span class="sxs-lookup"><span data-stu-id="e1920-106">Type</span></span>|<span data-ttu-id="e1920-107">説明</span><span class="sxs-lookup"><span data-stu-id="e1920-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e1920-108">platformBlocked</span><span class="sxs-lookup"><span data-stu-id="e1920-108">platformBlocked</span></span>|<span data-ttu-id="e1920-109">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="e1920-109">Boolean</span></span>|<span data-ttu-id="e1920-110">登録で対象プラットフォームをブロックします</span><span class="sxs-lookup"><span data-stu-id="e1920-110">Block the platform from enrolling</span></span>|
|<span data-ttu-id="e1920-111">personalDeviceEnrollmentBlocked</span><span class="sxs-lookup"><span data-stu-id="e1920-111">personalDeviceEnrollmentBlocked</span></span>|<span data-ttu-id="e1920-112">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="e1920-112">Boolean</span></span>|<span data-ttu-id="e1920-113">個人所有のデバイスの登録をブロックします</span><span class="sxs-lookup"><span data-stu-id="e1920-113">Block personally owned devices from enrolling</span></span>|
|<span data-ttu-id="e1920-114">osMinimumVersion</span><span class="sxs-lookup"><span data-stu-id="e1920-114">osMinimumVersion</span></span>|<span data-ttu-id="e1920-115">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="e1920-115">String</span></span>|<span data-ttu-id="e1920-116">サポートされる最小 OS バージョン</span><span class="sxs-lookup"><span data-stu-id="e1920-116">Min OS version supported</span></span>|
|<span data-ttu-id="e1920-117">osMaximumVersion</span><span class="sxs-lookup"><span data-stu-id="e1920-117">osMaximumVersion</span></span>|<span data-ttu-id="e1920-118">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="e1920-118">String</span></span>|<span data-ttu-id="e1920-119">サポートされる最大 OS バージョン</span><span class="sxs-lookup"><span data-stu-id="e1920-119">Max OS version supported</span></span>|

## <a name="relationships"></a><span data-ttu-id="e1920-120">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e1920-120">Relationships</span></span>
<span data-ttu-id="e1920-121">なし</span><span class="sxs-lookup"><span data-stu-id="e1920-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e1920-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e1920-122">JSON Representation</span></span>
<span data-ttu-id="e1920-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e1920-123">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.deviceEnrollmentPlatformRestriction"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceEnrollmentPlatformRestriction",
  "platformBlocked": true,
  "personalDeviceEnrollmentBlocked": true,
  "osMinimumVersion": "String",
  "osMaximumVersion": "String"
}
```



