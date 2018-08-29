# <a name="managedebookassignment-resource-type"></a><span data-ttu-id="5a625-101">managedEBookAssignment リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5a625-101">managedEBookAssignment resource type</span></span>

> <span data-ttu-id="5a625-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="5a625-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5a625-103">グループへの電子ブックの割り当てに使用されるプロパティが含まれています。</span><span class="sxs-lookup"><span data-stu-id="5a625-103">Contains properties used to assign a eBook to a group.</span></span>
## <a name="methods"></a><span data-ttu-id="5a625-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="5a625-104">Methods</span></span>
|<span data-ttu-id="5a625-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="5a625-105">Method</span></span>|<span data-ttu-id="5a625-106">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="5a625-106">Return Type</span></span>|<span data-ttu-id="5a625-107">説明</span><span class="sxs-lookup"><span data-stu-id="5a625-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5a625-108">managedEBookAssignments のリスト</span><span class="sxs-lookup"><span data-stu-id="5a625-108">List managedEBookAssignments</span></span>](../api/intune_books_managedebookassignment_list.md)|<span data-ttu-id="5a625-109">[managedEBookAssignment](../resources/intune_books_managedebookassignment.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="5a625-109">[managedEBookAssignment](../resources/intune_books_managedebookassignment.md) collection</span></span>|<span data-ttu-id="5a625-110">[managedEBookAssignment](../resources/intune_books_managedebookassignment.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="5a625-110">List properties and relationships of the [managedEBookAssignment](../resources/intune_books_managedebookassignment.md) objects.</span></span>|
|[<span data-ttu-id="5a625-111">managedEBookAssignment の取得</span><span class="sxs-lookup"><span data-stu-id="5a625-111">Get managedEBookAssignment</span></span>](../api/intune_books_managedebookassignment_get.md)|[<span data-ttu-id="5a625-112">managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="5a625-112">managedEBookAssignment</span></span>](../resources/intune_books_managedebookassignment.md)|<span data-ttu-id="5a625-113">[managedEBookAssignment](../resources/intune_books_managedebookassignment.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="5a625-113">Read properties and relationships of the [managedEBookAssignment](../resources/intune_books_managedebookassignment.md) object.</span></span>|
|[<span data-ttu-id="5a625-114">managedEBookAssignment の作成</span><span class="sxs-lookup"><span data-stu-id="5a625-114">Create managedEBookAssignment</span></span>](../api/intune_books_managedebookassignment_create.md)|[<span data-ttu-id="5a625-115">managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="5a625-115">managedEBookAssignment</span></span>](../resources/intune_books_managedebookassignment.md)|<span data-ttu-id="5a625-116">新しい [managedEBookAssignment](../resources/intune_books_managedebookassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="5a625-116">Create a new [managedEBookAssignment](../resources/intune_books_managedebookassignment.md) object.</span></span>|
|[<span data-ttu-id="5a625-117">managedEBookAssignment の削除</span><span class="sxs-lookup"><span data-stu-id="5a625-117">Delete managedEBookAssignment</span></span>](../api/intune_books_managedebookassignment_delete.md)|<span data-ttu-id="5a625-118">なし</span><span class="sxs-lookup"><span data-stu-id="5a625-118">None</span></span>|<span data-ttu-id="5a625-119">[managedEBookAssignment](../resources/intune_books_managedebookassignment.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="5a625-119">Deletes a [managedEBookAssignment](../resources/intune_books_managedebookassignment.md).</span></span>|
|[<span data-ttu-id="5a625-120">managedEBookAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="5a625-120">Update managedEBookAssignment</span></span>](../api/intune_books_managedebookassignment_update.md)|[<span data-ttu-id="5a625-121">managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="5a625-121">managedEBookAssignment</span></span>](../resources/intune_books_managedebookassignment.md)|<span data-ttu-id="5a625-122">[managedEBookAssignment](../resources/intune_books_managedebookassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="5a625-122">Update the properties of a [managedEBookAssignment](../resources/intune_books_managedebookassignment.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="5a625-123">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5a625-123">Properties</span></span>
|<span data-ttu-id="5a625-124">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5a625-124">Property</span></span>|<span data-ttu-id="5a625-125">タイプ</span><span class="sxs-lookup"><span data-stu-id="5a625-125">Type</span></span>|<span data-ttu-id="5a625-126">説明</span><span class="sxs-lookup"><span data-stu-id="5a625-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5a625-127">ID</span><span class="sxs-lookup"><span data-stu-id="5a625-127">id</span></span>|<span data-ttu-id="5a625-128">文字列</span><span class="sxs-lookup"><span data-stu-id="5a625-128">String</span></span>|<span data-ttu-id="5a625-129">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="5a625-129">Key of the entity.</span></span>|
|<span data-ttu-id="5a625-130">target</span><span class="sxs-lookup"><span data-stu-id="5a625-130">target</span></span>|[<span data-ttu-id="5a625-131">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="5a625-131">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune_shared_deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="5a625-132">電子ブックの割り当て先。</span><span class="sxs-lookup"><span data-stu-id="5a625-132">The assignment target for eBook.</span></span>|
|<span data-ttu-id="5a625-133">installIntent</span><span class="sxs-lookup"><span data-stu-id="5a625-133">installIntent</span></span>|[<span data-ttu-id="5a625-134">installIntent</span><span class="sxs-lookup"><span data-stu-id="5a625-134">installIntent</span></span>](../resources/intune_shared_installintent.md)|<span data-ttu-id="5a625-135">電子ブックのインストールの目的。</span><span class="sxs-lookup"><span data-stu-id="5a625-135">The install intent for eBook.</span></span> <span data-ttu-id="5a625-136">指定できる値は、`available`、`required`、`uninstall`、`availableWithoutEnrollment` です。</span><span class="sxs-lookup"><span data-stu-id="5a625-136">The possible values are `available`, `required`, `uninstall`, `availableWithoutEnrollment`, , , , , , , , or .</span></span>|

## <a name="relationships"></a><span data-ttu-id="5a625-137">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="5a625-137">Relationships</span></span>
<span data-ttu-id="5a625-138">なし</span><span class="sxs-lookup"><span data-stu-id="5a625-138">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="5a625-139">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5a625-139">JSON Representation</span></span>
<span data-ttu-id="5a625-140">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="5a625-140">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.managedEBookAssignment"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.managedEBookAssignment",
  "id": "String (identifier)",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "installIntent": "String"
}
```



