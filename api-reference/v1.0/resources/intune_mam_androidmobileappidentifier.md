# <a name="androidmobileappidentifier-resource-type"></a><span data-ttu-id="dcc97-101">androidMobileAppIdentifier リソースの種類</span><span class="sxs-lookup"><span data-stu-id="dcc97-101">androidMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="dcc97-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="dcc97-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dcc97-103">Android アプリの識別子。</span><span class="sxs-lookup"><span data-stu-id="dcc97-103">The identifier for an Android app.</span></span>

<span data-ttu-id="dcc97-104">[mobileAppIdentifier](../resources/intune_mam_mobileappidentifier.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="dcc97-104">Inherits from [mobileAppIdentifier](../resources/intune_mam_mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="dcc97-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dcc97-105">Properties</span></span>
|<span data-ttu-id="dcc97-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dcc97-106">Property</span></span>|<span data-ttu-id="dcc97-107">型</span><span class="sxs-lookup"><span data-stu-id="dcc97-107">Type</span></span>|<span data-ttu-id="dcc97-108">説明</span><span class="sxs-lookup"><span data-stu-id="dcc97-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dcc97-109">packageId</span><span class="sxs-lookup"><span data-stu-id="dcc97-109">packageId</span></span>|<span data-ttu-id="dcc97-110">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="dcc97-110">String</span></span>|<span data-ttu-id="dcc97-111">Play ストアで指定されている、アプリの識別子。</span><span class="sxs-lookup"><span data-stu-id="dcc97-111">The identifier for an app, as specified in the play store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="dcc97-112">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="dcc97-112">Relationships</span></span>
<span data-ttu-id="dcc97-113">なし</span><span class="sxs-lookup"><span data-stu-id="dcc97-113">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="dcc97-114">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="dcc97-114">JSON Representation</span></span>
<span data-ttu-id="dcc97-115">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="dcc97-115">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.androidMobileAppIdentifier"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidMobileAppIdentifier",
  "packageId": "String"
}
```



