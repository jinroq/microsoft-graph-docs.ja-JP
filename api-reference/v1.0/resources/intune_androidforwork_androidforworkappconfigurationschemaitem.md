# <a name="androidforworkappconfigurationschemaitem-resource-type"></a><span data-ttu-id="3c332-101">androidForWorkAppConfigurationSchemaItem リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="3c332-101">androidForWorkAppConfigurationSchemaItem resource type</span></span>

> <span data-ttu-id="3c332-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="3c332-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3c332-103">Android for Work アプリケーションのカスタム構成スキーマ内の単一の構成アイテムです。</span><span class="sxs-lookup"><span data-stu-id="3c332-103">Single configuration item inside an Android for Work application's custom configuration schema.</span></span>
## <a name="properties"></a><span data-ttu-id="3c332-104">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3c332-104">Properties</span></span>
|<span data-ttu-id="3c332-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3c332-105">Property</span></span>|<span data-ttu-id="3c332-106">型</span><span class="sxs-lookup"><span data-stu-id="3c332-106">Type</span></span>|<span data-ttu-id="3c332-107">説明</span><span class="sxs-lookup"><span data-stu-id="3c332-107">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c332-108">schemaItemKey</span><span class="sxs-lookup"><span data-stu-id="3c332-108">schemaItemKey</span></span>|<span data-ttu-id="3c332-109">String</span><span class="sxs-lookup"><span data-stu-id="3c332-109">String</span></span>|<span data-ttu-id="3c332-110">アイテムを識別するためにアプリケーションが使用する一意のキー</span><span class="sxs-lookup"><span data-stu-id="3c332-110">Unique key the application uses to identify the item</span></span>|
|<span data-ttu-id="3c332-111">displayName</span><span class="sxs-lookup"><span data-stu-id="3c332-111">displayName</span></span>|<span data-ttu-id="3c332-112">String</span><span class="sxs-lookup"><span data-stu-id="3c332-112">String</span></span>|<span data-ttu-id="3c332-113">人間が判読できる名前</span><span class="sxs-lookup"><span data-stu-id="3c332-113">Human readable name of the student</span></span>|
|<span data-ttu-id="3c332-114">description</span><span class="sxs-lookup"><span data-stu-id="3c332-114">description</span></span>|<span data-ttu-id="3c332-115">String</span><span class="sxs-lookup"><span data-stu-id="3c332-115">String</span></span>|<span data-ttu-id="3c332-116">アプリケーション内でアイテムが制御する内容の説明</span><span class="sxs-lookup"><span data-stu-id="3c332-116">Description of what the item controls within the application</span></span>|
|<span data-ttu-id="3c332-117">defaultBoolValue</span><span class="sxs-lookup"><span data-stu-id="3c332-117">defaultBoolValue</span></span>|<span data-ttu-id="3c332-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="3c332-118">Boolean</span></span>|<span data-ttu-id="3c332-119">アプリの開発者が指定している場合、ブール型のアイテムの既定値</span><span class="sxs-lookup"><span data-stu-id="3c332-119">Default value for boolean type items, if specified by the app developer</span></span>|
|<span data-ttu-id="3c332-120">defaultIntValue</span><span class="sxs-lookup"><span data-stu-id="3c332-120">defaultIntValue</span></span>|<span data-ttu-id="3c332-121">Int32</span><span class="sxs-lookup"><span data-stu-id="3c332-121">Int32</span></span>|<span data-ttu-id="3c332-122">アプリの開発者が指定している場合、整数型のアイテムの既定値</span><span class="sxs-lookup"><span data-stu-id="3c332-122">Default value for integer type items, if specified by the app developer</span></span>|
|<span data-ttu-id="3c332-123">defaultStringValue</span><span class="sxs-lookup"><span data-stu-id="3c332-123">defaultStringValue</span></span>|<span data-ttu-id="3c332-124">String</span><span class="sxs-lookup"><span data-stu-id="3c332-124">String</span></span>|<span data-ttu-id="3c332-125">アプリの開発者が指定している場合、文字列型のアイテムの既定値</span><span class="sxs-lookup"><span data-stu-id="3c332-125">Default value for string type items, if specified by the app developer</span></span>|
|<span data-ttu-id="3c332-126">defaultStringArrayValue</span><span class="sxs-lookup"><span data-stu-id="3c332-126">defaultStringArrayValue</span></span>|<span data-ttu-id="3c332-127">String コレクション</span><span class="sxs-lookup"><span data-stu-id="3c332-127">String collection</span></span>|<span data-ttu-id="3c332-128">アプリの開発者が指定している場合、配列型のアイテムの既定値</span><span class="sxs-lookup"><span data-stu-id="3c332-128">Default value for string array type items, if specified by the app developer</span></span>|
|<span data-ttu-id="3c332-129">dataType</span><span class="sxs-lookup"><span data-stu-id="3c332-129">DataType</span></span>|<span data-ttu-id="3c332-130">String</span><span class="sxs-lookup"><span data-stu-id="3c332-130">String</span></span>|<span data-ttu-id="3c332-131">このアイテムが示す値の種類。可能な値は、`bool`、`integer`、`string`、`choice`、`multiselect`、`bundle`、`bundleArray`、`hidden` です。</span><span class="sxs-lookup"><span data-stu-id="3c332-131">The type of value this item describes Possible values are: `bool`, `integer`, `string`, `choice`, `multiselect`, `bundle`, `bundleArray`, `hidden`.</span></span>|
|<span data-ttu-id="3c332-132">selections</span><span class="sxs-lookup"><span data-stu-id="3c332-132">selections</span></span>|<span data-ttu-id="3c332-133">[keyValuePair](../resources/intune_androidforwork_keyvaluepair.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="3c332-133">[keyValuePair](../resources/intune_androidforwork_keyvaluepair.md) collection</span></span>|<span data-ttu-id="3c332-134">このアイテムに設定可能な有効な値に対しての、人間が判読できる名前と値の組のリスト (選択肢と複数選択項目のみ)</span><span class="sxs-lookup"><span data-stu-id="3c332-134">List of human readable name/value pairs for the valid values that can be set for this item (Choice and Multiselect items only)</span></span>|

## <a name="relationships"></a><span data-ttu-id="3c332-135">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="3c332-135">Relationships</span></span>
<span data-ttu-id="3c332-136">なし</span><span class="sxs-lookup"><span data-stu-id="3c332-136">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="3c332-137">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3c332-137">JSON Representation</span></span>
<span data-ttu-id="3c332-138">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="3c332-138">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.androidForWorkAppConfigurationSchemaItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.androidForWorkAppConfigurationSchemaItem",
  "schemaItemKey": "String",
  "displayName": "String",
  "description": "String",
  "defaultBoolValue": true,
  "defaultIntValue": 1024,
  "defaultStringValue": "String",
  "defaultStringArrayValue": [
    "String"
  ],
  "dataType": "String",
  "selections": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ]
}
```



