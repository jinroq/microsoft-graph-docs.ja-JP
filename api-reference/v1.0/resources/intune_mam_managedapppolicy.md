# <a name="managedapppolicy-resource-type"></a><span data-ttu-id="71c53-101">managedAppPolicy リソースの種類</span><span class="sxs-lookup"><span data-stu-id="71c53-101">managedAppPolicy resource type</span></span>

> <span data-ttu-id="71c53-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="71c53-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="71c53-103">ManagedAppPolicy リソースは、プラットフォーム特有のポリシーの基本型を表します。</span><span class="sxs-lookup"><span data-stu-id="71c53-103">The ManagedAppPolicy resource represents a base type for platform specific policies.</span></span>
## <a name="methods"></a><span data-ttu-id="71c53-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="71c53-104">Methods</span></span>
|<span data-ttu-id="71c53-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="71c53-105">Method</span></span>|<span data-ttu-id="71c53-106">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="71c53-106">Return Type</span></span>|<span data-ttu-id="71c53-107">説明</span><span class="sxs-lookup"><span data-stu-id="71c53-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="71c53-108">List managedAppPolicies</span><span class="sxs-lookup"><span data-stu-id="71c53-108">List managedAppPolicies</span></span>](../api/intune_mam_managedapppolicy_list.md)|<span data-ttu-id="71c53-109">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="71c53-109">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) collection</span></span>|<span data-ttu-id="71c53-110">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="71c53-110">List properties and relationships of the [managedAppPolicy](../resources/intune_mam_managedapppolicy.md) objects.</span></span>|
|[<span data-ttu-id="71c53-111">Get managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="71c53-111">Get managedAppPolicy</span></span>](../api/intune_mam_managedapppolicy_get.md)|[<span data-ttu-id="71c53-112">managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="71c53-112">managedAppPolicy</span></span>](../resources/intune_mam_managedapppolicy.md)|<span data-ttu-id="71c53-113">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="71c53-113">Read properties and relationships of the [managedAppPolicy](../resources/intune_mam_managedapppolicy.md) object.</span></span>|
|[<span data-ttu-id="71c53-114">targetApps アクション</span><span class="sxs-lookup"><span data-stu-id="71c53-114">targetApps action</span></span>](../api/intune_mam_managedapppolicy_targetapps.md)|<span data-ttu-id="71c53-115">なし</span><span class="sxs-lookup"><span data-stu-id="71c53-115">None</span></span>|<span data-ttu-id="71c53-116">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="71c53-116">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="71c53-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="71c53-117">Properties</span></span>
|<span data-ttu-id="71c53-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="71c53-118">Property</span></span>|<span data-ttu-id="71c53-119">型</span><span class="sxs-lookup"><span data-stu-id="71c53-119">Type</span></span>|<span data-ttu-id="71c53-120">説明</span><span class="sxs-lookup"><span data-stu-id="71c53-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71c53-121">displayName</span><span class="sxs-lookup"><span data-stu-id="71c53-121">displayName</span></span>|<span data-ttu-id="71c53-122">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="71c53-122">String</span></span>|<span data-ttu-id="71c53-123">ポリシーの表示名。</span><span class="sxs-lookup"><span data-stu-id="71c53-123">Policy display name.</span></span>|
|<span data-ttu-id="71c53-124">description</span><span class="sxs-lookup"><span data-stu-id="71c53-124">description</span></span>|<span data-ttu-id="71c53-125">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="71c53-125">String</span></span>|<span data-ttu-id="71c53-126">ポリシーの説明。</span><span class="sxs-lookup"><span data-stu-id="71c53-126">The policy's description.</span></span>|
|<span data-ttu-id="71c53-127">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="71c53-127">createdDateTime</span></span>|<span data-ttu-id="71c53-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="71c53-128">DateTimeOffset</span></span>|<span data-ttu-id="71c53-129">ポリシーが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="71c53-129">The date and time the policy was created.</span></span>|
|<span data-ttu-id="71c53-130">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="71c53-130">lastModifiedDateTime</span></span>|<span data-ttu-id="71c53-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="71c53-131">DateTimeOffset</span></span>|<span data-ttu-id="71c53-132">ポリシーが変更された最終日時。</span><span class="sxs-lookup"><span data-stu-id="71c53-132">Last time the policy was modified.</span></span>|
|<span data-ttu-id="71c53-133">id</span><span class="sxs-lookup"><span data-stu-id="71c53-133">id</span></span>|<span data-ttu-id="71c53-134">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="71c53-134">String</span></span>|<span data-ttu-id="71c53-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="71c53-135">Key of the entity.</span></span>|
|<span data-ttu-id="71c53-136">version</span><span class="sxs-lookup"><span data-stu-id="71c53-136">version</span></span>|<span data-ttu-id="71c53-137">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="71c53-137">String</span></span>|<span data-ttu-id="71c53-138">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="71c53-138">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="71c53-139">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="71c53-139">Relationships</span></span>
<span data-ttu-id="71c53-140">なし</span><span class="sxs-lookup"><span data-stu-id="71c53-140">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="71c53-141">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="71c53-141">JSON Representation</span></span>
<span data-ttu-id="71c53-142">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="71c53-142">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppPolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppPolicy",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "version": "String"
}
```



