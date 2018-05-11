# <a name="update-iosmanagedappregistration"></a><span data-ttu-id="1105d-101">iosManagedAppRegistration の更新</span><span class="sxs-lookup"><span data-stu-id="1105d-101">Update iosManagedAppRegistration</span></span>

> <span data-ttu-id="1105d-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="1105d-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1105d-103">[iosManagedAppRegistration](../resources/intune_mam_iosmanagedappregistration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="1105d-103">Update the properties of a [iosManagedAppRegistration](../resources/intune_mam_iosmanagedappregistration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1105d-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="1105d-104">Prerequisites</span></span>
<span data-ttu-id="1105d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1105d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1105d-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1105d-107">Permission type</span></span>|<span data-ttu-id="1105d-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="1105d-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1105d-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1105d-109">Delegated (work or school account)</span></span>|<span data-ttu-id="1105d-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1105d-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1105d-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1105d-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1105d-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1105d-112">Not supported.</span></span>|
|<span data-ttu-id="1105d-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1105d-113">Application</span></span>|<span data-ttu-id="1105d-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1105d-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1105d-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1105d-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}
```

## <a name="request-headers"></a><span data-ttu-id="1105d-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1105d-116">Request headers</span></span>
|<span data-ttu-id="1105d-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1105d-117">Header</span></span>|<span data-ttu-id="1105d-118">値</span><span class="sxs-lookup"><span data-stu-id="1105d-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1105d-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="1105d-119">Authorization</span></span>|<span data-ttu-id="1105d-120">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="1105d-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1105d-121">Accept</span><span class="sxs-lookup"><span data-stu-id="1105d-121">Accept</span></span>|<span data-ttu-id="1105d-122">application/json</span><span class="sxs-lookup"><span data-stu-id="1105d-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1105d-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="1105d-123">Request body</span></span>
<span data-ttu-id="1105d-124">要求本文で、[iosManagedAppRegistration](../resources/intune_mam_iosmanagedappregistration.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="1105d-124">In the request body, supply a JSON representation for the [iosManagedAppRegistration](../resources/intune_mam_iosmanagedappregistration.md) object.</span></span>

<span data-ttu-id="1105d-125">次の表に、[iosManagedAppRegistration](../resources/intune_mam_iosmanagedappregistration.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="1105d-125">The following table shows the properties that are required when you create the [iosManagedAppRegistration](../resources/intune_mam_iosmanagedappregistration.md).</span></span>

|<span data-ttu-id="1105d-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1105d-126">Property</span></span>|<span data-ttu-id="1105d-127">型</span><span class="sxs-lookup"><span data-stu-id="1105d-127">Type</span></span>|<span data-ttu-id="1105d-128">説明</span><span class="sxs-lookup"><span data-stu-id="1105d-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1105d-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="1105d-129">createdDateTime</span></span>|<span data-ttu-id="1105d-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1105d-130">DateTimeOffset</span></span>|<span data-ttu-id="1105d-131">作成日時 ([managedAppRegistration](../resources/intune_mam_managedappregistration.md) から継承)。</span><span class="sxs-lookup"><span data-stu-id="1105d-131">Date and time of creation Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="1105d-132">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="1105d-132">lastSyncDateTime</span></span>|<span data-ttu-id="1105d-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="1105d-133">DateTimeOffset</span></span>|<span data-ttu-id="1105d-134">アプリが管理サービスと最後に同期した日時。</span><span class="sxs-lookup"><span data-stu-id="1105d-134">Date and time of last the app synced with management service.</span></span> <span data-ttu-id="1105d-135">[managedAppRegistration](../resources/intune_mam_managedappregistration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1105d-135">Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="1105d-136">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="1105d-136">applicationVersion</span></span>|<span data-ttu-id="1105d-137">String</span><span class="sxs-lookup"><span data-stu-id="1105d-137">String</span></span>|<span data-ttu-id="1105d-138">アプリのバージョン ([managedAppRegistration](../resources/intune_mam_managedappregistration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="1105d-138">App version Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="1105d-139">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="1105d-139">managementSdkVersion</span></span>|<span data-ttu-id="1105d-140">String</span><span class="sxs-lookup"><span data-stu-id="1105d-140">String</span></span>|<span data-ttu-id="1105d-141">アプリ管理 SDK のバージョン ([managedAppRegistration](../resources/intune_mam_managedappregistration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="1105d-141">App management SDK version Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="1105d-142">platformVersion</span><span class="sxs-lookup"><span data-stu-id="1105d-142">platformVersion</span></span>|<span data-ttu-id="1105d-143">String</span><span class="sxs-lookup"><span data-stu-id="1105d-143">String</span></span>|<span data-ttu-id="1105d-144">オペレーティング システムのバージョン ([managedAppRegistration](../resources/intune_mam_managedappregistration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="1105d-144">Operating System version Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="1105d-145">deviceType</span><span class="sxs-lookup"><span data-stu-id="1105d-145">deviceType</span></span>|<span data-ttu-id="1105d-146">String</span><span class="sxs-lookup"><span data-stu-id="1105d-146">String</span></span>|<span data-ttu-id="1105d-147">ホスト デバイスの種類 ([managedAppRegistration](../resources/intune_mam_managedappregistration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="1105d-147">Host device type Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="1105d-148">deviceTag</span><span class="sxs-lookup"><span data-stu-id="1105d-148">deviceTag</span></span>|<span data-ttu-id="1105d-149">String</span><span class="sxs-lookup"><span data-stu-id="1105d-149">String</span></span>|<span data-ttu-id="1105d-150">アプリ管理 SDK が生成したタグで、同じデバイス上にホストされているアプリを関連付けるのに役立ちます。</span><span class="sxs-lookup"><span data-stu-id="1105d-150">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="1105d-151">あらゆる状況においてアプリを関連付けることを保証するものではありません。</span><span class="sxs-lookup"><span data-stu-id="1105d-151">Not guaranteed to relate apps in all conditions.</span></span> <span data-ttu-id="1105d-152">[managedAppRegistration](../resources/intune_mam_managedappregistration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1105d-152">Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="1105d-153">deviceName</span><span class="sxs-lookup"><span data-stu-id="1105d-153">deviceName</span></span>|<span data-ttu-id="1105d-154">String</span><span class="sxs-lookup"><span data-stu-id="1105d-154">String</span></span>|<span data-ttu-id="1105d-155">ホスト デバイスの名前 ([managedAppRegistration](../resources/intune_mam_managedappregistration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="1105d-155">Host device name Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="1105d-156">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="1105d-156">flaggedReasons</span></span>|<span data-ttu-id="1105d-157">String コレクション</span><span class="sxs-lookup"><span data-stu-id="1105d-157">String collection</span></span>|<span data-ttu-id="1105d-158">アプリ登録にフラグが付けられた、0 個以上の理由です。</span><span class="sxs-lookup"><span data-stu-id="1105d-158">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="1105d-159">例: </span><span class="sxs-lookup"><span data-stu-id="1105d-159">E.g.</span></span> <span data-ttu-id="1105d-160">[managedAppRegistration](../resources/intune_mam_managedappregistration.md) から継承された、ルート化されたデバイス上で実行されているアプリ。可能な値は、`none`、`rootedDevice` です。</span><span class="sxs-lookup"><span data-stu-id="1105d-160">app running on rooted device Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md) Possible values are: `none`, `rootedDevice`.</span></span>|
|<span data-ttu-id="1105d-161">userId</span><span class="sxs-lookup"><span data-stu-id="1105d-161">userId</span></span>|<span data-ttu-id="1105d-162">String</span><span class="sxs-lookup"><span data-stu-id="1105d-162">String</span></span>|<span data-ttu-id="1105d-163">このアプリ登録が所属するユーザー ID。</span><span class="sxs-lookup"><span data-stu-id="1105d-163">The user Id to who this app registration belongs.</span></span> <span data-ttu-id="1105d-164">[managedAppRegistration](../resources/intune_mam_managedappregistration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1105d-164">Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="1105d-165">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="1105d-165">appIdentifier</span></span>|[<span data-ttu-id="1105d-166">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="1105d-166">mobileAppIdentifier</span></span>](../resources/intune_mam_mobileappidentifier.md)|<span data-ttu-id="1105d-167">アプリ パッケージの識別子 ([managedAppRegistration](../resources/intune_mam_managedappregistration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="1105d-167">The app package Identifier Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="1105d-168">id</span><span class="sxs-lookup"><span data-stu-id="1105d-168">id</span></span>|<span data-ttu-id="1105d-169">String</span><span class="sxs-lookup"><span data-stu-id="1105d-169">String</span></span>|<span data-ttu-id="1105d-170">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="1105d-170">Key of the entity.</span></span> <span data-ttu-id="1105d-171">[managedAppRegistration](../resources/intune_mam_managedappregistration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1105d-171">Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="1105d-172">version</span><span class="sxs-lookup"><span data-stu-id="1105d-172">version</span></span>|<span data-ttu-id="1105d-173">String</span><span class="sxs-lookup"><span data-stu-id="1105d-173">String</span></span>|<span data-ttu-id="1105d-174">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="1105d-174">Version of the entity.</span></span> <span data-ttu-id="1105d-175">[managedAppRegistration](../resources/intune_mam_managedappregistration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1105d-175">Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="1105d-176">応答</span><span class="sxs-lookup"><span data-stu-id="1105d-176">Response</span></span>
<span data-ttu-id="1105d-177">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [iosManagedAppRegistration](../resources/intune_mam_iosmanagedappregistration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="1105d-177">If successful, this method returns a `200 OK` response code and an updated [iosManagedAppRegistration](../resources/intune_mam_iosmanagedappregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1105d-178">例</span><span class="sxs-lookup"><span data-stu-id="1105d-178">Example</span></span>
### <a name="request"></a><span data-ttu-id="1105d-179">要求</span><span class="sxs-lookup"><span data-stu-id="1105d-179">Request</span></span>
<span data-ttu-id="1105d-180">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1105d-180">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}
Content-type: application/json
Content-length: 571

{
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

### <a name="response"></a><span data-ttu-id="1105d-181">応答</span><span class="sxs-lookup"><span data-stu-id="1105d-181">Response</span></span>
<span data-ttu-id="1105d-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1105d-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



