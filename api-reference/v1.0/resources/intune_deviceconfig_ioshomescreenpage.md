# <a name="ioshomescreenpage-resource-type"></a><span data-ttu-id="2a61a-101">iosHomeScreenPage リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2a61a-101">iosHomeScreenPage resource type</span></span>

> <span data-ttu-id="2a61a-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="2a61a-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2a61a-103">ホーム画面上のアプリとフォルダーが含まれるページ</span><span class="sxs-lookup"><span data-stu-id="2a61a-103">A page containing apps and folders on the Home Screen</span></span>
## <a name="properties"></a><span data-ttu-id="2a61a-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2a61a-104">Properties</span></span>
|<span data-ttu-id="2a61a-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2a61a-105">Property</span></span>|<span data-ttu-id="2a61a-106">型</span><span class="sxs-lookup"><span data-stu-id="2a61a-106">Type</span></span>|<span data-ttu-id="2a61a-107">説明</span><span class="sxs-lookup"><span data-stu-id="2a61a-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2a61a-108">displayName</span><span class="sxs-lookup"><span data-stu-id="2a61a-108">displayName</span></span>|<span data-ttu-id="2a61a-109">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="2a61a-109">String</span></span>|<span data-ttu-id="2a61a-110">ページの名前</span><span class="sxs-lookup"><span data-stu-id="2a61a-110">Name of the page</span></span>|
|<span data-ttu-id="2a61a-111">アイコン</span><span class="sxs-lookup"><span data-stu-id="2a61a-111">Icons</span></span>|<span data-ttu-id="2a61a-112">[iosHomeScreenItem](../resources/intune_deviceconfig_ioshomescreenitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="2a61a-112">[iosHomeScreenItem](../resources/intune_deviceconfig_ioshomescreenitem.md) collection</span></span>|<span data-ttu-id="2a61a-113">特定ページに表示されるアプリとフォルダーの一覧。</span><span class="sxs-lookup"><span data-stu-id="2a61a-113">A list of apps and folders to appear on a page.</span></span> <span data-ttu-id="2a61a-114">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="2a61a-114">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="2a61a-115">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2a61a-115">Relationships</span></span>
<span data-ttu-id="2a61a-116">なし</span><span class="sxs-lookup"><span data-stu-id="2a61a-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="2a61a-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2a61a-117">JSON Representation</span></span>
<span data-ttu-id="2a61a-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2a61a-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosHomeScreenPage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenPage",
  "displayName": "String",
  "icons": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenFolder",
      "displayName": "String",
      "pages": [
        {
          "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
          "displayName": "String",
          "apps": [
            {
              "@odata.type": "microsoft.graph.iosHomeScreenApp",
              "displayName": "String",
              "bundleID": "String"
            }
          ]
        }
      ]
    }
  ]
}
```



