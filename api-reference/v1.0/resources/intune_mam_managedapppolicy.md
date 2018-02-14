# <a name="managedapppolicy-resource-type"></a><span data-ttu-id="014e5-101">managedAppPolicy リソースの種類</span><span class="sxs-lookup"><span data-stu-id="014e5-101">managedAppPolicy resource type</span></span>

> <span data-ttu-id="014e5-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="014e5-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="014e5-103">ManagedAppPolicy リソースは、プラットフォーム特有のポリシーの基本型を表します。</span><span class="sxs-lookup"><span data-stu-id="014e5-103">The ManagedAppPolicy resource represents a base type for platform specific policies.</span></span>
## <a name="methods"></a><span data-ttu-id="014e5-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="014e5-104">Methods</span></span>
|<span data-ttu-id="014e5-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="014e5-105">Method</span></span>|<span data-ttu-id="014e5-106">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="014e5-106">Return Type</span></span>|<span data-ttu-id="014e5-107">説明</span><span class="sxs-lookup"><span data-stu-id="014e5-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="014e5-108">List managedAppPolicies</span><span class="sxs-lookup"><span data-stu-id="014e5-108">List managedAppPolicies</span></span>](../api/intune_mam_managedapppolicy_list.md)|<span data-ttu-id="014e5-109">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="014e5-109">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) collection</span></span>|<span data-ttu-id="014e5-110">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="014e5-110">List properties and relationships of the [managedAppPolicy](../resources/intune_mam_managedapppolicy.md) objects.</span></span>|
|[<span data-ttu-id="014e5-111">Get managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="014e5-111">Get managedAppPolicy</span></span>](../api/intune_mam_managedapppolicy_get.md)|[<span data-ttu-id="014e5-112">managedAppPolicy</span><span class="sxs-lookup"><span data-stu-id="014e5-112">managedAppPolicy</span></span>](../resources/intune_mam_managedapppolicy.md)|<span data-ttu-id="014e5-113">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="014e5-113">Read properties and relationships of [plannerTaskDetails](../resources/intune_mam_managedapppolicy.md) object.</span></span>|
|[<span data-ttu-id="014e5-114">targetApps アクション</span><span class="sxs-lookup"><span data-stu-id="014e5-114">targetApps action</span></span>](../api/intune_mam_managedapppolicy_targetapps.md)|<span data-ttu-id="014e5-115">なし</span><span class="sxs-lookup"><span data-stu-id="014e5-115">None</span></span>|<span data-ttu-id="014e5-116">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="014e5-116">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="014e5-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="014e5-117">Properties</span></span>
|<span data-ttu-id="014e5-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="014e5-118">Property</span></span>|<span data-ttu-id="014e5-119">型</span><span class="sxs-lookup"><span data-stu-id="014e5-119">Type</span></span>|<span data-ttu-id="014e5-120">説明</span><span class="sxs-lookup"><span data-stu-id="014e5-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="014e5-121">displayName</span><span class="sxs-lookup"><span data-stu-id="014e5-121">displayName</span></span>|<span data-ttu-id="014e5-122">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="014e5-122">String</span></span>|<span data-ttu-id="014e5-123">ポリシーの表示名。</span><span class="sxs-lookup"><span data-stu-id="014e5-123">Policy display name.</span></span>|
|<span data-ttu-id="014e5-124">description</span><span class="sxs-lookup"><span data-stu-id="014e5-124">description</span></span>|<span data-ttu-id="014e5-125">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="014e5-125">String</span></span>|<span data-ttu-id="014e5-126">ポリシーの説明。</span><span class="sxs-lookup"><span data-stu-id="014e5-126">The policy's description.</span></span>|
|<span data-ttu-id="014e5-127">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="014e5-127">createdDateTime</span></span>|<span data-ttu-id="014e5-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="014e5-128">DateTimeOffset</span></span>|<span data-ttu-id="014e5-129">ポリシーが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="014e5-129">The date and time when the page was created.</span></span>|
|<span data-ttu-id="014e5-130">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="014e5-130">lastModifiedDateTime</span></span>|<span data-ttu-id="014e5-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="014e5-131">DateTimeOffset</span></span>|<span data-ttu-id="014e5-132">ポリシーが変更された最終日時。</span><span class="sxs-lookup"><span data-stu-id="014e5-132">Last time the policy was modified.</span></span>|
|<span data-ttu-id="014e5-133">id</span><span class="sxs-lookup"><span data-stu-id="014e5-133">id</span></span>|<span data-ttu-id="014e5-134">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="014e5-134">String</span></span>|<span data-ttu-id="014e5-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="014e5-135">Name of the entity.</span></span>|
|<span data-ttu-id="014e5-136">version</span><span class="sxs-lookup"><span data-stu-id="014e5-136">version</span></span>|<span data-ttu-id="014e5-137">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="014e5-137">String</span></span>|<span data-ttu-id="014e5-138">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="014e5-138">Version of the entity.</span></span>|

## <a name="relationships"></a><span data-ttu-id="014e5-139">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="014e5-139">Relationships</span></span>
<span data-ttu-id="014e5-140">なし</span><span class="sxs-lookup"><span data-stu-id="014e5-140">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="014e5-141">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="014e5-141">JSON Representation</span></span>
<span data-ttu-id="014e5-142">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="014e5-142">Here is a JSON representation of the resource.</span></span>
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



