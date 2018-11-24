# <a name="edgesearchengine-resource-type"></a><span data-ttu-id="c8fa6-101">edgeSearchEngine リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c8fa6-101">edgeSearchEngine resource type</span></span>

> <span data-ttu-id="c8fa6-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c8fa6-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c8fa6-103">IT 管理者が MDM 制御デバイス用向けに事前定義されている既定の検索エンジンを設定できるようにします。</span><span class="sxs-lookup"><span data-stu-id="c8fa6-103">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span>

<span data-ttu-id="c8fa6-104">[edgeSearchEngineBase](../resources/intune_deviceconfig_edgesearchenginebase.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="c8fa6-104">Inherits from [edgeSearchEngineBase](../resources/intune_deviceconfig_edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="c8fa6-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c8fa6-105">Properties</span></span>
|<span data-ttu-id="c8fa6-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c8fa6-106">Property</span></span>|<span data-ttu-id="c8fa6-107">型</span><span class="sxs-lookup"><span data-stu-id="c8fa6-107">Type</span></span>|<span data-ttu-id="c8fa6-108">説明</span><span class="sxs-lookup"><span data-stu-id="c8fa6-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c8fa6-109">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="c8fa6-109">edgeSearchEngineType</span></span>|[<span data-ttu-id="c8fa6-110">edgeSearchEngineType</span><span class="sxs-lookup"><span data-stu-id="c8fa6-110">edgeSearchEngineType</span></span>](../resources/intune_deviceconfig_edgesearchenginetype.md)|<span data-ttu-id="c8fa6-111">IT 管理者が MDM 制御デバイス用向けに事前定義されている既定の検索エンジンを設定できるようにします。</span><span class="sxs-lookup"><span data-stu-id="c8fa6-111">Allows IT admins to set a predefined default search engine for MDM-Controlled devices.</span></span> <span data-ttu-id="c8fa6-112">可能な値: `default`、`bing`。</span><span class="sxs-lookup"><span data-stu-id="c8fa6-112">Possible values are: `default`, `bing`.</span></span>|

## <a name="relationships"></a><span data-ttu-id="c8fa6-113">関係</span><span class="sxs-lookup"><span data-stu-id="c8fa6-113">Relationships</span></span>
<span data-ttu-id="c8fa6-114">なし</span><span class="sxs-lookup"><span data-stu-id="c8fa6-114">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="c8fa6-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c8fa6-115">JSON Representation</span></span>
<span data-ttu-id="c8fa6-116">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="c8fa6-116">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.edgeSearchEngine"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.edgeSearchEngine",
  "edgeSearchEngineType": "String"
}
```



