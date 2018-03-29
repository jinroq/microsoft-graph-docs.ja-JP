# <a name="create-iosmanagedappregistration"></a><span data-ttu-id="d36f3-101">Create iosManagedAppRegistration</span><span class="sxs-lookup"><span data-stu-id="d36f3-101">Create iosManagedAppRegistration</span></span>

> <span data-ttu-id="d36f3-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="d36f3-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d36f3-103">新しい [iosManagedAppRegistration](../resources/intune_mam_iosmanagedappregistration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="d36f3-103">Create a new [plannerBucket](../resources/intune_mam_iosmanagedappregistration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d36f3-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="d36f3-104">Prerequisites</span></span>
<span data-ttu-id="d36f3-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d36f3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="d36f3-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d36f3-107">Permission type</span></span>|<span data-ttu-id="d36f3-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="d36f3-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d36f3-109">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="d36f3-109">Delegated (work or school account)</span></span>|<span data-ttu-id="d36f3-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d36f3-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d36f3-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d36f3-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d36f3-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d36f3-112">Not supported.</span></span>|
|<span data-ttu-id="d36f3-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d36f3-113">Application</span></span>|<span data-ttu-id="d36f3-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d36f3-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d36f3-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d36f3-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppRegistrations
```

## <a name="request-headers"></a><span data-ttu-id="d36f3-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d36f3-116">Request headers</span></span>
|<span data-ttu-id="d36f3-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d36f3-117">Header</span></span>|<span data-ttu-id="d36f3-118">値</span><span class="sxs-lookup"><span data-stu-id="d36f3-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d36f3-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="d36f3-119">Authorization</span></span>|<span data-ttu-id="d36f3-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="d36f3-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="d36f3-121">Accept</span><span class="sxs-lookup"><span data-stu-id="d36f3-121">Accept</span></span>|<span data-ttu-id="d36f3-122">application/json</span><span class="sxs-lookup"><span data-stu-id="d36f3-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d36f3-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="d36f3-123">Request body</span></span>
<span data-ttu-id="d36f3-124">要求本文で、iosManagedAppRegistration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="d36f3-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="d36f3-125">次の表に、iosManagedAppRegistration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="d36f3-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="d36f3-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d36f3-126">Property</span></span>|<span data-ttu-id="d36f3-127">型</span><span class="sxs-lookup"><span data-stu-id="d36f3-127">Type</span></span>|<span data-ttu-id="d36f3-128">説明</span><span class="sxs-lookup"><span data-stu-id="d36f3-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d36f3-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d36f3-129">createdDateTime</span></span>|<span data-ttu-id="d36f3-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d36f3-130">DateTimeOffset</span></span>|<span data-ttu-id="d36f3-131">[managedAppRegistration](../resources/intune_mam_managedappregistration.md) から継承した作成日時。</span><span class="sxs-lookup"><span data-stu-id="d36f3-131">Date and time of creation Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="d36f3-132">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="d36f3-132">lastSyncDateTime</span></span>|<span data-ttu-id="d36f3-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d36f3-133">DateTimeOffset</span></span>|<span data-ttu-id="d36f3-134">アプリが管理サービスと最後に同期した日時。</span><span class="sxs-lookup"><span data-stu-id="d36f3-134">Date and time of last the app synced with management service.</span></span> <span data-ttu-id="d36f3-135">[managedAppRegistration](../resources/intune_mam_managedappregistration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d36f3-135">Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="d36f3-136">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="d36f3-136">applicationVersion</span></span>|<span data-ttu-id="d36f3-137">String</span><span class="sxs-lookup"><span data-stu-id="d36f3-137">String</span></span>|<span data-ttu-id="d36f3-138">[managedAppRegistration](../resources/intune_mam_managedappregistration.md) から継承したアプリのバージョン</span><span class="sxs-lookup"><span data-stu-id="d36f3-138">App version Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="d36f3-139">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="d36f3-139">managementSdkVersion</span></span>|<span data-ttu-id="d36f3-140">String</span><span class="sxs-lookup"><span data-stu-id="d36f3-140">String</span></span>|<span data-ttu-id="d36f3-141">[managedAppRegistration](../resources/intune_mam_managedappregistration.md) から継承したアプリ管理 SDK のバージョン</span><span class="sxs-lookup"><span data-stu-id="d36f3-141">App management SDK version Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="d36f3-142">platformVersion</span><span class="sxs-lookup"><span data-stu-id="d36f3-142">platformVersion</span></span>|<span data-ttu-id="d36f3-143">String</span><span class="sxs-lookup"><span data-stu-id="d36f3-143">String</span></span>|<span data-ttu-id="d36f3-144">[managedAppRegistration](../resources/intune_mam_managedappregistration.md) から継承したオペレーティング システムのバージョン</span><span class="sxs-lookup"><span data-stu-id="d36f3-144">Operating System version Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="d36f3-145">deviceType</span><span class="sxs-lookup"><span data-stu-id="d36f3-145">DeviceType</span></span>|<span data-ttu-id="d36f3-146">String</span><span class="sxs-lookup"><span data-stu-id="d36f3-146">String</span></span>|<span data-ttu-id="d36f3-147">[managedAppRegistration](../resources/intune_mam_managedappregistration.md) から継承したホスト デバイスの種類</span><span class="sxs-lookup"><span data-stu-id="d36f3-147">Host device type Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="d36f3-148">deviceTag</span><span class="sxs-lookup"><span data-stu-id="d36f3-148">deviceTag</span></span>|<span data-ttu-id="d36f3-149">String</span><span class="sxs-lookup"><span data-stu-id="d36f3-149">String</span></span>|<span data-ttu-id="d36f3-150">アプリ管理 SDK が生成したタグで、同じデバイス上にホストされているアプリを関連付けるのに役立ちます。</span><span class="sxs-lookup"><span data-stu-id="d36f3-150">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="d36f3-151">あらゆる状況においてアプリを関連付けることを保証するものではありません。</span><span class="sxs-lookup"><span data-stu-id="d36f3-151">Not guaranteed to relate apps in all conditions.</span></span> <span data-ttu-id="d36f3-152">[managedAppRegistration](../resources/intune_mam_managedappregistration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d36f3-152">Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="d36f3-153">deviceName</span><span class="sxs-lookup"><span data-stu-id="d36f3-153">DeviceName</span></span>|<span data-ttu-id="d36f3-154">String</span><span class="sxs-lookup"><span data-stu-id="d36f3-154">String</span></span>|<span data-ttu-id="d36f3-155">[managedAppRegistration](../resources/intune_mam_managedappregistration.md) から継承したホスト デバイス名</span><span class="sxs-lookup"><span data-stu-id="d36f3-155">Host device name Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="d36f3-156">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="d36f3-156">flaggedReasons</span></span>|<span data-ttu-id="d36f3-157">String コレクション</span><span class="sxs-lookup"><span data-stu-id="d36f3-157">String collection</span></span>|<span data-ttu-id="d36f3-158">アプリ登録にフラグが付けられた、0 個以上の理由です。</span><span class="sxs-lookup"><span data-stu-id="d36f3-158">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="d36f3-159">例: </span><span class="sxs-lookup"><span data-stu-id="d36f3-159">E.g.</span></span> <span data-ttu-id="d36f3-160">[managedAppRegistration](../resources/intune_mam_managedappregistration.md) から継承された、ルート化されたデバイス上で実行されているアプリ。可能な値は、`none`、`rootedDevice` です。</span><span class="sxs-lookup"><span data-stu-id="d36f3-160">app running on rooted device Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md) Possible values are: `none`, `rootedDevice`.</span></span>|
|<span data-ttu-id="d36f3-161">userId</span><span class="sxs-lookup"><span data-stu-id="d36f3-161">userId</span></span>|<span data-ttu-id="d36f3-162">String</span><span class="sxs-lookup"><span data-stu-id="d36f3-162">String</span></span>|<span data-ttu-id="d36f3-163">このアプリ登録が所属するユーザー ID。</span><span class="sxs-lookup"><span data-stu-id="d36f3-163">The user Id to who this app registration belongs.</span></span> <span data-ttu-id="d36f3-164">[managedAppRegistration](../resources/intune_mam_managedappregistration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d36f3-164">Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="d36f3-165">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="d36f3-165">appIdentifier</span></span>|[<span data-ttu-id="d36f3-166">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="d36f3-166">mobileAppIdentifier</span></span>](../resources/intune_mam_mobileappidentifier.md)|<span data-ttu-id="d36f3-167">[managedAppRegistration](../resources/intune_mam_managedappregistration.md) から継承したアプリ パッケージ識別子</span><span class="sxs-lookup"><span data-stu-id="d36f3-167">The app package Identifier Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="d36f3-168">id</span><span class="sxs-lookup"><span data-stu-id="d36f3-168">id</span></span>|<span data-ttu-id="d36f3-169">String</span><span class="sxs-lookup"><span data-stu-id="d36f3-169">String</span></span>|<span data-ttu-id="d36f3-170">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="d36f3-170">Name of the entity.</span></span> <span data-ttu-id="d36f3-171">[managedAppRegistration](../resources/intune_mam_managedappregistration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d36f3-171">Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="d36f3-172">version</span><span class="sxs-lookup"><span data-stu-id="d36f3-172">version</span></span>|<span data-ttu-id="d36f3-173">String</span><span class="sxs-lookup"><span data-stu-id="d36f3-173">String</span></span>|<span data-ttu-id="d36f3-174">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="d36f3-174">Version of the entity.</span></span> <span data-ttu-id="d36f3-175">[managedAppRegistration](../resources/intune_mam_managedappregistration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="d36f3-175">Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="d36f3-176">応答</span><span class="sxs-lookup"><span data-stu-id="d36f3-176">Response</span></span>
<span data-ttu-id="d36f3-177">このメソッドが成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [iosManagedAppRegistration](../resources/intune_mam_iosmanagedappregistration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d36f3-177">If successful, this method returns a `201 Created` response code and a [section](../resources/intune_mam_iosmanagedappregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d36f3-178">例</span><span class="sxs-lookup"><span data-stu-id="d36f3-178">Example</span></span>
### <a name="request"></a><span data-ttu-id="d36f3-179">要求</span><span class="sxs-lookup"><span data-stu-id="d36f3-179">Request</span></span>
<span data-ttu-id="d36f3-180">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d36f3-180">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppRegistrations
Content-type: application/json
Content-length: 635

{
  "@odata.type": "#microsoft.graph.iosManagedAppRegistration",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "applicationVersion": "Application Version value",
  "managementSdkVersion": "Management Sdk Version value",
  "platformVersion": "Platform Version value",
  "deviceType": "Device Type value",
  "deviceTag": "Device Tag value",
  "deviceName": "Device Name value",
  "flaggedReasons": [
    "rootedDevice"
  ],
  "userId": "User Id value",
  "appIdentifier": {
    "@odata.type": "microsoft.graph.iosMobileAppIdentifier",
    "bundleId": "Bundle Id value"
  },
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="d36f3-181">応答</span><span class="sxs-lookup"><span data-stu-id="d36f3-181">Response</span></span>
<span data-ttu-id="d36f3-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d36f3-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 743

{
  "@odata.type": "#microsoft.graph.iosManagedAppRegistration",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "applicationVersion": "Application Version value",
  "managementSdkVersion": "Management Sdk Version value",
  "platformVersion": "Platform Version value",
  "deviceType": "Device Type value",
  "deviceTag": "Device Tag value",
  "deviceName": "Device Name value",
  "flaggedReasons": [
    "rootedDevice"
  ],
  "userId": "User Id value",
  "appIdentifier": {
    "@odata.type": "microsoft.graph.iosMobileAppIdentifier",
    "bundleId": "Bundle Id value"
  },
  "id": "47632c19-2c19-4763-192c-6347192c6347",
  "version": "Version value"
}
```



