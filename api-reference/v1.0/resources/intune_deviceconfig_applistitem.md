# <a name="applistitem-resource-type"></a><span data-ttu-id="70abb-101">appListItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="70abb-101">appListItem resource type</span></span>

> <span data-ttu-id="70abb-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="70abb-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="70abb-103">管理対象アプリケーションの一覧にあるアプリを表します</span><span class="sxs-lookup"><span data-stu-id="70abb-103">Represents an app in the list of managed applications</span></span>
## <a name="properties"></a><span data-ttu-id="70abb-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="70abb-104">Properties</span></span>
|<span data-ttu-id="70abb-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="70abb-105">Property</span></span>|<span data-ttu-id="70abb-106">タイプ</span><span class="sxs-lookup"><span data-stu-id="70abb-106">Type</span></span>|<span data-ttu-id="70abb-107">説明</span><span class="sxs-lookup"><span data-stu-id="70abb-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="70abb-108">name</span><span class="sxs-lookup"><span data-stu-id="70abb-108">name</span></span>|<span data-ttu-id="70abb-109">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="70abb-109">String</span></span>|<span data-ttu-id="70abb-110">アプリケーション名</span><span class="sxs-lookup"><span data-stu-id="70abb-110">The application name</span></span>|
|<span data-ttu-id="70abb-111">発行元</span><span class="sxs-lookup"><span data-stu-id="70abb-111">publisher</span></span>|<span data-ttu-id="70abb-112">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="70abb-112">String</span></span>|<span data-ttu-id="70abb-113">アプリケーションの発行元</span><span class="sxs-lookup"><span data-stu-id="70abb-113">The publisher of the application</span></span>|
|<span data-ttu-id="70abb-114">appStoreUrl</span><span class="sxs-lookup"><span data-stu-id="70abb-114">appStoreUrl</span></span>|<span data-ttu-id="70abb-115">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="70abb-115">String</span></span>|<span data-ttu-id="70abb-116">アプリケーションのストア URL</span><span class="sxs-lookup"><span data-stu-id="70abb-116">The Store URL of the application</span></span>|
|<span data-ttu-id="70abb-117">appId</span><span class="sxs-lookup"><span data-stu-id="70abb-117">appId</span></span>|<span data-ttu-id="70abb-118">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="70abb-118">String</span></span>|<span data-ttu-id="70abb-119">アプリケーションのアプリケーションまたはバンドルの識別子</span><span class="sxs-lookup"><span data-stu-id="70abb-119">The application or bundle identifier of the application</span></span>|

## <a name="relationships"></a><span data-ttu-id="70abb-120">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="70abb-120">Relationships</span></span>
<span data-ttu-id="70abb-121">なし</span><span class="sxs-lookup"><span data-stu-id="70abb-121">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="70abb-122">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="70abb-122">JSON Representation</span></span>
<span data-ttu-id="70abb-123">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="70abb-123">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appListItem"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.appListItem",
  "name": "String",
  "publisher": "String",
  "appStoreUrl": "String",
  "appId": "String"
}
```



