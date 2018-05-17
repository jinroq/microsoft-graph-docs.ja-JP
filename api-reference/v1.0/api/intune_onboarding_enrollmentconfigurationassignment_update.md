# <a name="update-enrollmentconfigurationassignment"></a><span data-ttu-id="9bc7c-101">enrollmentConfigurationAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="9bc7c-101">Update enrollmentConfigurationAssignment</span></span>

> <span data-ttu-id="9bc7c-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="9bc7c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9bc7c-103">[enrollmentConfigurationAssignment](../resources/intune_onboarding_enrollmentconfigurationassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="9bc7c-103">Update the properties of a [enrollmentConfigurationAssignment](../resources/intune_onboarding_enrollmentconfigurationassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9bc7c-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="9bc7c-104">Prerequisites</span></span>
<span data-ttu-id="9bc7c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9bc7c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9bc7c-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9bc7c-107">Permission type</span></span>|<span data-ttu-id="9bc7c-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="9bc7c-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9bc7c-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9bc7c-109">Delegated (work or school account)</span></span>|<span data-ttu-id="9bc7c-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9bc7c-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="9bc7c-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9bc7c-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9bc7c-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9bc7c-112">Not supported.</span></span>|
|<span data-ttu-id="9bc7c-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9bc7c-113">Application</span></span>|<span data-ttu-id="9bc7c-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9bc7c-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9bc7c-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9bc7c-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments/{enrollmentConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="9bc7c-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9bc7c-116">Request headers</span></span>
|<span data-ttu-id="9bc7c-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9bc7c-117">Header</span></span>|<span data-ttu-id="9bc7c-118">値</span><span class="sxs-lookup"><span data-stu-id="9bc7c-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9bc7c-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="9bc7c-119">Authorization</span></span>|<span data-ttu-id="9bc7c-120">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="9bc7c-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9bc7c-121">Accept</span><span class="sxs-lookup"><span data-stu-id="9bc7c-121">Accept</span></span>|<span data-ttu-id="9bc7c-122">application/json</span><span class="sxs-lookup"><span data-stu-id="9bc7c-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9bc7c-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="9bc7c-123">Request body</span></span>
<span data-ttu-id="9bc7c-124">要求本文で、[enrollmentConfigurationAssignment](../resources/intune_onboarding_enrollmentconfigurationassignment.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="9bc7c-124">In the request body, supply a JSON representation for the [enrollmentConfigurationAssignment](../resources/intune_onboarding_enrollmentconfigurationassignment.md) object.</span></span>

<span data-ttu-id="9bc7c-125">次の表に、[enrollmentConfigurationAssignment](../resources/intune_onboarding_enrollmentconfigurationassignment.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="9bc7c-125">The following table shows the properties that are required when you create the [enrollmentConfigurationAssignment](../resources/intune_onboarding_enrollmentconfigurationassignment.md).</span></span>

|<span data-ttu-id="9bc7c-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9bc7c-126">Property</span></span>|<span data-ttu-id="9bc7c-127">型</span><span class="sxs-lookup"><span data-stu-id="9bc7c-127">Type</span></span>|<span data-ttu-id="9bc7c-128">説明</span><span class="sxs-lookup"><span data-stu-id="9bc7c-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9bc7c-129">id</span><span class="sxs-lookup"><span data-stu-id="9bc7c-129">id</span></span>|<span data-ttu-id="9bc7c-130">String</span><span class="sxs-lookup"><span data-stu-id="9bc7c-130">String</span></span>|<span data-ttu-id="9bc7c-131">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="9bc7c-131">Not yet documented</span></span>|
|<span data-ttu-id="9bc7c-132">target</span><span class="sxs-lookup"><span data-stu-id="9bc7c-132">target</span></span>|[<span data-ttu-id="9bc7c-133">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="9bc7c-133">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune_shared_deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="9bc7c-134">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="9bc7c-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="9bc7c-135">応答</span><span class="sxs-lookup"><span data-stu-id="9bc7c-135">Response</span></span>
<span data-ttu-id="9bc7c-136">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [enrollmentConfigurationAssignment](../resources/intune_onboarding_enrollmentconfigurationassignment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="9bc7c-136">If successful, this method returns a `200 OK` response code and an updated [enrollmentConfigurationAssignment](../resources/intune_onboarding_enrollmentconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9bc7c-137">例</span><span class="sxs-lookup"><span data-stu-id="9bc7c-137">Example</span></span>
### <a name="request"></a><span data-ttu-id="9bc7c-138">要求</span><span class="sxs-lookup"><span data-stu-id="9bc7c-138">Request</span></span>
<span data-ttu-id="9bc7c-139">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9bc7c-139">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments/{enrollmentConfigurationAssignmentId}
Content-type: application/json
Content-length: 101

{
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="9bc7c-140">応答</span><span class="sxs-lookup"><span data-stu-id="9bc7c-140">Response</span></span>
<span data-ttu-id="9bc7c-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="9bc7c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 222

{
  "@odata.type": "#microsoft.graph.enrollmentConfigurationAssignment",
  "id": "705b021c-021c-705b-1c02-5b701c025b70",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```



