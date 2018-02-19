# <a name="managedappconfiguration-resource-type"></a><span data-ttu-id="1adda-101">managedAppConfiguration リソースの種類</span><span class="sxs-lookup"><span data-stu-id="1adda-101">managedAppConfiguration resource type</span></span>

> <span data-ttu-id="1adda-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="1adda-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1adda-103">構成の対象であるユーザーに対して、一連のカスタム設定を現状のままアプリに配信するために使用する構成です。</span><span class="sxs-lookup"><span data-stu-id="1adda-103">Configuration used to deliver a set of custom settings as-is to apps for users to whom the configuration is scoped</span></span>

<span data-ttu-id="1adda-104">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1adda-104">Inherits from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>

## <a name="methods"></a><span data-ttu-id="1adda-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="1adda-105">Methods</span></span>
|<span data-ttu-id="1adda-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="1adda-106">Method</span></span>|<span data-ttu-id="1adda-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="1adda-107">Return Type</span></span>|<span data-ttu-id="1adda-108">説明</span><span class="sxs-lookup"><span data-stu-id="1adda-108">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="1adda-109">managedAppConfigurations のリスト</span><span class="sxs-lookup"><span data-stu-id="1adda-109">List managedAppConfigurations</span></span>](../api/intune_mam_managedappconfiguration_list.md)|<span data-ttu-id="1adda-110">[managedAppConfiguration](../resources/intune_mam_managedappconfiguration.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="1adda-110">[managedAppConfiguration](../resources/intune_mam_managedappconfiguration.md) collection</span></span>|<span data-ttu-id="1adda-111">[managedAppConfiguration](../resources/intune_mam_managedappconfiguration.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="1adda-111">List properties and relationships of the [managedAppConfiguration](../resources/intune_mam_managedappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="1adda-112">managedAppConfiguration の取得</span><span class="sxs-lookup"><span data-stu-id="1adda-112">Get managedAppConfiguration</span></span>](../api/intune_mam_managedappconfiguration_get.md)|[<span data-ttu-id="1adda-113">managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="1adda-113">managedAppConfiguration</span></span>](../resources/intune_mam_managedappconfiguration.md)|<span data-ttu-id="1adda-114">[managedAppConfiguration](../resources/intune_mam_managedappconfiguration.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="1adda-114">Read properties and relationships of [plannerTaskDetails](../resources/intune_mam_managedappconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="1adda-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1adda-115">Properties</span></span>
|<span data-ttu-id="1adda-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1adda-116">Property</span></span>|<span data-ttu-id="1adda-117">型</span><span class="sxs-lookup"><span data-stu-id="1adda-117">Type</span></span>|<span data-ttu-id="1adda-118">説明</span><span class="sxs-lookup"><span data-stu-id="1adda-118">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1adda-119">displayName</span><span class="sxs-lookup"><span data-stu-id="1adda-119">displayName</span></span>|<span data-ttu-id="1adda-120">String</span><span class="sxs-lookup"><span data-stu-id="1adda-120">String</span></span>|<span data-ttu-id="1adda-121">ポリシーの表示名。</span><span class="sxs-lookup"><span data-stu-id="1adda-121">Policy display name.</span></span> <span data-ttu-id="1adda-122">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1adda-122">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="1adda-123">description</span><span class="sxs-lookup"><span data-stu-id="1adda-123">description</span></span>|<span data-ttu-id="1adda-124">String</span><span class="sxs-lookup"><span data-stu-id="1adda-124">String</span></span>|<span data-ttu-id="1adda-125">ポリシーの説明。</span><span class="sxs-lookup"><span data-stu-id="1adda-125">The policy's description.</span></span> <span data-ttu-id="1adda-126">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1adda-126">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="1adda-127">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1adda-127">createdDateTime</span></span>|<span data-ttu-id="1adda-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1adda-128">DateTimeOffset</span></span>|<span data-ttu-id="1adda-129">ポリシーが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="1adda-129">The date and time when the page was created.</span></span> <span data-ttu-id="1adda-130">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1adda-130">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="1adda-131">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="1adda-131">lastModifiedDateTime</span></span>|<span data-ttu-id="1adda-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1adda-132">DateTimeOffset</span></span>|<span data-ttu-id="1adda-133">ポリシーが変更された最終日時。</span><span class="sxs-lookup"><span data-stu-id="1adda-133">Last time the policy was modified.</span></span> <span data-ttu-id="1adda-134">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1adda-134">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="1adda-135">id</span><span class="sxs-lookup"><span data-stu-id="1adda-135">id</span></span>|<span data-ttu-id="1adda-136">String</span><span class="sxs-lookup"><span data-stu-id="1adda-136">String</span></span>|<span data-ttu-id="1adda-137">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="1adda-137">Name of the entity.</span></span> <span data-ttu-id="1adda-138">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1adda-138">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="1adda-139">version</span><span class="sxs-lookup"><span data-stu-id="1adda-139">version</span></span>|<span data-ttu-id="1adda-140">String</span><span class="sxs-lookup"><span data-stu-id="1adda-140">String</span></span>|<span data-ttu-id="1adda-141">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="1adda-141">Version of the entity.</span></span> <span data-ttu-id="1adda-142">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1adda-142">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="1adda-143">customSettings</span><span class="sxs-lookup"><span data-stu-id="1adda-143">customSettings</span></span>|<span data-ttu-id="1adda-144">[keyValuePair](../resources/intune_mam_keyvaluepair.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="1adda-144">[keyValuePair](../resources/intune_mam_keyvaluepair.md) collection</span></span>|<span data-ttu-id="1adda-145">構成の対象であるユーザーに対して、このサービスで変更せずに、アプリに送信される文字列キーと文字列値の一連のペア</span><span class="sxs-lookup"><span data-stu-id="1adda-145">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service</span></span>|

## <a name="relationships"></a><span data-ttu-id="1adda-146">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="1adda-146">Relationships</span></span>
<span data-ttu-id="1adda-147">なし</span><span class="sxs-lookup"><span data-stu-id="1adda-147">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="1adda-148">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="1adda-148">JSON Representation</span></span>
<span data-ttu-id="1adda-149">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="1adda-149">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppConfiguration",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "version": "String",
  "customSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ]
}
```



