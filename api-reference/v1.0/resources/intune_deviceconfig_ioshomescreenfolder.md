# <a name="ioshomescreenfolder-resource-type"></a><span data-ttu-id="e9336-101">iosHomeScreenFolder リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e9336-101">iosHomeScreenFolder resource type</span></span>

> <span data-ttu-id="e9336-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e9336-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e9336-103">ホーム画面上のアプリのページが含まれるフォルダー</span><span class="sxs-lookup"><span data-stu-id="e9336-103">A folder containing pages of apps on the Home Screen</span></span>

<span data-ttu-id="e9336-104">[iosHomeScreenItem](../resources/intune_deviceconfig_ioshomescreenitem.md) からの継承</span><span class="sxs-lookup"><span data-stu-id="e9336-104">Inherits from [iosHomeScreenItem](../resources/intune_deviceconfig_ioshomescreenitem.md)</span></span>

## <a name="properties"></a><span data-ttu-id="e9336-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e9336-105">Properties</span></span>
|<span data-ttu-id="e9336-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e9336-106">Property</span></span>|<span data-ttu-id="e9336-107">型</span><span class="sxs-lookup"><span data-stu-id="e9336-107">Type</span></span>|<span data-ttu-id="e9336-108">説明</span><span class="sxs-lookup"><span data-stu-id="e9336-108">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e9336-109">displayName</span><span class="sxs-lookup"><span data-stu-id="e9336-109">displayName</span></span>|<span data-ttu-id="e9336-110">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="e9336-110">String</span></span>|<span data-ttu-id="e9336-111">アプリの名前。[iosHomeScreenItem](../resources/intune_deviceconfig_ioshomescreenitem.md) から継承</span><span class="sxs-lookup"><span data-stu-id="e9336-111">Name of the app Inherited from [iosHomeScreenItem](../resources/intune_deviceconfig_ioshomescreenitem.md)</span></span>|
|<span data-ttu-id="e9336-112">pages</span><span class="sxs-lookup"><span data-stu-id="e9336-112">pages</span></span>|<span data-ttu-id="e9336-113">[iosHomeScreenFolderPage](../resources/intune_deviceconfig_ioshomescreenfolderpage.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e9336-113">[iosHomeScreenFolderPage](../resources/intune_deviceconfig_ioshomescreenfolderpage.md) collection</span></span>|<span data-ttu-id="e9336-114">アプリケーションの種類にする必要がある、ホーム画面レイアウト アイコンで構成されるページ。</span><span class="sxs-lookup"><span data-stu-id="e9336-114">Pages of Home Screen Layout Icons which must be Application Type.</span></span> <span data-ttu-id="e9336-115">このコレクションには、最大で 500 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="e9336-115">This collection can contain a maximum of 500 elements.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e9336-116">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e9336-116">Relationships</span></span>
<span data-ttu-id="e9336-117">なし</span><span class="sxs-lookup"><span data-stu-id="e9336-117">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e9336-118">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e9336-118">JSON Representation</span></span>
<span data-ttu-id="e9336-119">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e9336-119">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosHomeScreenFolder"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenFolder",
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
```



