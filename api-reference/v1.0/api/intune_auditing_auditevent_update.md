# <a name="update-auditevent"></a><span data-ttu-id="b47b2-101">auditEvent の更新</span><span class="sxs-lookup"><span data-stu-id="b47b2-101">Update auditEvent</span></span>

> <span data-ttu-id="b47b2-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b47b2-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b47b2-103">[auditEvent](../resources/intune_auditing_auditevent.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="b47b2-103">Update the properties of a [auditEvent](../resources/intune_auditing_auditevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b47b2-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="b47b2-104">Prerequisites</span></span>
<span data-ttu-id="b47b2-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b47b2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b47b2-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b47b2-107">Permission type</span></span>|<span data-ttu-id="b47b2-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="b47b2-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b47b2-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b47b2-109">Delegated (work or school account)</span></span>|<span data-ttu-id="b47b2-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b47b2-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b47b2-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b47b2-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b47b2-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b47b2-112">Not supported.</span></span>|
|<span data-ttu-id="b47b2-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b47b2-113">Application</span></span>|<span data-ttu-id="b47b2-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b47b2-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b47b2-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b47b2-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/auditEvents/{auditEventId}
```

## <a name="request-headers"></a><span data-ttu-id="b47b2-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b47b2-116">Request headers</span></span>
|<span data-ttu-id="b47b2-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b47b2-117">Header</span></span>|<span data-ttu-id="b47b2-118">値</span><span class="sxs-lookup"><span data-stu-id="b47b2-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b47b2-119">承認</span><span class="sxs-lookup"><span data-stu-id="b47b2-119">Authorization</span></span>|<span data-ttu-id="b47b2-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="b47b2-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b47b2-121">承諾</span><span class="sxs-lookup"><span data-stu-id="b47b2-121">Accept</span></span>|<span data-ttu-id="b47b2-122">アプリケーションまたは JSON</span><span class="sxs-lookup"><span data-stu-id="b47b2-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b47b2-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="b47b2-123">Request body</span></span>
<span data-ttu-id="b47b2-124">要求本文で、[auditEvent](../resources/intune_auditing_auditevent.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="b47b2-124">In the request body, supply a JSON representation for the [auditEvent](../resources/intune_auditing_auditevent.md) object.</span></span>

<span data-ttu-id="b47b2-125">次の表に、[auditEvent](../resources/intune_auditing_auditevent.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="b47b2-125">The following table shows the properties that are required when you create the [auditEvent](../resources/intune_auditing_auditevent.md).</span></span>

|<span data-ttu-id="b47b2-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b47b2-126">Property</span></span>|<span data-ttu-id="b47b2-127">タイプ</span><span class="sxs-lookup"><span data-stu-id="b47b2-127">Type</span></span>|<span data-ttu-id="b47b2-128">説明</span><span class="sxs-lookup"><span data-stu-id="b47b2-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b47b2-129">ID</span><span class="sxs-lookup"><span data-stu-id="b47b2-129">id</span></span>|<span data-ttu-id="b47b2-130">文字列</span><span class="sxs-lookup"><span data-stu-id="b47b2-130">String</span></span>|<span data-ttu-id="b47b2-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="b47b2-131">Key of the entity.</span></span>|
|<span data-ttu-id="b47b2-132">displayName</span><span class="sxs-lookup"><span data-stu-id="b47b2-132">displayName</span></span>|<span data-ttu-id="b47b2-133">文字列</span><span class="sxs-lookup"><span data-stu-id="b47b2-133">String</span></span>|<span data-ttu-id="b47b2-134">イベントの表示名。</span><span class="sxs-lookup"><span data-stu-id="b47b2-134">Event display name.</span></span>|
|<span data-ttu-id="b47b2-135">componentName</span><span class="sxs-lookup"><span data-stu-id="b47b2-135">componentName</span></span>|<span data-ttu-id="b47b2-136">文字列</span><span class="sxs-lookup"><span data-stu-id="b47b2-136">String</span></span>|<span data-ttu-id="b47b2-137">コンポーネント名。</span><span class="sxs-lookup"><span data-stu-id="b47b2-137">Component name.</span></span>|
|<span data-ttu-id="b47b2-138">アクター</span><span class="sxs-lookup"><span data-stu-id="b47b2-138">actor</span></span>|[<span data-ttu-id="b47b2-139">auditActor</span><span class="sxs-lookup"><span data-stu-id="b47b2-139">auditActor</span></span>](../resources/intune_auditing_auditactor.md)|<span data-ttu-id="b47b2-140">監査イベントに関連付けられている AAD ユーザーとアプリケーション。</span><span class="sxs-lookup"><span data-stu-id="b47b2-140">AAD user and application that are associated with the audit event.</span></span>|
|<span data-ttu-id="b47b2-141">アクティビティ</span><span class="sxs-lookup"><span data-stu-id="b47b2-141">activity</span></span>|<span data-ttu-id="b47b2-142">文字列</span><span class="sxs-lookup"><span data-stu-id="b47b2-142">String</span></span>|<span data-ttu-id="b47b2-143">わかりやすいアクティビティの名前。</span><span class="sxs-lookup"><span data-stu-id="b47b2-143">Friendly name of the activity.</span></span>|
|<span data-ttu-id="b47b2-144">activityDateTime</span><span class="sxs-lookup"><span data-stu-id="b47b2-144">activityDateTime</span></span>|<span data-ttu-id="b47b2-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b47b2-145">DateTimeOffset</span></span>|<span data-ttu-id="b47b2-146">アクティビティが実行された日時 (UTC)。</span><span class="sxs-lookup"><span data-stu-id="b47b2-146">The date time in UTC when the activity was performed.</span></span>|
|<span data-ttu-id="b47b2-147">activityType</span><span class="sxs-lookup"><span data-stu-id="b47b2-147">activityType</span></span>|<span data-ttu-id="b47b2-148">文字列</span><span class="sxs-lookup"><span data-stu-id="b47b2-148">String</span></span>|<span data-ttu-id="b47b2-149">実行されたアクティビティの種類。</span><span class="sxs-lookup"><span data-stu-id="b47b2-149">The type of activity that was being performed.</span></span>|
|<span data-ttu-id="b47b2-150">activityOperationType</span><span class="sxs-lookup"><span data-stu-id="b47b2-150">activityOperationType</span></span>|<span data-ttu-id="b47b2-151">文字列</span><span class="sxs-lookup"><span data-stu-id="b47b2-151">String</span></span>|<span data-ttu-id="b47b2-152">アクティビティの HTTP 操作の種類。</span><span class="sxs-lookup"><span data-stu-id="b47b2-152">The HTTP operation type of the activity.</span></span>|
|<span data-ttu-id="b47b2-153">activityResult</span><span class="sxs-lookup"><span data-stu-id="b47b2-153">activityResult</span></span>|<span data-ttu-id="b47b2-154">文字列</span><span class="sxs-lookup"><span data-stu-id="b47b2-154">String</span></span>|<span data-ttu-id="b47b2-155">アクティビティの結果。</span><span class="sxs-lookup"><span data-stu-id="b47b2-155">The result of the activity.</span></span>|
|<span data-ttu-id="b47b2-156">correlationId</span><span class="sxs-lookup"><span data-stu-id="b47b2-156">correlationId</span></span>|<span data-ttu-id="b47b2-157">Guid</span><span class="sxs-lookup"><span data-stu-id="b47b2-157">Guid</span></span>|<span data-ttu-id="b47b2-158">システム内でのアクティビティに関連付けるために使用されるクライアント要求 ID。</span><span class="sxs-lookup"><span data-stu-id="b47b2-158">The client request Id that is used to correlate activity within the system.</span></span>|
|<span data-ttu-id="b47b2-159">リソース</span><span class="sxs-lookup"><span data-stu-id="b47b2-159">resources</span></span>|<span data-ttu-id="b47b2-160">[auditResource](../resources/intune_auditing_auditresource.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b47b2-160">[auditResource](../resources/intune_auditing_auditresource.md) collection</span></span>|<span data-ttu-id="b47b2-161">変更中のリソースです。</span><span class="sxs-lookup"><span data-stu-id="b47b2-161">Resources being modified.</span></span>|
|<span data-ttu-id="b47b2-162">カテゴリ</span><span class="sxs-lookup"><span data-stu-id="b47b2-162">category</span></span>|<span data-ttu-id="b47b2-163">文字列</span><span class="sxs-lookup"><span data-stu-id="b47b2-163">String</span></span>|<span data-ttu-id="b47b2-164">監査のカテゴリです。</span><span class="sxs-lookup"><span data-stu-id="b47b2-164">Audit category.</span></span>|



## <a name="response"></a><span data-ttu-id="b47b2-165">応答</span><span class="sxs-lookup"><span data-stu-id="b47b2-165">Response</span></span>
<span data-ttu-id="b47b2-166">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [auditEvent](../resources/intune_auditing_auditevent.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="b47b2-166">If successful, this method returns a `200 OK` response code and an updated [auditEvent](../resources/intune_auditing_auditevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b47b2-167">例</span><span class="sxs-lookup"><span data-stu-id="b47b2-167">Example</span></span>
### <a name="request"></a><span data-ttu-id="b47b2-168">要求</span><span class="sxs-lookup"><span data-stu-id="b47b2-168">Request</span></span>
<span data-ttu-id="b47b2-169">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b47b2-169">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/auditEvents/{auditEventId}
Content-type: application/json
Content-length: 1338

{
  "displayName": "Display Name value",
  "componentName": "Component Name value",
  "actor": {
    "@odata.type": "microsoft.graph.auditActor",
    "type": "Type value",
    "userPermissions": [
      "User Permissions value"
    ],
    "applicationId": "Application Id value",
    "applicationDisplayName": "Application Display Name value",
    "userPrincipalName": "User Principal Name value",
    "servicePrincipalName": "Service Principal Name value",
    "ipAddress": "Ip Address value",
    "userId": "User Id value"
  },
  "activity": "Activity value",
  "activityDateTime": "2016-12-31T23:59:51.6363086-08:00",
  "activityType": "Activity Type value",
  "activityOperationType": "Activity Operation Type value",
  "activityResult": "Activity Result value",
  "correlationId": "<Unknown Primitive Type Edm.Guid>",
  "resources": [
    {
      "@odata.type": "microsoft.graph.auditResource",
      "displayName": "Display Name value",
      "modifiedProperties": [
        {
          "@odata.type": "microsoft.graph.auditProperty",
          "displayName": "Display Name value",
          "oldValue": "Old Value value",
          "newValue": "New Value value"
        }
      ],
      "type": "Type value",
      "resourceId": "Resource Id value"
    }
  ],
  "category": "Category value"
}
```

### <a name="response"></a><span data-ttu-id="b47b2-170">応答</span><span class="sxs-lookup"><span data-stu-id="b47b2-170">Response</span></span>
<span data-ttu-id="b47b2-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b47b2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1436

{
  "@odata.type": "#microsoft.graph.auditEvent",
  "id": "59653ce8-3ce8-5965-e83c-6559e83c6559",
  "displayName": "Display Name value",
  "componentName": "Component Name value",
  "actor": {
    "@odata.type": "microsoft.graph.auditActor",
    "type": "Type value",
    "userPermissions": [
      "User Permissions value"
    ],
    "applicationId": "Application Id value",
    "applicationDisplayName": "Application Display Name value",
    "userPrincipalName": "User Principal Name value",
    "servicePrincipalName": "Service Principal Name value",
    "ipAddress": "Ip Address value",
    "userId": "User Id value"
  },
  "activity": "Activity value",
  "activityDateTime": "2016-12-31T23:59:51.6363086-08:00",
  "activityType": "Activity Type value",
  "activityOperationType": "Activity Operation Type value",
  "activityResult": "Activity Result value",
  "correlationId": "<Unknown Primitive Type Edm.Guid>",
  "resources": [
    {
      "@odata.type": "microsoft.graph.auditResource",
      "displayName": "Display Name value",
      "modifiedProperties": [
        {
          "@odata.type": "microsoft.graph.auditProperty",
          "displayName": "Display Name value",
          "oldValue": "Old Value value",
          "newValue": "New Value value"
        }
      ],
      "type": "Type value",
      "resourceId": "Resource Id value"
    }
  ],
  "category": "Category value"
}
```








