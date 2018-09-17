# <a name="auditevent-resource-type"></a><span data-ttu-id="4b94a-101">auditEvent リソース タイプ</span><span class="sxs-lookup"><span data-stu-id="4b94a-101">auditEvent resource type</span></span>

> <span data-ttu-id="4b94a-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="4b94a-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4b94a-103">監査イベントのプロパティが含まれるクラス。</span><span class="sxs-lookup"><span data-stu-id="4b94a-103">A class containing the properties for Audit Event.</span></span>
## <a name="methods"></a><span data-ttu-id="4b94a-104">メソッド</span><span class="sxs-lookup"><span data-stu-id="4b94a-104">Methods</span></span>
|<span data-ttu-id="4b94a-105">メソッド</span><span class="sxs-lookup"><span data-stu-id="4b94a-105">Method</span></span>|<span data-ttu-id="4b94a-106">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="4b94a-106">Return Type</span></span>|<span data-ttu-id="4b94a-107">説明</span><span class="sxs-lookup"><span data-stu-id="4b94a-107">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="4b94a-108">auditEvents をリストします。</span><span class="sxs-lookup"><span data-stu-id="4b94a-108">List auditEvents</span></span>](../api/intune_auditing_auditevent_list.md)|<span data-ttu-id="4b94a-109">[auditEvent](../resources/intune_auditing_auditevent.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="4b94a-109">[auditEvent](../resources/intune_auditing_auditevent.md) collection</span></span>|<span data-ttu-id="4b94a-110">[auditEvent](../resources/intune_auditing_auditevent.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="4b94a-110">List properties and relationships of the [auditEvent](../resources/intune_auditing_auditevent.md) objects.</span></span>|
|[<span data-ttu-id="4b94a-111">auditEvent を取得します。</span><span class="sxs-lookup"><span data-stu-id="4b94a-111">Get auditEvent</span></span>](../api/intune_auditing_auditevent_get.md)|[<span data-ttu-id="4b94a-112">auditEvent</span><span class="sxs-lookup"><span data-stu-id="4b94a-112">auditEvent</span></span>](../resources/intune_auditing_auditevent.md)|<span data-ttu-id="4b94a-113">[auditEvent](../resources/intune_auditing_auditevent.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="4b94a-113">Read properties and relationships of the [auditEvent](../resources/intune_auditing_auditevent.md) object.</span></span>|
|[<span data-ttu-id="4b94a-114">auditEvent を作成します。</span><span class="sxs-lookup"><span data-stu-id="4b94a-114">Create auditEvent</span></span>](../api/intune_auditing_auditevent_create.md)|[<span data-ttu-id="4b94a-115">auditEvent</span><span class="sxs-lookup"><span data-stu-id="4b94a-115">auditEvent</span></span>](../resources/intune_auditing_auditevent.md)|<span data-ttu-id="4b94a-116">新しい [auditEvent](../resources/intune_auditing_auditevent.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="4b94a-116">Create a new [auditEvent](../resources/intune_auditing_auditevent.md) object.</span></span>|
|[<span data-ttu-id="4b94a-117"> auditEvent を削除します。</span><span class="sxs-lookup"><span data-stu-id="4b94a-117">Delete auditEvent</span></span>](../api/intune_auditing_auditevent_delete.md)|<span data-ttu-id="4b94a-118">なし</span><span class="sxs-lookup"><span data-stu-id="4b94a-118">None</span></span>|<span data-ttu-id="4b94a-119">[auditEvent](../resources/intune_auditing_auditevent.md) を削除します。</span><span class="sxs-lookup"><span data-stu-id="4b94a-119">Deletes a [auditEvent](../resources/intune_auditing_auditevent.md).</span></span>|
|[<span data-ttu-id="4b94a-120">auditEvent を更新します。</span><span class="sxs-lookup"><span data-stu-id="4b94a-120">Update auditEvent</span></span>](../api/intune_auditing_auditevent_update.md)|[<span data-ttu-id="4b94a-121">auditEvent</span><span class="sxs-lookup"><span data-stu-id="4b94a-121">auditEvent</span></span>](../resources/intune_auditing_auditevent.md)|<span data-ttu-id="4b94a-122">[auditEvent](../resources/intune_auditing_auditevent.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="4b94a-122">Update the properties of a [auditEvent](../resources/intune_auditing_auditevent.md) object.</span></span>|
|[<span data-ttu-id="4b94a-123">getAuditCategories 関数</span><span class="sxs-lookup"><span data-stu-id="4b94a-123">getAuditCategories function</span></span>](../api/intune_auditing_auditevent_getauditcategories.md)|<span data-ttu-id="4b94a-124">String コレクション</span><span class="sxs-lookup"><span data-stu-id="4b94a-124">String collection</span></span>|<span data-ttu-id="4b94a-125">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="4b94a-125">Not yet documented</span></span>|
|[<span data-ttu-id="4b94a-126">getAuditActivityTypes 関数</span><span class="sxs-lookup"><span data-stu-id="4b94a-126">getAuditActivityTypes function</span></span>](../api/intune_auditing_auditevent_getauditactivitytypes.md)|<span data-ttu-id="4b94a-127">String コレクション</span><span class="sxs-lookup"><span data-stu-id="4b94a-127">String collection</span></span>|<span data-ttu-id="4b94a-128">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="4b94a-128">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="4b94a-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4b94a-129">Properties</span></span>
|<span data-ttu-id="4b94a-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4b94a-130">Property</span></span>|<span data-ttu-id="4b94a-131">型</span><span class="sxs-lookup"><span data-stu-id="4b94a-131">Type</span></span>|<span data-ttu-id="4b94a-132">説明</span><span class="sxs-lookup"><span data-stu-id="4b94a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4b94a-133">ID</span><span class="sxs-lookup"><span data-stu-id="4b94a-133">id</span></span>|<span data-ttu-id="4b94a-134">文字列</span><span class="sxs-lookup"><span data-stu-id="4b94a-134">String</span></span>|<span data-ttu-id="4b94a-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="4b94a-135">Key of the entity.</span></span>|
|<span data-ttu-id="4b94a-136">displayName</span><span class="sxs-lookup"><span data-stu-id="4b94a-136">displayName</span></span>|<span data-ttu-id="4b94a-137">文字列</span><span class="sxs-lookup"><span data-stu-id="4b94a-137">String</span></span>|<span data-ttu-id="4b94a-138">イベントの表示名。</span><span class="sxs-lookup"><span data-stu-id="4b94a-138">Event display name.</span></span>|
|<span data-ttu-id="4b94a-139">componentName</span><span class="sxs-lookup"><span data-stu-id="4b94a-139">componentName</span></span>|<span data-ttu-id="4b94a-140">文字列</span><span class="sxs-lookup"><span data-stu-id="4b94a-140">String</span></span>|<span data-ttu-id="4b94a-141">コンポーネント名。</span><span class="sxs-lookup"><span data-stu-id="4b94a-141">Component name.</span></span>|
|<span data-ttu-id="4b94a-142">アクター</span><span class="sxs-lookup"><span data-stu-id="4b94a-142">actor</span></span>|[<span data-ttu-id="4b94a-143">auditActor</span><span class="sxs-lookup"><span data-stu-id="4b94a-143">auditActor</span></span>](../resources/intune_auditing_auditactor.md)|<span data-ttu-id="4b94a-144">監査イベントに関連付けられている AAD ユーザーとアプリケーション。</span><span class="sxs-lookup"><span data-stu-id="4b94a-144">AAD user and application that are associated with the audit event.</span></span>|
|<span data-ttu-id="4b94a-145">アクティビティ</span><span class="sxs-lookup"><span data-stu-id="4b94a-145">activity</span></span>|<span data-ttu-id="4b94a-146">文字列</span><span class="sxs-lookup"><span data-stu-id="4b94a-146">String</span></span>|<span data-ttu-id="4b94a-147">わかりやすいアクティビティの名前。</span><span class="sxs-lookup"><span data-stu-id="4b94a-147">Friendly name of the activity.</span></span>|
|<span data-ttu-id="4b94a-148">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="4b94a-148">activityDateTime</span></span>|<span data-ttu-id="4b94a-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4b94a-149">DateTimeOffset</span></span>|<span data-ttu-id="4b94a-150">アクティビティが実行された日時 (UTC)。</span><span class="sxs-lookup"><span data-stu-id="4b94a-150">The date time in UTC when the activity was performed.</span></span>|
|<span data-ttu-id="4b94a-151">activityType</span><span class="sxs-lookup"><span data-stu-id="4b94a-151">activityType</span></span>|<span data-ttu-id="4b94a-152">文字列</span><span class="sxs-lookup"><span data-stu-id="4b94a-152">String</span></span>|<span data-ttu-id="4b94a-153">実行されたアクティビティの種類。</span><span class="sxs-lookup"><span data-stu-id="4b94a-153">The type of activity that was being performed.</span></span>|
|<span data-ttu-id="4b94a-154">activityOperationType</span><span class="sxs-lookup"><span data-stu-id="4b94a-154">activityOperationType</span></span>|<span data-ttu-id="4b94a-155">文字列</span><span class="sxs-lookup"><span data-stu-id="4b94a-155">String</span></span>|<span data-ttu-id="4b94a-156">アクティビティの HTTP 操作の種類。</span><span class="sxs-lookup"><span data-stu-id="4b94a-156">The HTTP operation type of the activity.</span></span>|
|<span data-ttu-id="4b94a-157">activityResult</span><span class="sxs-lookup"><span data-stu-id="4b94a-157">activityResult</span></span>|<span data-ttu-id="4b94a-158">文字列</span><span class="sxs-lookup"><span data-stu-id="4b94a-158">String</span></span>|<span data-ttu-id="4b94a-159">アクティビティの結果。</span><span class="sxs-lookup"><span data-stu-id="4b94a-159">The result of the activity.</span></span>|
|<span data-ttu-id="4b94a-160">correlationId</span><span class="sxs-lookup"><span data-stu-id="4b94a-160">correlationId</span></span>|<span data-ttu-id="4b94a-161">GUID</span><span class="sxs-lookup"><span data-stu-id="4b94a-161">Guid</span></span>|<span data-ttu-id="4b94a-162">システム内でのアクティビティに関連付けるために使用されるクライアント要求 ID。</span><span class="sxs-lookup"><span data-stu-id="4b94a-162">The client request Id that is used to correlate activity within the system.</span></span>|
|<span data-ttu-id="4b94a-163">リソース</span><span class="sxs-lookup"><span data-stu-id="4b94a-163">resources</span></span>|<span data-ttu-id="4b94a-164">[auditResource](../resources/intune_auditing_auditresource.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="4b94a-164">[auditResource](../resources/intune_auditing_auditresource.md) collection</span></span>|<span data-ttu-id="4b94a-165">変更中のリソースです。</span><span class="sxs-lookup"><span data-stu-id="4b94a-165">Resources being modified.</span></span>|
|<span data-ttu-id="4b94a-166">カテゴリ</span><span class="sxs-lookup"><span data-stu-id="4b94a-166">category</span></span>|<span data-ttu-id="4b94a-167">文字列</span><span class="sxs-lookup"><span data-stu-id="4b94a-167">String</span></span>|<span data-ttu-id="4b94a-168">監査のカテゴリです。</span><span class="sxs-lookup"><span data-stu-id="4b94a-168">Audit category.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4b94a-169">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4b94a-169">Relationships</span></span>
<span data-ttu-id="4b94a-170">なし</span><span class="sxs-lookup"><span data-stu-id="4b94a-170">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="4b94a-171">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4b94a-171">JSON Representation</span></span>
<span data-ttu-id="4b94a-172">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="4b94a-172">Here is a JSON representation of the resource.</span></span>
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








