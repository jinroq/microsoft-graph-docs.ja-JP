# <a name="appconfigurationsettingitem-resource-type"></a><span data-ttu-id="5b205-101">appConfigurationSettingItem リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5b205-101">appConfigurationSettingItem resource type</span></span>

> <span data-ttu-id="5b205-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="5b205-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5b205-103">アプリの構成設定アイテムのプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="5b205-103">Contains properties for App configuration setting item.</span></span>
## <a name="properties"></a><span data-ttu-id="5b205-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5b205-104">Properties</span></span>
|<span data-ttu-id="5b205-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5b205-105">Property</span></span>|<span data-ttu-id="5b205-106">タイプ</span><span class="sxs-lookup"><span data-stu-id="5b205-106">Type</span></span>|<span data-ttu-id="5b205-107">説明</span><span class="sxs-lookup"><span data-stu-id="5b205-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5b205-108">appConfigKey</span><span class="sxs-lookup"><span data-stu-id="5b205-108">appConfigKey</span></span>|<span data-ttu-id="5b205-109">String</span><span class="sxs-lookup"><span data-stu-id="5b205-109">String</span></span>|<span data-ttu-id="5b205-110">アプリの構成キー。</span><span class="sxs-lookup"><span data-stu-id="5b205-110">app configuration key.</span></span>|
|<span data-ttu-id="5b205-111">appConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="5b205-111">appConfigKeyType</span></span>|<span data-ttu-id="5b205-112">mdmAppConfigKeyType</span><span class="sxs-lookup"><span data-stu-id="5b205-112">mdmAppConfigKeyType</span></span>|<span data-ttu-id="5b205-113">アプリの構成キーの種類。</span><span class="sxs-lookup"><span data-stu-id="5b205-113">app configuration key type.</span></span> <span data-ttu-id="5b205-114">可能な値は、`stringType`、`integerType`、`realType`、`booleanType`、`tokenType` です。</span><span class="sxs-lookup"><span data-stu-id="5b205-114">The possible values are `stringType`, `integerType`, `realType`, `booleanType`, `tokenType`, , , , , , , or .</span></span>|
|<span data-ttu-id="5b205-115">appConfigKeyValue</span><span class="sxs-lookup"><span data-stu-id="5b205-115">appConfigKeyValue</span></span>|<span data-ttu-id="5b205-116">String</span><span class="sxs-lookup"><span data-stu-id="5b205-116">String</span></span>|<span data-ttu-id="5b205-117">アプリの構成キーの値。</span><span class="sxs-lookup"><span data-stu-id="5b205-117">app configuration key value.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5b205-118">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="5b205-118">Relationships</span></span>
<span data-ttu-id="5b205-119">なし</span><span class="sxs-lookup"><span data-stu-id="5b205-119">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5b205-120">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5b205-120">JSON Representation</span></span>
<span data-ttu-id="5b205-121">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="5b205-121">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.appConfigurationSettingItem"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.appConfigurationSettingItem",
  "appConfigKey": "String",
  "appConfigKeyType": "String",
  "appConfigKeyValue": "String"
}
```



