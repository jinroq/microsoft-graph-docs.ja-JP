# <a name="termsandconditionsassignment-resource-type"></a><span data-ttu-id="d3a97-101">termsAndConditionsAssignment リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="d3a97-101">termsAndConditionsAssignment resource type</span></span>

> <span data-ttu-id="d3a97-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="d3a97-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d3a97-103">termsAndConditionsAssignment エンティティは、特定の使用条件 (T&C) ポリシーの特定のグループへの割り当てを表します。</span><span class="sxs-lookup"><span data-stu-id="d3a97-103">A termsAndConditionsAssignment entity represents the assignment of a given Terms and Conditions (T&C) policy to a given group.</span></span> <span data-ttu-id="d3a97-104">グループ内のユーザーは、デバイスを Intune に登録するためには使用条件に同意する必要があります。</span><span class="sxs-lookup"><span data-stu-id="d3a97-104">Users in the group will be required to accept the terms in order to have devices enrolled into Intune.</span></span>
## <a name="methods"></a><span data-ttu-id="d3a97-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="d3a97-105">Methods</span></span>
|<span data-ttu-id="d3a97-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="d3a97-106">Method</span></span>|<span data-ttu-id="d3a97-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="d3a97-107">Return Type</span></span>|<span data-ttu-id="d3a97-108">説明</span><span class="sxs-lookup"><span data-stu-id="d3a97-108">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d3a97-109">List termsAndConditionsAssignments</span><span class="sxs-lookup"><span data-stu-id="d3a97-109">List termsAndConditionsAssignments</span></span>](../api/intune_companyterms_termsandconditionsassignment_list.md)|<span data-ttu-id="d3a97-110">[termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="d3a97-110">[termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md) collection</span></span>|<span data-ttu-id="d3a97-111">[termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="d3a97-111">List properties and relationships of the [termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md) objects.</span></span>|
|[<span data-ttu-id="d3a97-112">Get termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="d3a97-112">Get termsAndConditionsAssignment</span></span>](../api/intune_companyterms_termsandconditionsassignment_get.md)|[<span data-ttu-id="d3a97-113">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="d3a97-113">termsAndConditionsAssignment</span></span>](../resources/intune_companyterms_termsandconditionsassignment.md)|<span data-ttu-id="d3a97-114">[termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="d3a97-114">Read properties and relationships of the [termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="d3a97-115">Create termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="d3a97-115">Create termsAndConditionsAssignment</span></span>](../api/intune_companyterms_termsandconditionsassignment_create.md)|[<span data-ttu-id="d3a97-116">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="d3a97-116">termsAndConditionsAssignment</span></span>](../resources/intune_companyterms_termsandconditionsassignment.md)|<span data-ttu-id="d3a97-117">新しい [termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="d3a97-117">Create a new [termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="d3a97-118">Delete termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="d3a97-118">Delete termsAndConditionsAssignment</span></span>](../api/intune_companyterms_termsandconditionsassignment_delete.md)|<span data-ttu-id="d3a97-119">なし</span><span class="sxs-lookup"><span data-stu-id="d3a97-119">None</span></span>|<span data-ttu-id="d3a97-120">[termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="d3a97-120">Deletes a [termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md).</span></span>|
|[<span data-ttu-id="d3a97-121">Update termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="d3a97-121">Update termsAndConditionsAssignment</span></span>](../api/intune_companyterms_termsandconditionsassignment_update.md)|[<span data-ttu-id="d3a97-122">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="d3a97-122">termsAndConditionsAssignment</span></span>](../resources/intune_companyterms_termsandconditionsassignment.md)|<span data-ttu-id="d3a97-123">[termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="d3a97-123">Update the properties of a [termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="d3a97-124">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d3a97-124">Properties</span></span>
|<span data-ttu-id="d3a97-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d3a97-125">Property</span></span>|<span data-ttu-id="d3a97-126">型</span><span class="sxs-lookup"><span data-stu-id="d3a97-126">Type</span></span>|<span data-ttu-id="d3a97-127">説明</span><span class="sxs-lookup"><span data-stu-id="d3a97-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d3a97-128">id</span><span class="sxs-lookup"><span data-stu-id="d3a97-128">id</span></span>|<span data-ttu-id="d3a97-129">String</span><span class="sxs-lookup"><span data-stu-id="d3a97-129">String</span></span>|<span data-ttu-id="d3a97-130">エンティティの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="d3a97-130">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="d3a97-131">target</span><span class="sxs-lookup"><span data-stu-id="d3a97-131">target</span></span>|[<span data-ttu-id="d3a97-132">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="d3a97-132">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune_shared_deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="d3a97-133">T & C ポリシーが割り当てられる、割り当て先です。</span><span class="sxs-lookup"><span data-stu-id="d3a97-133">Assignment target that the T&C policy is assigned to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d3a97-134">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d3a97-134">Relationships</span></span>
<span data-ttu-id="d3a97-135">なし</span><span class="sxs-lookup"><span data-stu-id="d3a97-135">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="d3a97-136">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d3a97-136">JSON Representation</span></span>
<span data-ttu-id="d3a97-137">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d3a97-137">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termsAndConditionsAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termsAndConditionsAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



