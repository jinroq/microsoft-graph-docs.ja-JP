# <a name="create-devicecompliancescheduledactionforrule"></a><span data-ttu-id="a6c5e-101">deviceComplianceScheduledActionForRule の作成</span><span class="sxs-lookup"><span data-stu-id="a6c5e-101">Create deviceComplianceScheduledActionForRule</span></span>

> <span data-ttu-id="a6c5e-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="a6c5e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a6c5e-103">新しい [deviceComplianceScheduledActionForRule](../resources/intune_deviceconfig_devicecompliancescheduledactionforrule.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="a6c5e-103">Create a new [deviceComplianceScheduledActionForRule](../resources/intune_deviceconfig_devicecompliancescheduledactionforrule.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a6c5e-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="a6c5e-104">Prerequisites</span></span>
<span data-ttu-id="a6c5e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a6c5e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a6c5e-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a6c5e-107">Permission type</span></span>|<span data-ttu-id="a6c5e-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a6c5e-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a6c5e-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a6c5e-109">Delegated (work or school account)</span></span>|<span data-ttu-id="a6c5e-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a6c5e-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a6c5e-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a6c5e-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a6c5e-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a6c5e-112">Not supported.</span></span>|
|<span data-ttu-id="a6c5e-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a6c5e-113">Application</span></span>|<span data-ttu-id="a6c5e-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a6c5e-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a6c5e-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a6c5e-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule
```

## <a name="request-headers"></a><span data-ttu-id="a6c5e-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a6c5e-116">Request headers</span></span>
|<span data-ttu-id="a6c5e-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a6c5e-117">Header</span></span>|<span data-ttu-id="a6c5e-118">値</span><span class="sxs-lookup"><span data-stu-id="a6c5e-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a6c5e-119">承認</span><span class="sxs-lookup"><span data-stu-id="a6c5e-119">Authorization</span></span>|<span data-ttu-id="a6c5e-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="a6c5e-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a6c5e-121">承諾</span><span class="sxs-lookup"><span data-stu-id="a6c5e-121">Accept</span></span>|<span data-ttu-id="a6c5e-122">アプリケーションまたは json</span><span class="sxs-lookup"><span data-stu-id="a6c5e-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a6c5e-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="a6c5e-123">Request body</span></span>
<span data-ttu-id="a6c5e-124">要求本文で、deviceComplianceScheduledActionForRule オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="a6c5e-124">In the request body, supply a JSON representation for the deviceComplianceScheduledActionForRule object.</span></span>

<span data-ttu-id="a6c5e-125">次の表に、deviceComplianceScheduledActionForRule の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="a6c5e-125">The following table shows the properties that are required when you create the deviceComplianceScheduledActionForRule.</span></span>

|<span data-ttu-id="a6c5e-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a6c5e-126">Property</span></span>|<span data-ttu-id="a6c5e-127">型</span><span class="sxs-lookup"><span data-stu-id="a6c5e-127">Type</span></span>|<span data-ttu-id="a6c5e-128">説明</span><span class="sxs-lookup"><span data-stu-id="a6c5e-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a6c5e-129">id</span><span class="sxs-lookup"><span data-stu-id="a6c5e-129">id</span></span>|<span data-ttu-id="a6c5e-130">文字列</span><span class="sxs-lookup"><span data-stu-id="a6c5e-130">String</span></span>|<span data-ttu-id="a6c5e-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="a6c5e-131">Key of the entity.</span></span>|
|<span data-ttu-id="a6c5e-132">ruleName</span><span class="sxs-lookup"><span data-stu-id="a6c5e-132">ruleName</span></span>|<span data-ttu-id="a6c5e-133">文字列</span><span class="sxs-lookup"><span data-stu-id="a6c5e-133">String</span></span>|<span data-ttu-id="a6c5e-134">このスケジュール済みのアクションが適用されるルールの名前です。</span><span class="sxs-lookup"><span data-stu-id="a6c5e-134">Name of the rule which this scheduled action applies to.</span></span>|



## <a name="response"></a><span data-ttu-id="a6c5e-135">応答</span><span class="sxs-lookup"><span data-stu-id="a6c5e-135">Response</span></span>
<span data-ttu-id="a6c5e-136">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [deviceComplianceScheduledActionForRule](../resources/intune_deviceconfig_devicecompliancescheduledactionforrule.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a6c5e-136">If successful, this method returns a `201 Created` response code and a [deviceComplianceScheduledActionForRule](../resources/intune_deviceconfig_devicecompliancescheduledactionforrule.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a6c5e-137">例</span><span class="sxs-lookup"><span data-stu-id="a6c5e-137">Example</span></span>
### <a name="request"></a><span data-ttu-id="a6c5e-138">要求</span><span class="sxs-lookup"><span data-stu-id="a6c5e-138">Request</span></span>
<span data-ttu-id="a6c5e-139">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a6c5e-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule
Content-type: application/json
Content-length: 114

{
  "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
  "ruleName": "Rule Name value"
}
```

### <a name="response"></a><span data-ttu-id="a6c5e-140">応答</span><span class="sxs-lookup"><span data-stu-id="a6c5e-140">Response</span></span>
<span data-ttu-id="a6c5e-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a6c5e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 163

{
  "@odata.type": "#microsoft.graph.deviceComplianceScheduledActionForRule",
  "id": "f0075d5e-5d5e-f007-5e5d-07f05e5d07f0",
  "ruleName": "Rule Name value"
}
```








