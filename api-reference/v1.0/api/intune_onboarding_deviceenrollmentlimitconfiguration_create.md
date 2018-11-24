# <a name="create-deviceenrollmentlimitconfiguration"></a><span data-ttu-id="0dfbd-101">deviceEnrollmentLimitConfiguration の作成</span><span class="sxs-lookup"><span data-stu-id="0dfbd-101">Create deviceEnrollmentLimitConfiguration</span></span>

> <span data-ttu-id="0dfbd-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="0dfbd-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0dfbd-103">新しい [deviceEnrollmentLimitConfiguration](../resources/intune_onboarding_deviceenrollmentlimitconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="0dfbd-103">Create a new [deviceEnrollmentLimitConfiguration](../resources/intune_onboarding_deviceenrollmentlimitconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0dfbd-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="0dfbd-104">Prerequisites</span></span>
<span data-ttu-id="0dfbd-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0dfbd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="0dfbd-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0dfbd-107">Permission type</span></span>|<span data-ttu-id="0dfbd-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="0dfbd-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0dfbd-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0dfbd-109">Delegated (work or school account)</span></span>|<span data-ttu-id="0dfbd-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0dfbd-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="0dfbd-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0dfbd-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0dfbd-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0dfbd-112">Not supported.</span></span>|
|<span data-ttu-id="0dfbd-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0dfbd-113">Application</span></span>|<span data-ttu-id="0dfbd-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0dfbd-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0dfbd-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0dfbd-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="0dfbd-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0dfbd-116">Request headers</span></span>
|<span data-ttu-id="0dfbd-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0dfbd-117">Header</span></span>|<span data-ttu-id="0dfbd-118">値</span><span class="sxs-lookup"><span data-stu-id="0dfbd-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0dfbd-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="0dfbd-119">Authorization</span></span>|<span data-ttu-id="0dfbd-120">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="0dfbd-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0dfbd-121">Accept</span><span class="sxs-lookup"><span data-stu-id="0dfbd-121">Accept</span></span>|<span data-ttu-id="0dfbd-122">application/json</span><span class="sxs-lookup"><span data-stu-id="0dfbd-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0dfbd-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="0dfbd-123">Request body</span></span>
<span data-ttu-id="0dfbd-124">要求本文で、deviceEnrollmentLimitConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="0dfbd-124">In the request body, supply a JSON representation for the deviceEnrollmentLimitConfiguration object.</span></span>

<span data-ttu-id="0dfbd-125">次の表に、deviceEnrollmentLimitConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="0dfbd-125">The following table shows the properties that are required when you create the deviceEnrollmentLimitConfiguration.</span></span>

|<span data-ttu-id="0dfbd-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0dfbd-126">Property</span></span>|<span data-ttu-id="0dfbd-127">型</span><span class="sxs-lookup"><span data-stu-id="0dfbd-127">Type</span></span>|<span data-ttu-id="0dfbd-128">説明</span><span class="sxs-lookup"><span data-stu-id="0dfbd-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0dfbd-129">id</span><span class="sxs-lookup"><span data-stu-id="0dfbd-129">id</span></span>|<span data-ttu-id="0dfbd-130">String</span><span class="sxs-lookup"><span data-stu-id="0dfbd-130">String</span></span>|<span data-ttu-id="0dfbd-131">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0dfbd-131">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="0dfbd-132">displayName</span><span class="sxs-lookup"><span data-stu-id="0dfbd-132">displayName</span></span>|<span data-ttu-id="0dfbd-133">String</span><span class="sxs-lookup"><span data-stu-id="0dfbd-133">String</span></span>|<span data-ttu-id="0dfbd-134">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0dfbd-134">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="0dfbd-135">description</span><span class="sxs-lookup"><span data-stu-id="0dfbd-135">description</span></span>|<span data-ttu-id="0dfbd-136">String</span><span class="sxs-lookup"><span data-stu-id="0dfbd-136">String</span></span>|<span data-ttu-id="0dfbd-137">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0dfbd-137">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="0dfbd-138">priority</span><span class="sxs-lookup"><span data-stu-id="0dfbd-138">priority</span></span>|<span data-ttu-id="0dfbd-139">Int32</span><span class="sxs-lookup"><span data-stu-id="0dfbd-139">Int32</span></span>|<span data-ttu-id="0dfbd-140">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0dfbd-140">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="0dfbd-141">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0dfbd-141">createdDateTime</span></span>|<span data-ttu-id="0dfbd-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0dfbd-142">DateTimeOffset</span></span>|<span data-ttu-id="0dfbd-143">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0dfbd-143">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="0dfbd-144">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0dfbd-144">lastModifiedDateTime</span></span>|<span data-ttu-id="0dfbd-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0dfbd-145">DateTimeOffset</span></span>|<span data-ttu-id="0dfbd-146">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0dfbd-146">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="0dfbd-147">version</span><span class="sxs-lookup"><span data-stu-id="0dfbd-147">version</span></span>|<span data-ttu-id="0dfbd-148">Int32</span><span class="sxs-lookup"><span data-stu-id="0dfbd-148">Int32</span></span>|<span data-ttu-id="0dfbd-149">まだ文書化されていません。[deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0dfbd-149">Not yet documented Inherited from [deviceEnrollmentConfiguration](../resources/intune_onboarding_deviceenrollmentconfiguration.md)</span></span>|
|<span data-ttu-id="0dfbd-150">limit</span><span class="sxs-lookup"><span data-stu-id="0dfbd-150">limit</span></span>|<span data-ttu-id="0dfbd-151">Int32</span><span class="sxs-lookup"><span data-stu-id="0dfbd-151">Int32</span></span>|<span data-ttu-id="0dfbd-152">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="0dfbd-152">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="0dfbd-153">応答</span><span class="sxs-lookup"><span data-stu-id="0dfbd-153">Response</span></span>
<span data-ttu-id="0dfbd-154">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [deviceEnrollmentLimitConfiguration](../resources/intune_onboarding_deviceenrollmentlimitconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="0dfbd-154">If successful, this method returns a `201 Created` response code and a [deviceEnrollmentLimitConfiguration](../resources/intune_onboarding_deviceenrollmentlimitconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0dfbd-155">例</span><span class="sxs-lookup"><span data-stu-id="0dfbd-155">Example</span></span>
### <a name="request"></a><span data-ttu-id="0dfbd-156">要求</span><span class="sxs-lookup"><span data-stu-id="0dfbd-156">Request</span></span>
<span data-ttu-id="0dfbd-157">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0dfbd-157">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations
Content-type: application/json
Content-length: 205

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentLimitConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "version": 7,
  "limit": 5
}
```

### <a name="response"></a><span data-ttu-id="0dfbd-158">応答</span><span class="sxs-lookup"><span data-stu-id="0dfbd-158">Response</span></span>
<span data-ttu-id="0dfbd-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0dfbd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 377

{
  "@odata.type": "#microsoft.graph.deviceEnrollmentLimitConfiguration",
  "id": "4f8c4e4c-4e4c-4f8c-4c4e-8c4f4c4e8c4f",
  "displayName": "Display Name value",
  "description": "Description value",
  "priority": 8,
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "limit": 5
}
```



