# <a name="microsoftstoreforbusinessappassignmentsettings-resource-type"></a><span data-ttu-id="1de96-101">microsoftStoreForBusinessAppAssignmentSettings リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1de96-101">microsoftStoreForBusinessAppAssignmentSettings resource type</span></span>

> <span data-ttu-id="1de96-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="1de96-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1de96-103">グループに、ビジネス向け Microsoft Store モバイル アプリを割り当てるためのプロパティが含まれます。</span><span class="sxs-lookup"><span data-stu-id="1de96-103">Contains properties used to assign an Microsoft Store for Business mobile app to a group.</span></span>

<span data-ttu-id="1de96-104">[mobileAppAssignmentSettings](../resources/intune_apps_mobileappassignmentsettings.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="1de96-104">Inherits from [mobileAppAssignmentSettings](../resources/intune_apps_mobileappassignmentsettings.md)</span></span>

## <a name="properties"></a><span data-ttu-id="1de96-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1de96-105">Properties</span></span>
|<span data-ttu-id="1de96-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1de96-106">Property</span></span>|<span data-ttu-id="1de96-107">型</span><span class="sxs-lookup"><span data-stu-id="1de96-107">Type</span></span>|<span data-ttu-id="1de96-108">説明</span><span class="sxs-lookup"><span data-stu-id="1de96-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1de96-109">useDeviceContext</span><span class="sxs-lookup"><span data-stu-id="1de96-109">useDeviceContext</span></span>|<span data-ttu-id="1de96-110">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="1de96-110">Boolean</span></span>|<span data-ttu-id="1de96-111">ビジネス向け Microsoft Store モバイル アプリのデバイス実行コンテキストを使用するかどうか。</span><span class="sxs-lookup"><span data-stu-id="1de96-111">Whether or not to use device execution context for Microsoft Store for Business mobile app.</span></span>|

## <a name="relationships"></a><span data-ttu-id="1de96-112">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1de96-112">Relationships</span></span>
<span data-ttu-id="1de96-113">なし</span><span class="sxs-lookup"><span data-stu-id="1de96-113">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1de96-114">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1de96-114">JSON Representation</span></span>
<span data-ttu-id="1de96-115">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1de96-115">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.microsoftStoreForBusinessAppAssignmentSettings"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessAppAssignmentSettings",
  "useDeviceContext": true
}
```



