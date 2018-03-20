# <a name="update-androidmanagedappregistration"></a><span data-ttu-id="19c3e-101">androidManagedAppRegistration の更新</span><span class="sxs-lookup"><span data-stu-id="19c3e-101">Update androidManagedAppRegistration</span></span>

> <span data-ttu-id="19c3e-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="19c3e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="19c3e-103">[androidManagedAppRegistration](../resources/intune_mam_androidmanagedappregistration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="19c3e-103">Update the properties of a [calendar](../resources/intune_mam_androidmanagedappregistration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="19c3e-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="19c3e-104">Prerequisites</span></span>
<span data-ttu-id="19c3e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="19c3e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="19c3e-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="19c3e-107">Permission type</span></span>|<span data-ttu-id="19c3e-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="19c3e-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="19c3e-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="19c3e-109">Delegated (work or school account)</span></span>|<span data-ttu-id="19c3e-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19c3e-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="19c3e-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="19c3e-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="19c3e-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="19c3e-112">Not supported.</span></span>|
|<span data-ttu-id="19c3e-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="19c3e-113">Application</span></span>|<span data-ttu-id="19c3e-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="19c3e-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="19c3e-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="19c3e-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}
```

## <a name="request-headers"></a><span data-ttu-id="19c3e-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="19c3e-116">Request headers</span></span>
|<span data-ttu-id="19c3e-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="19c3e-117">Header</span></span>|<span data-ttu-id="19c3e-118">値</span><span class="sxs-lookup"><span data-stu-id="19c3e-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="19c3e-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="19c3e-119">Authorization</span></span>|<span data-ttu-id="19c3e-120">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="19c3e-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="19c3e-121">Accept</span><span class="sxs-lookup"><span data-stu-id="19c3e-121">Accept</span></span>|<span data-ttu-id="19c3e-122">application/json</span><span class="sxs-lookup"><span data-stu-id="19c3e-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="19c3e-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="19c3e-123">Request body</span></span>
<span data-ttu-id="19c3e-124">要求本文で、[androidManagedAppRegistration](../resources/intune_mam_androidmanagedappregistration.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="19c3e-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_mam_androidmanagedappregistration.md) object.</span></span>

<span data-ttu-id="19c3e-125">次の表に、[androidManagedAppRegistration](../resources/intune_mam_androidmanagedappregistration.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="19c3e-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="19c3e-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="19c3e-126">Property</span></span>|<span data-ttu-id="19c3e-127">型</span><span class="sxs-lookup"><span data-stu-id="19c3e-127">Type</span></span>|<span data-ttu-id="19c3e-128">説明</span><span class="sxs-lookup"><span data-stu-id="19c3e-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19c3e-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="19c3e-129">createdDateTime</span></span>|<span data-ttu-id="19c3e-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="19c3e-130">DateTimeOffset</span></span>|<span data-ttu-id="19c3e-131">作成日時 ([managedAppRegistration](../resources/intune_mam_managedappregistration.md) から継承)。</span><span class="sxs-lookup"><span data-stu-id="19c3e-131">Date and time of creation Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="19c3e-132">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="19c3e-132">lastSyncDateTime</span></span>|<span data-ttu-id="19c3e-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="19c3e-133">DateTimeOffset</span></span>|<span data-ttu-id="19c3e-134">アプリが管理サービスと最後に同期した日時。</span><span class="sxs-lookup"><span data-stu-id="19c3e-134">Date and time of last the app synced with management service.</span></span> <span data-ttu-id="19c3e-135">[managedAppRegistration](../resources/intune_mam_managedappregistration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="19c3e-135">Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="19c3e-136">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="19c3e-136">applicationVersion</span></span>|<span data-ttu-id="19c3e-137">String</span><span class="sxs-lookup"><span data-stu-id="19c3e-137">String</span></span>|<span data-ttu-id="19c3e-138">アプリのバージョン ([managedAppRegistration](../resources/intune_mam_managedappregistration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="19c3e-138">App version Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="19c3e-139">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="19c3e-139">managementSdkVersion</span></span>|<span data-ttu-id="19c3e-140">String</span><span class="sxs-lookup"><span data-stu-id="19c3e-140">String</span></span>|<span data-ttu-id="19c3e-141">アプリ管理 SDK のバージョン ([managedAppRegistration](../resources/intune_mam_managedappregistration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="19c3e-141">App management SDK version Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="19c3e-142">platformVersion</span><span class="sxs-lookup"><span data-stu-id="19c3e-142">platformVersion</span></span>|<span data-ttu-id="19c3e-143">String</span><span class="sxs-lookup"><span data-stu-id="19c3e-143">String</span></span>|<span data-ttu-id="19c3e-144">オペレーティング システムのバージョン ([managedAppRegistration](../resources/intune_mam_managedappregistration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="19c3e-144">Operating System version Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="19c3e-145">deviceType</span><span class="sxs-lookup"><span data-stu-id="19c3e-145">DeviceType</span></span>|<span data-ttu-id="19c3e-146">String</span><span class="sxs-lookup"><span data-stu-id="19c3e-146">String</span></span>|<span data-ttu-id="19c3e-147">ホスト デバイスの種類 ([managedAppRegistration](../resources/intune_mam_managedappregistration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="19c3e-147">Host device type Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="19c3e-148">deviceTag</span><span class="sxs-lookup"><span data-stu-id="19c3e-148">deviceTag</span></span>|<span data-ttu-id="19c3e-149">String</span><span class="sxs-lookup"><span data-stu-id="19c3e-149">String</span></span>|<span data-ttu-id="19c3e-150">アプリ管理 SDK が生成したタグ。同じデバイスでホストされているアプリの関連付けに役立ちます。</span><span class="sxs-lookup"><span data-stu-id="19c3e-150">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="19c3e-151">あらゆる状況でのアプリの関連付けを保証するものではありません。</span><span class="sxs-lookup"><span data-stu-id="19c3e-151">Not guaranteed to relate apps in all conditions.</span></span> <span data-ttu-id="19c3e-152">[managedAppRegistration](../resources/intune_mam_managedappregistration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="19c3e-152">Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="19c3e-153">deviceName</span><span class="sxs-lookup"><span data-stu-id="19c3e-153">DeviceName</span></span>|<span data-ttu-id="19c3e-154">String</span><span class="sxs-lookup"><span data-stu-id="19c3e-154">String</span></span>|<span data-ttu-id="19c3e-155">ホスト デバイスの名前 ([managedAppRegistration](../resources/intune_mam_managedappregistration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="19c3e-155">Host device name Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="19c3e-156">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="19c3e-156">flaggedReasons</span></span>|<span data-ttu-id="19c3e-157">String コレクション</span><span class="sxs-lookup"><span data-stu-id="19c3e-157">String collection</span></span>|<span data-ttu-id="19c3e-158">アプリ登録にフラグが設定された、0 個以上の理由。</span><span class="sxs-lookup"><span data-stu-id="19c3e-158">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="19c3e-159">例: </span><span class="sxs-lookup"><span data-stu-id="19c3e-159">E.g.</span></span> <span data-ttu-id="19c3e-160">ルートのデバイスで実行されているアプリ。[managedAppRegistration](../resources/intune_mam_managedappregistration.md) から継承します。可能な値は、`none`、`rootedDevice` です。</span><span class="sxs-lookup"><span data-stu-id="19c3e-160">app running on rooted device Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md) Possible values are: `none`, `rootedDevice`.</span></span>|
|<span data-ttu-id="19c3e-161">userId</span><span class="sxs-lookup"><span data-stu-id="19c3e-161">userId</span></span>|<span data-ttu-id="19c3e-162">String</span><span class="sxs-lookup"><span data-stu-id="19c3e-162">String</span></span>|<span data-ttu-id="19c3e-163">このアプリの登録が属するユーザー ID。</span><span class="sxs-lookup"><span data-stu-id="19c3e-163">The user Id to who this app registration belongs.</span></span> <span data-ttu-id="19c3e-164">[managedAppRegistration](../resources/intune_mam_managedappregistration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="19c3e-164">Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="19c3e-165">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="19c3e-165">appIdentifier</span></span>|[<span data-ttu-id="19c3e-166">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="19c3e-166">mobileAppIdentifier</span></span>](../resources/intune_mam_mobileappidentifier.md)|<span data-ttu-id="19c3e-167">アプリ パッケージの識別子 ([managedAppRegistration](../resources/intune_mam_managedappregistration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="19c3e-167">The app package Identifier Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="19c3e-168">id</span><span class="sxs-lookup"><span data-stu-id="19c3e-168">id</span></span>|<span data-ttu-id="19c3e-169">String</span><span class="sxs-lookup"><span data-stu-id="19c3e-169">String</span></span>|<span data-ttu-id="19c3e-170">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="19c3e-170">Name of the entity.</span></span> <span data-ttu-id="19c3e-171">[managedAppRegistration](../resources/intune_mam_managedappregistration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="19c3e-171">Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="19c3e-172">version</span><span class="sxs-lookup"><span data-stu-id="19c3e-172">version</span></span>|<span data-ttu-id="19c3e-173">String</span><span class="sxs-lookup"><span data-stu-id="19c3e-173">String</span></span>|<span data-ttu-id="19c3e-174">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="19c3e-174">Version of the entity.</span></span> <span data-ttu-id="19c3e-175">[managedAppRegistration](../resources/intune_mam_managedappregistration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="19c3e-175">Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="19c3e-176">応答</span><span class="sxs-lookup"><span data-stu-id="19c3e-176">Response</span></span>
<span data-ttu-id="19c3e-177">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [androidManagedAppRegistration](../resources/intune_mam_androidmanagedappregistration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="19c3e-177">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_mam_androidmanagedappregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="19c3e-178">例</span><span class="sxs-lookup"><span data-stu-id="19c3e-178">Example</span></span>
### <a name="request"></a><span data-ttu-id="19c3e-179">要求</span><span class="sxs-lookup"><span data-stu-id="19c3e-179">Request</span></span>
<span data-ttu-id="19c3e-180">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="19c3e-180">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}
Content-type: application/json
Content-length: 577

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
    "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
    "packageId": "Package Id value"
  },
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="19c3e-181">応答</span><span class="sxs-lookup"><span data-stu-id="19c3e-181">Response</span></span>
<span data-ttu-id="19c3e-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="19c3e-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 753

{
  "@odata.type": "#microsoft.graph.androidManagedAppRegistration",
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
    "@odata.type": "microsoft.graph.androidMobileAppIdentifier",
    "packageId": "Package Id value"
  },
  "id": "0e064997-4997-0e06-9749-060e9749060e",
  "version": "Version value"
}
```



