# <a name="ioshomescreenitem-resource-type"></a><span data-ttu-id="4e12f-101">iosHomeScreenItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4e12f-101">iosHomeScreenItem resource type</span></span>

> <span data-ttu-id="4e12f-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="4e12f-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4e12f-103">IOS ホーム画面上のアイテムを表します</span><span class="sxs-lookup"><span data-stu-id="4e12f-103">Represents an item on the iOS Home Screen</span></span>
## <a name="properties"></a><span data-ttu-id="4e12f-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4e12f-104">Properties</span></span>
|<span data-ttu-id="4e12f-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4e12f-105">Property</span></span>|<span data-ttu-id="4e12f-106">型</span><span class="sxs-lookup"><span data-stu-id="4e12f-106">Type</span></span>|<span data-ttu-id="4e12f-107">説明</span><span class="sxs-lookup"><span data-stu-id="4e12f-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4e12f-108">displayName</span><span class="sxs-lookup"><span data-stu-id="4e12f-108">displayName</span></span>|<span data-ttu-id="4e12f-109">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="4e12f-109">String</span></span>|<span data-ttu-id="4e12f-110">アプリの名前</span><span class="sxs-lookup"><span data-stu-id="4e12f-110">Name of the app</span></span>|

## <a name="relationships"></a><span data-ttu-id="4e12f-111">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4e12f-111">Relationships</span></span>
<span data-ttu-id="4e12f-112">なし</span><span class="sxs-lookup"><span data-stu-id="4e12f-112">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4e12f-113">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4e12f-113">JSON Representation</span></span>
<span data-ttu-id="4e12f-114">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="4e12f-114">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.iosHomeScreenItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.iosHomeScreenItem",
  "displayName": "String"
}
```



