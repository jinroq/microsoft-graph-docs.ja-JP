# <a name="managedappconfiguration-resource-type"></a><span data-ttu-id="641be-101">managedAppConfiguration リソースの種類</span><span class="sxs-lookup"><span data-stu-id="641be-101">managedAppConfiguration resource type</span></span>

> <span data-ttu-id="641be-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="641be-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="641be-103">構成の対象であるユーザーに対して、一連のカスタム設定を現状のままアプリに配信するために使用する構成です。</span><span class="sxs-lookup"><span data-stu-id="641be-103">Configuration used to deliver a set of custom settings as-is to apps for users to whom the configuration is scoped</span></span>

<span data-ttu-id="641be-104">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="641be-104">Inherits from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>

## <a name="methods"></a><span data-ttu-id="641be-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="641be-105">Methods</span></span>
|<span data-ttu-id="641be-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="641be-106">Method</span></span>|<span data-ttu-id="641be-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="641be-107">Return Type</span></span>|<span data-ttu-id="641be-108">説明</span><span class="sxs-lookup"><span data-stu-id="641be-108">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="641be-109">managedAppConfigurations のリスト</span><span class="sxs-lookup"><span data-stu-id="641be-109">List managedAppConfigurations</span></span>](../api/intune_mam_managedappconfiguration_list.md)|<span data-ttu-id="641be-110">[managedAppConfiguration](../resources/intune_mam_managedappconfiguration.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="641be-110">[managedAppConfiguration](../resources/intune_mam_managedappconfiguration.md) collection</span></span>|<span data-ttu-id="641be-111">[managedAppConfiguration](../resources/intune_mam_managedappconfiguration.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="641be-111">List properties and relationships of the [managedAppConfiguration](../resources/intune_mam_managedappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="641be-112">managedAppConfiguration の取得</span><span class="sxs-lookup"><span data-stu-id="641be-112">Get managedAppConfiguration</span></span>](../api/intune_mam_managedappconfiguration_get.md)|[<span data-ttu-id="641be-113">managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="641be-113">managedAppConfiguration</span></span>](../resources/intune_mam_managedappconfiguration.md)|<span data-ttu-id="641be-114">[managedAppConfiguration](../resources/intune_mam_managedappconfiguration.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="641be-114">Read properties and relationships of the [managedAppConfiguration](../resources/intune_mam_managedappconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="641be-115">プロパティ</span><span class="sxs-lookup"><span data-stu-id="641be-115">Properties</span></span>
|<span data-ttu-id="641be-116">プロパティ</span><span class="sxs-lookup"><span data-stu-id="641be-116">Property</span></span>|<span data-ttu-id="641be-117">タイプ</span><span class="sxs-lookup"><span data-stu-id="641be-117">Type</span></span>|<span data-ttu-id="641be-118">説明</span><span class="sxs-lookup"><span data-stu-id="641be-118">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="641be-119">displayName</span><span class="sxs-lookup"><span data-stu-id="641be-119">displayName</span></span>|<span data-ttu-id="641be-120">文字列</span><span class="sxs-lookup"><span data-stu-id="641be-120">String</span></span>|<span data-ttu-id="641be-121">ポリシーの表示名。</span><span class="sxs-lookup"><span data-stu-id="641be-121">Policy display name.</span></span> <span data-ttu-id="641be-122">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="641be-122">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="641be-123">説明</span><span class="sxs-lookup"><span data-stu-id="641be-123">description</span></span>|<span data-ttu-id="641be-124">文字列</span><span class="sxs-lookup"><span data-stu-id="641be-124">String</span></span>|<span data-ttu-id="641be-125">ポリシーの説明。</span><span class="sxs-lookup"><span data-stu-id="641be-125">The policy's description.</span></span> <span data-ttu-id="641be-126">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="641be-126">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="641be-127">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="641be-127">createdDateTime</span></span>|<span data-ttu-id="641be-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="641be-128">DateTimeOffset</span></span>|<span data-ttu-id="641be-129">ポリシーが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="641be-129">The date and time the policy was created.</span></span> <span data-ttu-id="641be-130">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="641be-130">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="641be-131">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="641be-131">lastModifiedDateTime</span></span>|<span data-ttu-id="641be-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="641be-132">DateTimeOffset</span></span>|<span data-ttu-id="641be-133">ポリシーが変更された最終日時。</span><span class="sxs-lookup"><span data-stu-id="641be-133">Last time the policy was modified.</span></span> <span data-ttu-id="641be-134">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="641be-134">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="641be-135">ID</span><span class="sxs-lookup"><span data-stu-id="641be-135">id</span></span>|<span data-ttu-id="641be-136">文字列</span><span class="sxs-lookup"><span data-stu-id="641be-136">String</span></span>|<span data-ttu-id="641be-137">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="641be-137">Key of the entity.</span></span> <span data-ttu-id="641be-138">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="641be-138">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="641be-139">バージョン</span><span class="sxs-lookup"><span data-stu-id="641be-139">version</span></span>|<span data-ttu-id="641be-140">文字列</span><span class="sxs-lookup"><span data-stu-id="641be-140">String</span></span>|<span data-ttu-id="641be-141">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="641be-141">Version of the entity.</span></span> <span data-ttu-id="641be-142">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="641be-142">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="641be-143">customSettings</span><span class="sxs-lookup"><span data-stu-id="641be-143">customSettings</span></span>|<span data-ttu-id="641be-144">[keyValuePair](../resources/intune_mam_keyvaluepair.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="641be-144">[keyValuePair](../resources/intune_mam_keyvaluepair.md) collection</span></span>|<span data-ttu-id="641be-145">構成の対象であるユーザーに対して、このサービスで変更せずに、アプリに送信される文字列キーと文字列値の一連のペア</span><span class="sxs-lookup"><span data-stu-id="641be-145">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service</span></span>|

## <a name="relationships"></a><span data-ttu-id="641be-146">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="641be-146">Relationships</span></span>
<span data-ttu-id="641be-147">なし</span><span class="sxs-lookup"><span data-stu-id="641be-147">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="641be-148">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="641be-148">JSON Representation</span></span>
<span data-ttu-id="641be-149">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="641be-149">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "abstract": true,
  "keyProperty": "id",
  "baseType": "microsoft.graph.managedAppPolicy",
  "@odata.type": "microsoft.graph.managedAppConfiguration"
}-->
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



