# <a name="ioshomescreenfolderpage-resource-type"></a><span data-ttu-id="51ac1-101">iosHomeScreenFolderPage リソースの種類</span><span class="sxs-lookup"><span data-stu-id="51ac1-101">iosHomeScreenFolderPage resource type</span></span>

> <span data-ttu-id="51ac1-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="51ac1-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="51ac1-103">ホーム画面上のアプリが含まれるフォルダー</span><span class="sxs-lookup"><span data-stu-id="51ac1-103">A folder containing apps on the Home Screen</span></span>
## <a name="properties"></a><span data-ttu-id="51ac1-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="51ac1-104">Properties</span></span>
|<span data-ttu-id="51ac1-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="51ac1-105">Property</span></span>|<span data-ttu-id="51ac1-106">型</span><span class="sxs-lookup"><span data-stu-id="51ac1-106">Type</span></span>|<span data-ttu-id="51ac1-107">説明</span><span class="sxs-lookup"><span data-stu-id="51ac1-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51ac1-108">displayName</span><span class="sxs-lookup"><span data-stu-id="51ac1-108">displayName</span></span>|<span data-ttu-id="51ac1-109">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="51ac1-109">String</span></span>|<span data-ttu-id="51ac1-110">フォルダー ページの名前</span><span class="sxs-lookup"><span data-stu-id="51ac1-110">Name of the page</span></span>|
|<span data-ttu-id="51ac1-111">apps</span><span class="sxs-lookup"><span data-stu-id="51ac1-111">apps</span></span>|<span data-ttu-id="51ac1-112">[iosHomeScreenApp](../resources/intune_deviceconfig_ioshomescreenapp.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="51ac1-112">[iosHomeScreenApp](../resources/intune_deviceconfig_ioshomescreenapp.md) collection</span></span>|<span data-ttu-id="51ac1-113">フォルダー内のページに表示されるアプリの一覧。</span><span class="sxs-lookup"><span data-stu-id="51ac1-113">A list of apps to appear on a page within a folder.</span></span> <span data-ttu-id="51ac1-114">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="51ac1-114">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="51ac1-115">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="51ac1-115">Relationships</span></span>
<span data-ttu-id="51ac1-116">なし</span><span class="sxs-lookup"><span data-stu-id="51ac1-116">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="51ac1-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="51ac1-117">JSON Representation</span></span>
<span data-ttu-id="51ac1-118">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="51ac1-118">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosHomeScreenFolderPage"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenFolderPage",
  "displayName": "String",
  "apps": [
    {
      "@odata.type": "microsoft.graph.iosHomeScreenApp",
      "displayName": "String",
      "bundleID": "String"
    }
  ]
}
```



