# <a name="termsandconditionsacceptancestatus-resource-type"></a><span data-ttu-id="5dc89-101">termsAndConditionsAcceptanceStatus リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="5dc89-101">termsAndConditionsAcceptanceStatus resource type</span></span>

> <span data-ttu-id="5dc89-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="5dc89-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5dc89-103">termsAndConditionsAcceptanceStatus エンティティは、特定のユーザーによる特定の使用条件 (T&C) のポリシーの承諾状況を表します。</span><span class="sxs-lookup"><span data-stu-id="5dc89-103">A termsAndConditionsAcceptanceStatus entity represents the acceptance status of a given Terms and Conditions (T&C) policy by a given user.</span></span> <span data-ttu-id="5dc89-104">ポータル サイトへのアクセスを保持するには、ユーザーは最新バージョンの使用条件を承諾する必要があります。</span><span class="sxs-lookup"><span data-stu-id="5dc89-104">Users must accept the most up-to-date version of the terms in order to retain access to the Company Portal.</span></span>
## <a name="methods"></a><span data-ttu-id="5dc89-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="5dc89-105">Methods</span></span>
|<span data-ttu-id="5dc89-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="5dc89-106">Method</span></span>|<span data-ttu-id="5dc89-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="5dc89-107">Return Type</span></span>|<span data-ttu-id="5dc89-108">説明</span><span class="sxs-lookup"><span data-stu-id="5dc89-108">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5dc89-109">List termsAndConditionsAcceptanceStatuses</span><span class="sxs-lookup"><span data-stu-id="5dc89-109">List termsAndConditionsAcceptanceStatuses</span></span>](../api/intune_companyterms_termsandconditionsacceptancestatus_list.md)|<span data-ttu-id="5dc89-110">[termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="5dc89-110">[termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md) collection</span></span>|<span data-ttu-id="5dc89-111">[termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="5dc89-111">List properties and relationships of the [termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md) objects.</span></span>|
|[<span data-ttu-id="5dc89-112">Get termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="5dc89-112">Get termsAndConditionsAcceptanceStatus</span></span>](../api/intune_companyterms_termsandconditionsacceptancestatus_get.md)|[<span data-ttu-id="5dc89-113">termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="5dc89-113">termsAndConditionsAcceptanceStatus</span></span>](../resources/intune_companyterms_termsandconditionsacceptancestatus.md)|<span data-ttu-id="5dc89-114">[termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="5dc89-114">Read properties and relationships of [plannerTaskDetails](../resources/intune_companyterms_termsandconditionsacceptancestatus.md) object.</span></span>|
|[<span data-ttu-id="5dc89-115">Create termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="5dc89-115">Create termsAndConditionsAcceptanceStatus</span></span>](../api/intune_companyterms_termsandconditionsacceptancestatus_create.md)|[<span data-ttu-id="5dc89-116">termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="5dc89-116">termsAndConditionsAcceptanceStatus</span></span>](../resources/intune_companyterms_termsandconditionsacceptancestatus.md)|<span data-ttu-id="5dc89-117">新しい [termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="5dc89-117">Create a new [plannerBucket](../resources/intune_companyterms_termsandconditionsacceptancestatus.md) object.</span></span>|
|[<span data-ttu-id="5dc89-118">Delete termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="5dc89-118">Delete termsAndConditionsAcceptanceStatus</span></span>](../api/intune_companyterms_termsandconditionsacceptancestatus_delete.md)|<span data-ttu-id="5dc89-119">なし</span><span class="sxs-lookup"><span data-stu-id="5dc89-119">None</span></span>|<span data-ttu-id="5dc89-120">[termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="5dc89-120">Deletes a [termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md).</span></span>|
|[<span data-ttu-id="5dc89-121">Update termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="5dc89-121">Update termsAndConditionsAcceptanceStatus</span></span>](../api/intune_companyterms_termsandconditionsacceptancestatus_update.md)|[<span data-ttu-id="5dc89-122">termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="5dc89-122">termsAndConditionsAcceptanceStatus</span></span>](../resources/intune_companyterms_termsandconditionsacceptancestatus.md)|<span data-ttu-id="5dc89-123">[termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="5dc89-123">Update the properties of a [calendar](../resources/intune_companyterms_termsandconditionsacceptancestatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="5dc89-124">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5dc89-124">Properties</span></span>
|<span data-ttu-id="5dc89-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5dc89-125">Property</span></span>|<span data-ttu-id="5dc89-126">型</span><span class="sxs-lookup"><span data-stu-id="5dc89-126">Type</span></span>|<span data-ttu-id="5dc89-127">説明</span><span class="sxs-lookup"><span data-stu-id="5dc89-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5dc89-128">id</span><span class="sxs-lookup"><span data-stu-id="5dc89-128">id</span></span>|<span data-ttu-id="5dc89-129">String</span><span class="sxs-lookup"><span data-stu-id="5dc89-129">String</span></span>|<span data-ttu-id="5dc89-130">エンティティの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="5dc89-130">Unique identifier of the folder.</span></span>|
|<span data-ttu-id="5dc89-131">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="5dc89-131">userDisplayName</span></span>|<span data-ttu-id="5dc89-132">String</span><span class="sxs-lookup"><span data-stu-id="5dc89-132">String</span></span>|<span data-ttu-id="5dc89-133">エンティティによって承諾が示されているユーザーの表示名。</span><span class="sxs-lookup"><span data-stu-id="5dc89-133">Display name of the user whose acceptance the entity represents.</span></span>|
|<span data-ttu-id="5dc89-134">acceptedVersion</span><span class="sxs-lookup"><span data-stu-id="5dc89-134">acceptedVersion</span></span>|<span data-ttu-id="5dc89-135">Int32</span><span class="sxs-lookup"><span data-stu-id="5dc89-135">Int32</span></span>|<span data-ttu-id="5dc89-136">ユーザーによって承諾された使用条件の最新バージョン番号。</span><span class="sxs-lookup"><span data-stu-id="5dc89-136">Most recent version number of the T&C accepted by the user.</span></span>|
|<span data-ttu-id="5dc89-137">acceptedDateTime</span><span class="sxs-lookup"><span data-stu-id="5dc89-137">acceptedDateTime</span></span>|<span data-ttu-id="5dc89-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5dc89-138">DateTimeOffset</span></span>|<span data-ttu-id="5dc89-139">最後に使用条件がユーザーによって承諾された DateTime。</span><span class="sxs-lookup"><span data-stu-id="5dc89-139">DateTime when the terms were last accepted by the user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5dc89-140">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="5dc89-140">Relationships</span></span>
|<span data-ttu-id="5dc89-141">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="5dc89-141">Relationship</span></span>|<span data-ttu-id="5dc89-142">型</span><span class="sxs-lookup"><span data-stu-id="5dc89-142">Type</span></span>|<span data-ttu-id="5dc89-143">説明</span><span class="sxs-lookup"><span data-stu-id="5dc89-143">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5dc89-144">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="5dc89-144">termsAndConditions</span></span>|[<span data-ttu-id="5dc89-145">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="5dc89-145">termsAndConditions</span></span>](../resources/intune_companyterms_termsandconditions.md)|<span data-ttu-id="5dc89-146">割り当てられた使用条件へのナビゲーション リンク。</span><span class="sxs-lookup"><span data-stu-id="5dc89-146">Navigation link to the terms and conditions that are assigned.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5dc89-147">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5dc89-147">JSON Representation</span></span>
<span data-ttu-id="5dc89-148">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="5dc89-148">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termsAndConditionsAcceptanceStatus"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
  "id": "String (identifier)",
  "userDisplayName": "String",
  "acceptedVersion": 1024,
  "acceptedDateTime": "String (timestamp)"
}
```


