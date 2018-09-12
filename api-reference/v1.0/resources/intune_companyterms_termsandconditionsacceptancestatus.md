# <a name="termsandconditionsacceptancestatus-resource-type"></a><span data-ttu-id="5966d-101">termsAndConditionsAcceptanceStatus リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="5966d-101">termsAndConditionsAcceptanceStatus resource type</span></span>

> <span data-ttu-id="5966d-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="5966d-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5966d-103">termsAndConditionsAcceptanceStatus エンティティは、特定のユーザーによる特定の使用条件 (T&C) のポリシーの承諾状況を表します。</span><span class="sxs-lookup"><span data-stu-id="5966d-103">A termsAndConditionsAcceptanceStatus entity represents the acceptance status of a given Terms and Conditions (T&C) policy by a given user.</span></span> <span data-ttu-id="5966d-104">ポータル サイトへのアクセスを保持するには、ユーザーは最新バージョンの使用条件を承諾する必要があります。</span><span class="sxs-lookup"><span data-stu-id="5966d-104">Users must accept the most up-to-date version of the terms in order to retain access to the Company Portal.</span></span>
## <a name="methods"></a><span data-ttu-id="5966d-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="5966d-105">Methods</span></span>
|<span data-ttu-id="5966d-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="5966d-106">Method</span></span>|<span data-ttu-id="5966d-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="5966d-107">Return Type</span></span>|<span data-ttu-id="5966d-108">説明</span><span class="sxs-lookup"><span data-stu-id="5966d-108">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5966d-109">termsAndConditionsAcceptanceStatuses のリスト</span><span class="sxs-lookup"><span data-stu-id="5966d-109">List termsAndConditionsAcceptanceStatuses</span></span>](../api/intune_companyterms_termsandconditionsacceptancestatus_list.md)|<span data-ttu-id="5966d-110">[termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="5966d-110">[termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md) collection</span></span>|<span data-ttu-id="5966d-111">[termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="5966d-111">List properties and relationships of the [termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md) objects.</span></span>|
|[<span data-ttu-id="5966d-112">termsAndConditionsAcceptanceStatus を取得する</span><span class="sxs-lookup"><span data-stu-id="5966d-112">Get termsAndConditionsAcceptanceStatus</span></span>](../api/intune_companyterms_termsandconditionsacceptancestatus_get.md)|[<span data-ttu-id="5966d-113">termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="5966d-113">termsAndConditionsAcceptanceStatus</span></span>](../resources/intune_companyterms_termsandconditionsacceptancestatus.md)|<span data-ttu-id="5966d-114">[termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="5966d-114">Read properties and relationships of the [termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md) object.</span></span>|
|[<span data-ttu-id="5966d-115">termsAndConditionsAcceptanceStatus を作成する</span><span class="sxs-lookup"><span data-stu-id="5966d-115">Create termsAndConditionsAcceptanceStatus</span></span>](../api/intune_companyterms_termsandconditionsacceptancestatus_create.md)|[<span data-ttu-id="5966d-116">termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="5966d-116">termsAndConditionsAcceptanceStatus</span></span>](../resources/intune_companyterms_termsandconditionsacceptancestatus.md)|<span data-ttu-id="5966d-117">新しい [termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="5966d-117">Create a new [termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md) object.</span></span>|
|[<span data-ttu-id="5966d-118">termsAndConditionsAcceptanceStatus を削除する</span><span class="sxs-lookup"><span data-stu-id="5966d-118">Delete termsAndConditionsAcceptanceStatus</span></span>](../api/intune_companyterms_termsandconditionsacceptancestatus_delete.md)|<span data-ttu-id="5966d-119">なし</span><span class="sxs-lookup"><span data-stu-id="5966d-119">None</span></span>|<span data-ttu-id="5966d-120">[termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="5966d-120">Deletes a [termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md).</span></span>|
|[<span data-ttu-id="5966d-121">termsAndConditionsAcceptanceStatus を更新する</span><span class="sxs-lookup"><span data-stu-id="5966d-121">Update termsAndConditionsAcceptanceStatus</span></span>](../api/intune_companyterms_termsandconditionsacceptancestatus_update.md)|[<span data-ttu-id="5966d-122">termsAndConditionsAcceptanceStatus</span><span class="sxs-lookup"><span data-stu-id="5966d-122">termsAndConditionsAcceptanceStatus</span></span>](../resources/intune_companyterms_termsandconditionsacceptancestatus.md)|<span data-ttu-id="5966d-123">[termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="5966d-123">Update the properties of a [termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="5966d-124">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5966d-124">Properties</span></span>
|<span data-ttu-id="5966d-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5966d-125">Property</span></span>|<span data-ttu-id="5966d-126">タイプ</span><span class="sxs-lookup"><span data-stu-id="5966d-126">Type</span></span>|<span data-ttu-id="5966d-127">説明</span><span class="sxs-lookup"><span data-stu-id="5966d-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5966d-128">ID</span><span class="sxs-lookup"><span data-stu-id="5966d-128">id</span></span>|<span data-ttu-id="5966d-129">文字列</span><span class="sxs-lookup"><span data-stu-id="5966d-129">String</span></span>|<span data-ttu-id="5966d-130">エンティティの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="5966d-130">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="5966d-131">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="5966d-131">userDisplayName</span></span>|<span data-ttu-id="5966d-132">文字列</span><span class="sxs-lookup"><span data-stu-id="5966d-132">String</span></span>|<span data-ttu-id="5966d-133">エンティティによって承諾が示されているユーザーの表示名。</span><span class="sxs-lookup"><span data-stu-id="5966d-133">Display name of the user whose acceptance the entity represents.</span></span>|
|<span data-ttu-id="5966d-134">acceptedVersion</span><span class="sxs-lookup"><span data-stu-id="5966d-134">acceptedVersion</span></span>|<span data-ttu-id="5966d-135">Int32</span><span class="sxs-lookup"><span data-stu-id="5966d-135">Int32</span></span>|<span data-ttu-id="5966d-136">ユーザーによって承諾された使用条件の最新バージョン番号。</span><span class="sxs-lookup"><span data-stu-id="5966d-136">Most recent version number of the T&C accepted by the user.</span></span>|
|<span data-ttu-id="5966d-137">acceptedDateTime</span><span class="sxs-lookup"><span data-stu-id="5966d-137">acceptedDateTime</span></span>|<span data-ttu-id="5966d-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5966d-138">DateTimeOffset</span></span>|<span data-ttu-id="5966d-139">最後に使用条件がユーザーによって承諾された DateTime。</span><span class="sxs-lookup"><span data-stu-id="5966d-139">DateTime when the terms were last accepted by the user.</span></span>|

## <a name="relationships"></a><span data-ttu-id="5966d-140">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="5966d-140">Relationships</span></span>
|<span data-ttu-id="5966d-141">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="5966d-141">Relationship</span></span>|<span data-ttu-id="5966d-142">型</span><span class="sxs-lookup"><span data-stu-id="5966d-142">Type</span></span>|<span data-ttu-id="5966d-143">説明</span><span class="sxs-lookup"><span data-stu-id="5966d-143">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5966d-144">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="5966d-144">termsAndConditions</span></span>|[<span data-ttu-id="5966d-145">termsAndConditions</span><span class="sxs-lookup"><span data-stu-id="5966d-145">termsAndConditions</span></span>](../resources/intune_companyterms_termsandconditions.md)|<span data-ttu-id="5966d-146">割り当てられた使用条件へのナビゲーション リンク。</span><span class="sxs-lookup"><span data-stu-id="5966d-146">Navigation link to the terms and conditions that are assigned.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="5966d-147">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5966d-147">JSON Representation</span></span>
<span data-ttu-id="5966d-148">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="5966d-148">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termsAndConditionsAcceptanceStatus"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
  "id": "String (identifier)",
  "userDisplayName": "String",
  "acceptedVersion": 1024,
  "acceptedDateTime": "String (timestamp)"
}
```








