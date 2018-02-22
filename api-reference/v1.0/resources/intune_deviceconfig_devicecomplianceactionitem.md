# <a name="devicecomplianceactionitem-resource-type"></a><span data-ttu-id="82cf3-101">deviceComplianceActionItem リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="82cf3-101">deviceComplianceActionItem resource type</span></span>

> <span data-ttu-id="82cf3-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="82cf3-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="82cf3-103">スケジュール済みのアクションの構成</span><span class="sxs-lookup"><span data-stu-id="82cf3-103">Scheduled Action Configuration</span></span>
## <a name="methods"></a><span data-ttu-id="82cf3-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="82cf3-104">Methods</span></span>
|<span data-ttu-id="82cf3-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="82cf3-105">Method</span></span>|<span data-ttu-id="82cf3-106">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="82cf3-106">Return Type</span></span>|<span data-ttu-id="82cf3-107">説明</span><span class="sxs-lookup"><span data-stu-id="82cf3-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="82cf3-108">List deviceComplianceActionItems</span><span class="sxs-lookup"><span data-stu-id="82cf3-108">List deviceComplianceActionItems</span></span>](../api/intune_deviceconfig_devicecomplianceactionitem_list.md)|<span data-ttu-id="82cf3-109">[deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="82cf3-109">[deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md) collection</span></span>|<span data-ttu-id="82cf3-110">[deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="82cf3-110">List properties and relationships of the [deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md) objects.</span></span>|
|[<span data-ttu-id="82cf3-111">Get deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="82cf3-111">Get deviceComplianceActionItem</span></span>](../api/intune_deviceconfig_devicecomplianceactionitem_get.md)|[<span data-ttu-id="82cf3-112">deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="82cf3-112">deviceComplianceActionItem</span></span>](../resources/intune_deviceconfig_devicecomplianceactionitem.md)|<span data-ttu-id="82cf3-113">[deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="82cf3-113">Read properties and relationships of [plannerAssignedToTaskBoardTaskFormat](../resources/intune_deviceconfig_devicecomplianceactionitem.md) object.</span></span>|
|[<span data-ttu-id="82cf3-114">Create deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="82cf3-114">Create deviceComplianceActionItem</span></span>](../api/intune_deviceconfig_devicecomplianceactionitem_create.md)|[<span data-ttu-id="82cf3-115">deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="82cf3-115">deviceComplianceActionItem</span></span>](../resources/intune_deviceconfig_devicecomplianceactionitem.md)|<span data-ttu-id="82cf3-116">新しい [deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="82cf3-116">Create a new [plannerBucket](../resources/intune_deviceconfig_devicecomplianceactionitem.md) object.</span></span>|
|[<span data-ttu-id="82cf3-117">Delete deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="82cf3-117">Delete deviceComplianceActionItem</span></span>](../api/intune_deviceconfig_devicecomplianceactionitem_delete.md)|<span data-ttu-id="82cf3-118">なし</span><span class="sxs-lookup"><span data-stu-id="82cf3-118">None</span></span>|<span data-ttu-id="82cf3-119">[deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="82cf3-119">Deletes a [deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md).</span></span>|
|[<span data-ttu-id="82cf3-120">Update deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="82cf3-120">Update deviceComplianceActionItem</span></span>](../api/intune_deviceconfig_devicecomplianceactionitem_update.md)|[<span data-ttu-id="82cf3-121">deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="82cf3-121">deviceComplianceActionItem</span></span>](../resources/intune_deviceconfig_devicecomplianceactionitem.md)|<span data-ttu-id="82cf3-122">[deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="82cf3-122">Update the properties of a [calendar](../resources/intune_deviceconfig_devicecomplianceactionitem.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="82cf3-123">プロパティ</span><span class="sxs-lookup"><span data-stu-id="82cf3-123">Properties</span></span>
|<span data-ttu-id="82cf3-124">プロパティ</span><span class="sxs-lookup"><span data-stu-id="82cf3-124">Property</span></span>|<span data-ttu-id="82cf3-125">型</span><span class="sxs-lookup"><span data-stu-id="82cf3-125">Type</span></span>|<span data-ttu-id="82cf3-126">説明</span><span class="sxs-lookup"><span data-stu-id="82cf3-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="82cf3-127">id</span><span class="sxs-lookup"><span data-stu-id="82cf3-127">id</span></span>|<span data-ttu-id="82cf3-128">String</span><span class="sxs-lookup"><span data-stu-id="82cf3-128">String</span></span>|<span data-ttu-id="82cf3-129">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="82cf3-129">Name of the entity.</span></span>|
|<span data-ttu-id="82cf3-130">gracePeriodHours</span><span class="sxs-lookup"><span data-stu-id="82cf3-130">gracePeriodHours</span></span>|<span data-ttu-id="82cf3-131">Int32</span><span class="sxs-lookup"><span data-stu-id="82cf3-131">Int32</span></span>|<span data-ttu-id="82cf3-132">アクションが実行されるまでの待機時間。</span><span class="sxs-lookup"><span data-stu-id="82cf3-132">Number of hours to wait till the action will be enforced.</span></span> <span data-ttu-id="82cf3-133">有効な値は 0 から 8760 までです</span><span class="sxs-lookup"><span data-stu-id="82cf3-133">Valid values 0 to 8760</span></span>|
|<span data-ttu-id="82cf3-134">actionType</span><span class="sxs-lookup"><span data-stu-id="82cf3-134">actionType</span></span>|<span data-ttu-id="82cf3-135">String</span><span class="sxs-lookup"><span data-stu-id="82cf3-135">String</span></span>|<span data-ttu-id="82cf3-136">実施するアクション。可能な値は、`noAction`、`notification`、`block`、`retire`、`wipe`、`removeResourceAccessProfiles` です。</span><span class="sxs-lookup"><span data-stu-id="82cf3-136">What action to take Possible values are: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`.</span></span>|
|<span data-ttu-id="82cf3-137">notificationTemplateId</span><span class="sxs-lookup"><span data-stu-id="82cf3-137">notificationTemplateId</span></span>|<span data-ttu-id="82cf3-138">String</span><span class="sxs-lookup"><span data-stu-id="82cf3-138">String</span></span>|<span data-ttu-id="82cf3-139">使用する通知メッセージ テンプレート</span><span class="sxs-lookup"><span data-stu-id="82cf3-139">What notification Message template to use</span></span>|
|<span data-ttu-id="82cf3-140">notificationMessageCCList</span><span class="sxs-lookup"><span data-stu-id="82cf3-140">notificationMessageCCList</span></span>|<span data-ttu-id="82cf3-141">String コレクション</span><span class="sxs-lookup"><span data-stu-id="82cf3-141">String collection</span></span>|<span data-ttu-id="82cf3-142">この通知メッセージの CC に設定するグループ ID のリスト。</span><span class="sxs-lookup"><span data-stu-id="82cf3-142">A list of group IDs to speicify who to CC this notification message to.</span></span>|

## <a name="relationships"></a><span data-ttu-id="82cf3-143">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="82cf3-143">Relationships</span></span>
<span data-ttu-id="82cf3-144">なし</span><span class="sxs-lookup"><span data-stu-id="82cf3-144">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="82cf3-145">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="82cf3-145">JSON Representation</span></span>
<span data-ttu-id="82cf3-146">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="82cf3-146">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceComplianceActionItem"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceComplianceActionItem",
  "id": "String (identifier)",
  "gracePeriodHours": 1024,
  "actionType": "String",
  "notificationTemplateId": "String",
  "notificationMessageCCList": [
    "String"
  ]
}
```



