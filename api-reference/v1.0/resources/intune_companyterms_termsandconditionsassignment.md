# <a name="termsandconditionsassignment-resource-type"></a><span data-ttu-id="0821a-101">termsAndConditionsAssignment リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="0821a-101">termsAndConditionsAssignment resource type</span></span>

> <span data-ttu-id="0821a-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="0821a-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0821a-103">termsAndConditionsAssignment エンティティは、特定の使用条件 (T&C) ポリシーの特定のグループへの割り当てを表します。</span><span class="sxs-lookup"><span data-stu-id="0821a-103">A termsAndConditionsAssignment entity represents the assignment of a given Terms and Conditions (T&C) policy to a given group.</span></span> <span data-ttu-id="0821a-104">グループ内のユーザーは、デバイスを Intune に登録するためには使用条件に同意する必要があります。</span><span class="sxs-lookup"><span data-stu-id="0821a-104">Users in the group will be required to accept the terms in order to have devices enrolled into Intune.</span></span>
## <a name="methods"></a><span data-ttu-id="0821a-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="0821a-105">Methods</span></span>
|<span data-ttu-id="0821a-106">メソッド</span><span class="sxs-lookup"><span data-stu-id="0821a-106">Method</span></span>|<span data-ttu-id="0821a-107">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="0821a-107">Return Type</span></span>|<span data-ttu-id="0821a-108">説明</span><span class="sxs-lookup"><span data-stu-id="0821a-108">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="0821a-109">termsAndConditionsAssignments をリストする</span><span class="sxs-lookup"><span data-stu-id="0821a-109">List termsAndConditionsAssignments</span></span>](../api/intune_companyterms_termsandconditionsassignment_list.md)|<span data-ttu-id="0821a-110">[termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="0821a-110">[termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md) collection</span></span>|<span data-ttu-id="0821a-111">[termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="0821a-111">List properties and relationships of the [termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md) objects.</span></span>|
|[<span data-ttu-id="0821a-112">termsAndConditionsAssignment を取得する</span><span class="sxs-lookup"><span data-stu-id="0821a-112">Get termsAndConditionsAssignment</span></span>](../api/intune_companyterms_termsandconditionsassignment_get.md)|[<span data-ttu-id="0821a-113">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="0821a-113">termsAndConditionsAssignment</span></span>](../resources/intune_companyterms_termsandconditionsassignment.md)|<span data-ttu-id="0821a-114">[termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="0821a-114">Read properties and relationships of the [termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="0821a-115">termsAndConditionsAssignment を作成する</span><span class="sxs-lookup"><span data-stu-id="0821a-115">Create termsAndConditionsAssignment</span></span>](../api/intune_companyterms_termsandconditionsassignment_create.md)|[<span data-ttu-id="0821a-116">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="0821a-116">termsAndConditionsAssignment</span></span>](../resources/intune_companyterms_termsandconditionsassignment.md)|<span data-ttu-id="0821a-117">新しい [termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="0821a-117">Create a new [termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md) object.</span></span>|
|[<span data-ttu-id="0821a-118">termsAndConditionsAssignment を削除する</span><span class="sxs-lookup"><span data-stu-id="0821a-118">Delete termsAndConditionsAssignment</span></span>](../api/intune_companyterms_termsandconditionsassignment_delete.md)|<span data-ttu-id="0821a-119">なし</span><span class="sxs-lookup"><span data-stu-id="0821a-119">None</span></span>|<span data-ttu-id="0821a-120">[termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="0821a-120">Deletes a [termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md).</span></span>|
|[<span data-ttu-id="0821a-121">termsAndConditionsAssignment を更新する</span><span class="sxs-lookup"><span data-stu-id="0821a-121">Update termsAndConditionsAssignment</span></span>](../api/intune_companyterms_termsandconditionsassignment_update.md)|[<span data-ttu-id="0821a-122">termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="0821a-122">termsAndConditionsAssignment</span></span>](../resources/intune_companyterms_termsandconditionsassignment.md)|<span data-ttu-id="0821a-123">[termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="0821a-123">Update the properties of a [termsAndConditionsAssignment](../resources/intune_companyterms_termsandconditionsassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="0821a-124">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0821a-124">Properties</span></span>
|<span data-ttu-id="0821a-125">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0821a-125">Property</span></span>|<span data-ttu-id="0821a-126">タイプ</span><span class="sxs-lookup"><span data-stu-id="0821a-126">Type</span></span>|<span data-ttu-id="0821a-127">説明</span><span class="sxs-lookup"><span data-stu-id="0821a-127">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0821a-128">ID</span><span class="sxs-lookup"><span data-stu-id="0821a-128">id</span></span>|<span data-ttu-id="0821a-129">文字列</span><span class="sxs-lookup"><span data-stu-id="0821a-129">String</span></span>|<span data-ttu-id="0821a-130">エンティティの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="0821a-130">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="0821a-131">ターゲット</span><span class="sxs-lookup"><span data-stu-id="0821a-131">target</span></span>|[<span data-ttu-id="0821a-132">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="0821a-132">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune_shared_deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="0821a-133">T & C ポリシーが割り当てられる、割り当て先です。</span><span class="sxs-lookup"><span data-stu-id="0821a-133">Assignment target that the T&C policy is assigned to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="0821a-134">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="0821a-134">Relationships</span></span>
<span data-ttu-id="0821a-135">なし</span><span class="sxs-lookup"><span data-stu-id="0821a-135">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="0821a-136">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="0821a-136">JSON Representation</span></span>
<span data-ttu-id="0821a-137">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="0821a-137">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "baseType": "microsoft.graph.entity",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termsAndConditionsAssignment"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.termsAndConditionsAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```








