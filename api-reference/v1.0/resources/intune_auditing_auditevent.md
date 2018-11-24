# <a name="auditevent-resource-type"></a><span data-ttu-id="157bb-101">auditEvent リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="157bb-101">auditEvent resource type</span></span>

> <span data-ttu-id="157bb-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="157bb-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="157bb-103">監査イベントのプロパティが含まれるクラス。</span><span class="sxs-lookup"><span data-stu-id="157bb-103">A class containing the properties for Audit Event.</span></span>
## <a name="methods"></a><span data-ttu-id="157bb-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="157bb-104">Methods</span></span>
|<span data-ttu-id="157bb-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="157bb-105">Method</span></span>|<span data-ttu-id="157bb-106">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="157bb-106">Return Type</span></span>|<span data-ttu-id="157bb-107">説明</span><span class="sxs-lookup"><span data-stu-id="157bb-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="157bb-108">List auditEvents</span><span class="sxs-lookup"><span data-stu-id="157bb-108">List auditEvents</span></span>](../api/intune_auditing_auditevent_list.md)|<span data-ttu-id="157bb-109">[auditEvent](../resources/intune_auditing_auditevent.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="157bb-109">[auditEvent](../resources/intune_auditing_auditevent.md) collection</span></span>|<span data-ttu-id="157bb-110">[auditEvent](../resources/intune_auditing_auditevent.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="157bb-110">List properties and relationships of the [auditEvent](../resources/intune_auditing_auditevent.md) objects.</span></span>|
|[<span data-ttu-id="157bb-111">Get auditEvent</span><span class="sxs-lookup"><span data-stu-id="157bb-111">Get auditEvent</span></span>](../api/intune_auditing_auditevent_get.md)|[<span data-ttu-id="157bb-112">auditEvent</span><span class="sxs-lookup"><span data-stu-id="157bb-112">auditEvent</span></span>](../resources/intune_auditing_auditevent.md)|<span data-ttu-id="157bb-113">[auditEvent](../resources/intune_auditing_auditevent.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="157bb-113">Read properties and relationships of the [auditEvent](../resources/intune_auditing_auditevent.md) object.</span></span>|
|[<span data-ttu-id="157bb-114">Create auditEvent</span><span class="sxs-lookup"><span data-stu-id="157bb-114">Create auditEvent</span></span>](../api/intune_auditing_auditevent_create.md)|[<span data-ttu-id="157bb-115">auditEvent</span><span class="sxs-lookup"><span data-stu-id="157bb-115">auditEvent</span></span>](../resources/intune_auditing_auditevent.md)|<span data-ttu-id="157bb-116">新しい [auditEvent](../resources/intune_auditing_auditevent.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="157bb-116">Create a new [auditEvent](../resources/intune_auditing_auditevent.md) object.</span></span>|
|[<span data-ttu-id="157bb-117">Delete auditEvent</span><span class="sxs-lookup"><span data-stu-id="157bb-117">Delete auditEvent</span></span>](../api/intune_auditing_auditevent_delete.md)|<span data-ttu-id="157bb-118">なし</span><span class="sxs-lookup"><span data-stu-id="157bb-118">None</span></span>|<span data-ttu-id="157bb-119">[auditEvent](../resources/intune_auditing_auditevent.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="157bb-119">Deletes a [auditEvent](../resources/intune_auditing_auditevent.md).</span></span>|
|[<span data-ttu-id="157bb-120">Update auditEvent</span><span class="sxs-lookup"><span data-stu-id="157bb-120">Update auditEvent</span></span>](../api/intune_auditing_auditevent_update.md)|[<span data-ttu-id="157bb-121">auditEvent</span><span class="sxs-lookup"><span data-stu-id="157bb-121">auditEvent</span></span>](../resources/intune_auditing_auditevent.md)|<span data-ttu-id="157bb-122">[auditEvent](../resources/intune_auditing_auditevent.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="157bb-122">Update the properties of a [auditEvent](../resources/intune_auditing_auditevent.md) object.</span></span>|
|[<span data-ttu-id="157bb-123">getAuditCategories function</span><span class="sxs-lookup"><span data-stu-id="157bb-123">getAuditCategories function</span></span>](../api/intune_auditing_auditevent_getauditcategories.md)|<span data-ttu-id="157bb-124">String コレクション</span><span class="sxs-lookup"><span data-stu-id="157bb-124">String collection</span></span>|<span data-ttu-id="157bb-125">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="157bb-125">Not yet documented</span></span>|
|[<span data-ttu-id="157bb-126">getAuditActivityTypes function</span><span class="sxs-lookup"><span data-stu-id="157bb-126">getAuditActivityTypes function</span></span>](../api/intune_auditing_auditevent_getauditactivitytypes.md)|<span data-ttu-id="157bb-127">String コレクション</span><span class="sxs-lookup"><span data-stu-id="157bb-127">String collection</span></span>|<span data-ttu-id="157bb-128">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="157bb-128">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="157bb-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="157bb-129">Properties</span></span>
|<span data-ttu-id="157bb-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="157bb-130">Property</span></span>|<span data-ttu-id="157bb-131">型</span><span class="sxs-lookup"><span data-stu-id="157bb-131">Type</span></span>|<span data-ttu-id="157bb-132">説明</span><span class="sxs-lookup"><span data-stu-id="157bb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="157bb-133">id</span><span class="sxs-lookup"><span data-stu-id="157bb-133">id</span></span>|<span data-ttu-id="157bb-134">String</span><span class="sxs-lookup"><span data-stu-id="157bb-134">String</span></span>|<span data-ttu-id="157bb-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="157bb-135">Key of the entity.</span></span>|
|<span data-ttu-id="157bb-136">displayName</span><span class="sxs-lookup"><span data-stu-id="157bb-136">displayName</span></span>|<span data-ttu-id="157bb-137">String</span><span class="sxs-lookup"><span data-stu-id="157bb-137">String</span></span>|<span data-ttu-id="157bb-138">イベントの表示名。</span><span class="sxs-lookup"><span data-stu-id="157bb-138">Event display name.</span></span>|
|<span data-ttu-id="157bb-139">componentName</span><span class="sxs-lookup"><span data-stu-id="157bb-139">componentName</span></span>|<span data-ttu-id="157bb-140">String</span><span class="sxs-lookup"><span data-stu-id="157bb-140">String</span></span>|<span data-ttu-id="157bb-141">コンポーネント名。</span><span class="sxs-lookup"><span data-stu-id="157bb-141">Component name.</span></span>|
|<span data-ttu-id="157bb-142">actor</span><span class="sxs-lookup"><span data-stu-id="157bb-142">actor</span></span>|[<span data-ttu-id="157bb-143">auditActor</span><span class="sxs-lookup"><span data-stu-id="157bb-143">auditActor</span></span>](../resources/intune_auditing_auditactor.md)|<span data-ttu-id="157bb-144">監査イベントに関連付けられている AAD ユーザーとアプリケーション。</span><span class="sxs-lookup"><span data-stu-id="157bb-144">AAD user and application that are associated with the audit event.</span></span>|
|<span data-ttu-id="157bb-145">activity</span><span class="sxs-lookup"><span data-stu-id="157bb-145">activity</span></span>|<span data-ttu-id="157bb-146">String</span><span class="sxs-lookup"><span data-stu-id="157bb-146">String</span></span>|<span data-ttu-id="157bb-147">わかりやすいアクティビティの名前。</span><span class="sxs-lookup"><span data-stu-id="157bb-147">Friendly name of the activity.</span></span>|
|<span data-ttu-id="157bb-148">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="157bb-148">activityDateTime</span></span>|<span data-ttu-id="157bb-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="157bb-149">DateTimeOffset</span></span>|<span data-ttu-id="157bb-150">アクティビティが実行された日時 (UTC)。</span><span class="sxs-lookup"><span data-stu-id="157bb-150">The date time in UTC when the activity was performed.</span></span>|
|<span data-ttu-id="157bb-151">activityType</span><span class="sxs-lookup"><span data-stu-id="157bb-151">activityType</span></span>|<span data-ttu-id="157bb-152">String</span><span class="sxs-lookup"><span data-stu-id="157bb-152">String</span></span>|<span data-ttu-id="157bb-153">実行されたアクティビティの種類。</span><span class="sxs-lookup"><span data-stu-id="157bb-153">The type of activity that was being performed.</span></span>|
|<span data-ttu-id="157bb-154">activityOperationType</span><span class="sxs-lookup"><span data-stu-id="157bb-154">activityOperationType</span></span>|<span data-ttu-id="157bb-155">String</span><span class="sxs-lookup"><span data-stu-id="157bb-155">String</span></span>|<span data-ttu-id="157bb-156">アクティビティの HTTP 操作の種類。</span><span class="sxs-lookup"><span data-stu-id="157bb-156">The HTTP operation type of the activity.</span></span>|
|<span data-ttu-id="157bb-157">activityResult</span><span class="sxs-lookup"><span data-stu-id="157bb-157">activityResult</span></span>|<span data-ttu-id="157bb-158">String</span><span class="sxs-lookup"><span data-stu-id="157bb-158">String</span></span>|<span data-ttu-id="157bb-159">アクティビティの結果。</span><span class="sxs-lookup"><span data-stu-id="157bb-159">The result of the activity.</span></span>|
|<span data-ttu-id="157bb-160">correlationId</span><span class="sxs-lookup"><span data-stu-id="157bb-160">correlationId</span></span>|<span data-ttu-id="157bb-161">Guid</span><span class="sxs-lookup"><span data-stu-id="157bb-161">Guid</span></span>|<span data-ttu-id="157bb-162">システム内でのアクティビティに関連付けるために使用されるクライアント要求 ID。</span><span class="sxs-lookup"><span data-stu-id="157bb-162">The client request Id that is used to correlate activity within the system.</span></span>|
|<span data-ttu-id="157bb-163">resources</span><span class="sxs-lookup"><span data-stu-id="157bb-163">resources</span></span>|<span data-ttu-id="157bb-164">[auditResource](../resources/intune_auditing_auditresource.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="157bb-164">[auditResource](../resources/intune_auditing_auditresource.md) collection</span></span>|<span data-ttu-id="157bb-165">変更中のリソースです。</span><span class="sxs-lookup"><span data-stu-id="157bb-165">Resources being modified.</span></span>|
|<span data-ttu-id="157bb-166">category</span><span class="sxs-lookup"><span data-stu-id="157bb-166">category</span></span>|<span data-ttu-id="157bb-167">String</span><span class="sxs-lookup"><span data-stu-id="157bb-167">String</span></span>|<span data-ttu-id="157bb-168">監査のカテゴリです。</span><span class="sxs-lookup"><span data-stu-id="157bb-168">Audit category.</span></span>|

## <a name="relationships"></a><span data-ttu-id="157bb-169">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="157bb-169">Relationships</span></span>
<span data-ttu-id="157bb-170">なし</span><span class="sxs-lookup"><span data-stu-id="157bb-170">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="157bb-171">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="157bb-171">JSON Representation</span></span>
<span data-ttu-id="157bb-172">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="157bb-172">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.auditEvent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.auditEvent",
  "id": "String (identifier)",
  "displayName": "String",
  "componentName": "String",
  "actor": {
    "@odata.type": "microsoft.graph.auditActor",
    "type": "String",
    "userPermissions": [
      "String"
    ],
    "applicationId": "String",
    "applicationDisplayName": "String",
    "userPrincipalName": "String",
    "servicePrincipalName": "String",
    "ipAddress": "String",
    "userId": "String"
  },
  "activity": "String",
  "activityDateTime": "String (timestamp)",
  "activityType": "String",
  "activityOperationType": "String",
  "activityResult": "String",
  "correlationId": "Guid",
  "resources": [
    {
      "@odata.type": "microsoft.graph.auditResource",
      "displayName": "String",
      "modifiedProperties": [
        {
          "@odata.type": "microsoft.graph.auditProperty",
          "displayName": "String",
          "oldValue": "String",
          "newValue": "String"
        }
      ],
      "type": "String",
      "resourceId": "String"
    }
  ],
  "category": "String"
}
```



