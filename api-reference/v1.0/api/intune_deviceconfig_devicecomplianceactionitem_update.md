# <a name="update-devicecomplianceactionitem"></a><span data-ttu-id="cf786-101">deviceComplianceActionItem の更新</span><span class="sxs-lookup"><span data-stu-id="cf786-101">Update deviceComplianceActionItem</span></span>

> <span data-ttu-id="cf786-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="cf786-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cf786-103">[deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="cf786-103">Update the properties of a [deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cf786-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="cf786-104">Prerequisites</span></span>
<span data-ttu-id="cf786-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cf786-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="cf786-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cf786-107">Permission type</span></span>|<span data-ttu-id="cf786-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="cf786-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cf786-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cf786-109">Delegated (work or school account)</span></span>|<span data-ttu-id="cf786-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf786-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cf786-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cf786-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cf786-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cf786-112">Not supported.</span></span>|
|<span data-ttu-id="cf786-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cf786-113">Application</span></span>|<span data-ttu-id="cf786-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cf786-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cf786-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cf786-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
```

## <a name="request-headers"></a><span data-ttu-id="cf786-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cf786-116">Request headers</span></span>
|<span data-ttu-id="cf786-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cf786-117">Header</span></span>|<span data-ttu-id="cf786-118">値</span><span class="sxs-lookup"><span data-stu-id="cf786-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cf786-119">承認</span><span class="sxs-lookup"><span data-stu-id="cf786-119">Authorization</span></span>|<span data-ttu-id="cf786-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="cf786-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cf786-121">承諾する</span><span class="sxs-lookup"><span data-stu-id="cf786-121">Accept</span></span>|<span data-ttu-id="cf786-122">アプリケーションまたは json</span><span class="sxs-lookup"><span data-stu-id="cf786-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cf786-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="cf786-123">Request body</span></span>
<span data-ttu-id="cf786-124">要求本文で、[deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="cf786-124">In the request body, supply a JSON representation for the [deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md) object.</span></span>

<span data-ttu-id="cf786-125">次の表に、[deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="cf786-125">The following table shows the properties that are required when you create the [deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md).</span></span>

|<span data-ttu-id="cf786-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="cf786-126">Property</span></span>|<span data-ttu-id="cf786-127">型</span><span class="sxs-lookup"><span data-stu-id="cf786-127">Type</span></span>|<span data-ttu-id="cf786-128">説明</span><span class="sxs-lookup"><span data-stu-id="cf786-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cf786-129">ID</span><span class="sxs-lookup"><span data-stu-id="cf786-129">id</span></span>|<span data-ttu-id="cf786-130">文字列</span><span class="sxs-lookup"><span data-stu-id="cf786-130">String</span></span>|<span data-ttu-id="cf786-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="cf786-131">Key of the entity.</span></span>|
|<span data-ttu-id="cf786-132">gracePeriodHours</span><span class="sxs-lookup"><span data-stu-id="cf786-132">gracePeriodHours</span></span>|<span data-ttu-id="cf786-133">Int32</span><span class="sxs-lookup"><span data-stu-id="cf786-133">Int32</span></span>|<span data-ttu-id="cf786-134">アクションが実行されるまでの待機時間。</span><span class="sxs-lookup"><span data-stu-id="cf786-134">Number of hours to wait till the action will be enforced.</span></span> <span data-ttu-id="cf786-135">有効な値は 0 から 8760 までです</span><span class="sxs-lookup"><span data-stu-id="cf786-135">Valid values 0 to 8760</span></span>|
|<span data-ttu-id="cf786-136">actionType</span><span class="sxs-lookup"><span data-stu-id="cf786-136">actionType</span></span>|[<span data-ttu-id="cf786-137">deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="cf786-137">deviceComplianceActionType</span></span>](../resources/intune_deviceconfig_devicecomplianceactiontype.md)|<span data-ttu-id="cf786-138">実行するアクションです。</span><span class="sxs-lookup"><span data-stu-id="cf786-138">What action to take.</span></span> <span data-ttu-id="cf786-139">可能な値は、`noAction`、`notification`、`block`、`retire`、`wipe`、`removeResourceAccessProfiles`、`pushNotification` です。</span><span class="sxs-lookup"><span data-stu-id="cf786-139">Possible values are: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`.</span></span>|
|<span data-ttu-id="cf786-140">notificationTemplateId</span><span class="sxs-lookup"><span data-stu-id="cf786-140">notificationTemplateId</span></span>|<span data-ttu-id="cf786-141">文字列</span><span class="sxs-lookup"><span data-stu-id="cf786-141">String</span></span>|<span data-ttu-id="cf786-142">使用する通知メッセージ テンプレート</span><span class="sxs-lookup"><span data-stu-id="cf786-142">What notification Message template to use</span></span>|
|<span data-ttu-id="cf786-143">notificationMessageCCList</span><span class="sxs-lookup"><span data-stu-id="cf786-143">notificationMessageCCList</span></span>|<span data-ttu-id="cf786-144">String コレクション</span><span class="sxs-lookup"><span data-stu-id="cf786-144">String collection</span></span>|<span data-ttu-id="cf786-145">この通知メッセージの CC に設定するグループ ID のリスト。</span><span class="sxs-lookup"><span data-stu-id="cf786-145">A list of group IDs to speicify who to CC this notification message to.</span></span>|



## <a name="response"></a><span data-ttu-id="cf786-146">応答</span><span class="sxs-lookup"><span data-stu-id="cf786-146">Response</span></span>
<span data-ttu-id="cf786-147">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="cf786-147">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceActionItem](../resources/intune_deviceconfig_devicecomplianceactionitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf786-148">例</span><span class="sxs-lookup"><span data-stu-id="cf786-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="cf786-149">要求</span><span class="sxs-lookup"><span data-stu-id="cf786-149">Request</span></span>
<span data-ttu-id="cf786-150">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="cf786-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
Content-type: application/json
Content-length: 206

{
  "gracePeriodHours": 0,
  "actionType": "notification",
  "notificationTemplateId": "Notification Template Id value",
  "notificationMessageCCList": [
    "Notification Message CCList value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="cf786-151">応答</span><span class="sxs-lookup"><span data-stu-id="cf786-151">Response</span></span>
<span data-ttu-id="cf786-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="cf786-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 320

{
  "@odata.type": "#microsoft.graph.deviceComplianceActionItem",
  "id": "e01a1893-1893-e01a-9318-1ae093181ae0",
  "gracePeriodHours": 0,
  "actionType": "notification",
  "notificationTemplateId": "Notification Template Id value",
  "notificationMessageCCList": [
    "Notification Message CCList value"
  ]
}
```








