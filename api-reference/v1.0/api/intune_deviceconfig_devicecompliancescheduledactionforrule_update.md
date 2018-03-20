# <a name="update-devicecompliancescheduledactionforrule"></a><span data-ttu-id="b0754-101">deviceComplianceScheduledActionForRule の更新</span><span class="sxs-lookup"><span data-stu-id="b0754-101">Update deviceComplianceScheduledActionForRule</span></span>

> <span data-ttu-id="b0754-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b0754-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b0754-103">[deviceComplianceScheduledActionForRule](../resources/intune_deviceconfig_devicecompliancescheduledactionforrule.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="b0754-103">Update the properties of a [calendar](../resources/intune_deviceconfig_devicecompliancescheduledactionforrule.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b0754-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="b0754-104">Prerequisites</span></span>
<span data-ttu-id="b0754-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b0754-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="b0754-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b0754-107">Permission type</span></span>|<span data-ttu-id="b0754-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="b0754-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b0754-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b0754-109">Delegated (work or school account)</span></span>|<span data-ttu-id="b0754-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0754-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b0754-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b0754-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b0754-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b0754-112">Not supported.</span></span>|
|<span data-ttu-id="b0754-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b0754-113">Application</span></span>|<span data-ttu-id="b0754-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b0754-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b0754-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b0754-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}
```

## <a name="request-headers"></a><span data-ttu-id="b0754-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b0754-116">Request headers</span></span>
|<span data-ttu-id="b0754-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b0754-117">Header</span></span>|<span data-ttu-id="b0754-118">値</span><span class="sxs-lookup"><span data-stu-id="b0754-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b0754-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="b0754-119">Authorization</span></span>|<span data-ttu-id="b0754-120">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="b0754-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="b0754-121">Accept</span><span class="sxs-lookup"><span data-stu-id="b0754-121">Accept</span></span>|<span data-ttu-id="b0754-122">application/json</span><span class="sxs-lookup"><span data-stu-id="b0754-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b0754-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="b0754-123">Request body</span></span>
<span data-ttu-id="b0754-124">要求本文で、[deviceComplianceScheduledActionForRule](../resources/intune_deviceconfig_devicecompliancescheduledactionforrule.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="b0754-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_deviceconfig_devicecompliancescheduledactionforrule.md) object.</span></span>

<span data-ttu-id="b0754-125">次の表に、[deviceComplianceScheduledActionForRule](../resources/intune_deviceconfig_devicecompliancescheduledactionforrule.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="b0754-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="b0754-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b0754-126">Property</span></span>|<span data-ttu-id="b0754-127">型</span><span class="sxs-lookup"><span data-stu-id="b0754-127">Type</span></span>|<span data-ttu-id="b0754-128">説明</span><span class="sxs-lookup"><span data-stu-id="b0754-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0754-129">id</span><span class="sxs-lookup"><span data-stu-id="b0754-129">id</span></span>|<span data-ttu-id="b0754-130">String</span><span class="sxs-lookup"><span data-stu-id="b0754-130">String</span></span>|<span data-ttu-id="b0754-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="b0754-131">Name of the entity.</span></span>|
|<span data-ttu-id="b0754-132">ruleName</span><span class="sxs-lookup"><span data-stu-id="b0754-132">ruleName</span></span>|<span data-ttu-id="b0754-133">String</span><span class="sxs-lookup"><span data-stu-id="b0754-133">String</span></span>|<span data-ttu-id="b0754-134">このスケジュール済みのアクションが適用されるルールの名前です。</span><span class="sxs-lookup"><span data-stu-id="b0754-134">Name of the rule which this scheduled action applies to.</span></span>|



## <a name="response"></a><span data-ttu-id="b0754-135">応答</span><span class="sxs-lookup"><span data-stu-id="b0754-135">Response</span></span>
<span data-ttu-id="b0754-136">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [deviceComplianceScheduledActionForRule](../resources/intune_deviceconfig_devicecompliancescheduledactionforrule.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="b0754-136">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_deviceconfig_devicecompliancescheduledactionforrule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b0754-137">例</span><span class="sxs-lookup"><span data-stu-id="b0754-137">Example</span></span>
### <a name="request"></a><span data-ttu-id="b0754-138">要求</span><span class="sxs-lookup"><span data-stu-id="b0754-138">Request</span></span>
<span data-ttu-id="b0754-139">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b0754-139">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}
Content-type: application/json
Content-length: 37

{
  "ruleName": "Rule Name value"
}
```

### <a name="response"></a><span data-ttu-id="b0754-140">応答</span><span class="sxs-lookup"><span data-stu-id="b0754-140">Response</span></span>
<span data-ttu-id="b0754-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b0754-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 163

{
  "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
  "id": "f0075d5e-5d5e-f007-5e5d-07f05e5d07f0",
  "ruleName": "Rule Name value"
}
```



