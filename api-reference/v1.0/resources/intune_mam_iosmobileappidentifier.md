# <a name="iosmobileappidentifier-resource-type"></a><span data-ttu-id="f17d0-101">iosMobileAppIdentifier リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f17d0-101">iosMobileAppIdentifier resource type</span></span>

> <span data-ttu-id="f17d0-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f17d0-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f17d0-103">iOS アプリの識別子。</span><span class="sxs-lookup"><span data-stu-id="f17d0-103">The identifier for an iOS app.</span></span>

<span data-ttu-id="f17d0-104">[mobileAppIdentifier](../resources/intune_mam_mobileappidentifier.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="f17d0-104">Inherits from [mobileAppIdentifier](../resources/intune_mam_mobileappidentifier.md)</span></span>

## <a name="properties"></a><span data-ttu-id="f17d0-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f17d0-105">Properties</span></span>
|<span data-ttu-id="f17d0-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f17d0-106">Property</span></span>|<span data-ttu-id="f17d0-107">型</span><span class="sxs-lookup"><span data-stu-id="f17d0-107">Type</span></span>|<span data-ttu-id="f17d0-108">説明</span><span class="sxs-lookup"><span data-stu-id="f17d0-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f17d0-109">bundleId</span><span class="sxs-lookup"><span data-stu-id="f17d0-109">bundleId</span></span>|<span data-ttu-id="f17d0-110">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="f17d0-110">String</span></span>|<span data-ttu-id="f17d0-111">App Store で指定されている、アプリの識別子。</span><span class="sxs-lookup"><span data-stu-id="f17d0-111">The identifier for an app, as specified in the app store.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f17d0-112">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f17d0-112">Relationships</span></span>
<span data-ttu-id="f17d0-113">なし</span><span class="sxs-lookup"><span data-stu-id="f17d0-113">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="f17d0-114">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f17d0-114">JSON Representation</span></span>
<span data-ttu-id="f17d0-115">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f17d0-115">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.iosMobileAppIdentifier"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.iosMobileAppIdentifier",
  "bundleId": "String"
}
```








