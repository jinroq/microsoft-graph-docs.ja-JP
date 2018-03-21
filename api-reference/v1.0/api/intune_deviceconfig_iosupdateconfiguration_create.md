# <a name="create-iosupdateconfiguration"></a><span data-ttu-id="a3345-101">iosUpdateConfiguration の作成</span><span class="sxs-lookup"><span data-stu-id="a3345-101">Create iosUpdateConfiguration</span></span>

> <span data-ttu-id="a3345-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="a3345-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a3345-103">新しい [iosUpdateConfiguration](../resources/intune_deviceconfig_iosupdateconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="a3345-103">Create a new [plannerBucket](../resources/intune_deviceconfig_iosupdateconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a3345-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="a3345-104">Prerequisites</span></span>
<span data-ttu-id="a3345-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a3345-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="a3345-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a3345-107">Permission type</span></span>|<span data-ttu-id="a3345-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a3345-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a3345-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a3345-109">Delegated (work or school account)</span></span>|<span data-ttu-id="a3345-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3345-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a3345-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a3345-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a3345-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a3345-112">Not supported.</span></span>|
|<span data-ttu-id="a3345-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a3345-113">Application</span></span>|<span data-ttu-id="a3345-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a3345-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a3345-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a3345-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="a3345-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a3345-116">Request headers</span></span>
|<span data-ttu-id="a3345-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a3345-117">Header</span></span>|<span data-ttu-id="a3345-118">値</span><span class="sxs-lookup"><span data-stu-id="a3345-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a3345-119">承認</span><span class="sxs-lookup"><span data-stu-id="a3345-119">Authorization</span></span>|<span data-ttu-id="a3345-120">ベアラー &lt;トークン&gt;が必須。</span><span class="sxs-lookup"><span data-stu-id="a3345-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="a3345-121">承諾</span><span class="sxs-lookup"><span data-stu-id="a3345-121">Accept</span></span>|<span data-ttu-id="a3345-122">application/json</span><span class="sxs-lookup"><span data-stu-id="a3345-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a3345-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="a3345-123">Request body</span></span>
<span data-ttu-id="a3345-124">要求本文で、iosUpdateConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="a3345-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="a3345-125">次の表に、iosUpdateConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="a3345-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="a3345-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a3345-126">Property</span></span>|<span data-ttu-id="a3345-127">型</span><span class="sxs-lookup"><span data-stu-id="a3345-127">Type</span></span>|<span data-ttu-id="a3345-128">説明</span><span class="sxs-lookup"><span data-stu-id="a3345-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a3345-129">id</span><span class="sxs-lookup"><span data-stu-id="a3345-129">id</span></span>|<span data-ttu-id="a3345-130">String</span><span class="sxs-lookup"><span data-stu-id="a3345-130">String</span></span>|<span data-ttu-id="a3345-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="a3345-131">Name of the entity.</span></span> <span data-ttu-id="a3345-132">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a3345-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a3345-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a3345-133">lastModifiedDateTime</span></span>|<span data-ttu-id="a3345-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a3345-134">DateTimeOffset</span></span>|<span data-ttu-id="a3345-135">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="a3345-135">Gets or sets a DateTime value specifying when the node object was last modified.</span></span> <span data-ttu-id="a3345-136">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a3345-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a3345-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a3345-137">createdDateTime</span></span>|<span data-ttu-id="a3345-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a3345-138">DateTimeOffset</span></span>|<span data-ttu-id="a3345-139">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="a3345-139">DateTime the object was created.</span></span> <span data-ttu-id="a3345-140">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a3345-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a3345-141">description</span><span class="sxs-lookup"><span data-stu-id="a3345-141">description</span></span>|<span data-ttu-id="a3345-142">String</span><span class="sxs-lookup"><span data-stu-id="a3345-142">String</span></span>|<span data-ttu-id="a3345-143">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="a3345-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a3345-144">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a3345-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a3345-145">displayName</span><span class="sxs-lookup"><span data-stu-id="a3345-145">displayName</span></span>|<span data-ttu-id="a3345-146">String</span><span class="sxs-lookup"><span data-stu-id="a3345-146">String</span></span>|<span data-ttu-id="a3345-147">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="a3345-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a3345-148">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a3345-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a3345-149">version</span><span class="sxs-lookup"><span data-stu-id="a3345-149">version</span></span>|<span data-ttu-id="a3345-150">Int32</span><span class="sxs-lookup"><span data-stu-id="a3345-150">Int32</span></span>|<span data-ttu-id="a3345-151">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="a3345-151">Version of the device configuration.</span></span> <span data-ttu-id="a3345-152">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="a3345-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a3345-153">activeHoursStart</span><span class="sxs-lookup"><span data-stu-id="a3345-153">activeHoursStart</span></span>|<span data-ttu-id="a3345-154">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="a3345-154">TimeOfDay</span></span>|<span data-ttu-id="a3345-155">アクティブ時間の開始 (アクティブ時間は、更新のインストールが実施されない時間枠のことです)</span><span class="sxs-lookup"><span data-stu-id="a3345-155">Active Hours Start (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="a3345-156">activeHoursEnd</span><span class="sxs-lookup"><span data-stu-id="a3345-156">activeHoursEnd</span></span>|<span data-ttu-id="a3345-157">TimeOfDay</span><span class="sxs-lookup"><span data-stu-id="a3345-157">TimeOfDay</span></span>|<span data-ttu-id="a3345-158">アクティブ時間の終了 (アクティブ時間は、更新のインストールが実施されない時間枠のことです)</span><span class="sxs-lookup"><span data-stu-id="a3345-158">Active Hours End (active hours mean the time window when updates install should not happen)</span></span>|
|<span data-ttu-id="a3345-159">scheduledInstallDays</span><span class="sxs-lookup"><span data-stu-id="a3345-159">scheduledInstallDays</span></span>|<span data-ttu-id="a3345-160">String コレクション</span><span class="sxs-lookup"><span data-stu-id="a3345-160">String collection</span></span>|<span data-ttu-id="a3345-161">アクティブ時間が設定されている曜日。</span><span class="sxs-lookup"><span data-stu-id="a3345-161">Days in week for which active hours are configured.</span></span> <span data-ttu-id="a3345-162">このコレクションには、最大で 7 個の要素を含めることができます。</span><span class="sxs-lookup"><span data-stu-id="a3345-162">This collection can contain a maximum of 7 elements.</span></span> <span data-ttu-id="a3345-163">可能な値は、`sunday`、`monday`、`tuesday`、`wednesday`、`thursday`、`friday`、`saturday` です。</span><span class="sxs-lookup"><span data-stu-id="a3345-163">Possible values are: `sunday`, `monday`, `tuesday`, `wednesday`, `thursday`, `friday`, `saturday`.</span></span>|
|<span data-ttu-id="a3345-164">utcTimeOffsetInMinutes</span><span class="sxs-lookup"><span data-stu-id="a3345-164">utcTimeOffsetInMinutes</span></span>|<span data-ttu-id="a3345-165">Int32</span><span class="sxs-lookup"><span data-stu-id="a3345-165">Int32</span></span>|<span data-ttu-id="a3345-166">UTC タイム オフセット (分単位で示されます)</span><span class="sxs-lookup"><span data-stu-id="a3345-166">UTC Time Offset indicated in minutes</span></span>|



## <a name="response"></a><span data-ttu-id="a3345-167">応答</span><span class="sxs-lookup"><span data-stu-id="a3345-167">Response</span></span>
<span data-ttu-id="a3345-168">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [iosUpdateConfiguration](../resources/intune_deviceconfig_iosupdateconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a3345-168">If successful, this method returns a `201 Created` response code and a [section](../resources/intune_deviceconfig_iosupdateconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a3345-169">例</span><span class="sxs-lookup"><span data-stu-id="a3345-169">Example</span></span>
### <a name="request"></a><span data-ttu-id="a3345-170">要求</span><span class="sxs-lookup"><span data-stu-id="a3345-170">Request</span></span>
<span data-ttu-id="a3345-171">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a3345-171">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 389

{
  "@odata.type": "#microsoft.graph.iosUpdateConfiguration",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "activeHoursStart": "12:00:05.5020000",
  "activeHoursEnd": "11:59:00.8990000",
  "scheduledInstallDays": [
    "monday"
  ],
  "utcTimeOffsetInMinutes": 6
}
```

### <a name="response"></a><span data-ttu-id="a3345-172">応答</span><span class="sxs-lookup"><span data-stu-id="a3345-172">Response</span></span>
<span data-ttu-id="a3345-p109">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a3345-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 497

{
  "@odata.type": "#microsoft.graph.iosUpdateConfiguration",
  "id": "321aef09-ef09-321a-09ef-1a3209ef1a32",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "activeHoursStart": "12:00:05.5020000",
  "activeHoursEnd": "11:59:00.8990000",
  "scheduledInstallDays": [
    "monday"
  ],
  "utcTimeOffsetInMinutes": 6
}
```



