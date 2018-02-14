# <a name="edgesearchenginecustom-resource-type"></a><span data-ttu-id="9cdc9-101">edgeSearchEngineCustom リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9cdc9-101">edgeSearchEngineCustom resource type</span></span>

> <span data-ttu-id="9cdc9-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="9cdc9-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9cdc9-103">IT 管理者が MDM 制御デバイス用向けのカスタムの既定の検索エンジンを設定できるようにします。</span><span class="sxs-lookup"><span data-stu-id="9cdc9-103">Allows IT admins to set a custom default search engine for MDM-Controlled devices.</span></span>

<span data-ttu-id="9cdc9-104">[edgeSearchEngineBase](../resources/intune_deviceconfig_edgesearchenginebase.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="9cdc9-104">Inherits from [edgeSearchEngineBase](../resources/intune_deviceconfig_edgesearchenginebase.md)</span></span>

## <a name="properties"></a><span data-ttu-id="9cdc9-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9cdc9-105">Properties</span></span>
|<span data-ttu-id="9cdc9-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9cdc9-106">Property</span></span>|<span data-ttu-id="9cdc9-107">型</span><span class="sxs-lookup"><span data-stu-id="9cdc9-107">Type</span></span>|<span data-ttu-id="9cdc9-108">説明</span><span class="sxs-lookup"><span data-stu-id="9cdc9-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9cdc9-109">edgeSearchEngineOpenSearchXmlUrl</span><span class="sxs-lookup"><span data-stu-id="9cdc9-109">edgeSearchEngineOpenSearchXmlUrl</span></span>|<span data-ttu-id="9cdc9-110">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="9cdc9-110">String</span></span>|<span data-ttu-id="9cdc9-111">短縮名と検索エンジンの URL が最低限含まれる OpenSearch xml ファイルが入っている https リンクを指します。</span><span class="sxs-lookup"><span data-stu-id="9cdc9-111">Points to a https link containing the OpenSearch xml file that contains, at minimum, the short name and the URL to the search Engine.</span></span>|

## <a name="relationships"></a><span data-ttu-id="9cdc9-112">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="9cdc9-112">Relationships</span></span>
<span data-ttu-id="9cdc9-113">なし</span><span class="sxs-lookup"><span data-stu-id="9cdc9-113">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="9cdc9-114">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9cdc9-114">JSON Representation</span></span>
<span data-ttu-id="9cdc9-115">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="9cdc9-115">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.edgeSearchEngineCustom"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.edgeSearchEngineCustom",
  "edgeSearchEngineOpenSearchXmlUrl": "String"
}
```



