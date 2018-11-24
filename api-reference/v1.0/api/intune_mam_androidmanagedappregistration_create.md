# <a name="create-androidmanagedappregistration"></a><span data-ttu-id="013c5-101">androidManagedAppRegistration の作成</span><span class="sxs-lookup"><span data-stu-id="013c5-101">Create androidManagedAppRegistration</span></span>

> <span data-ttu-id="013c5-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="013c5-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="013c5-103">新しい [androidManagedAppRegistration](../resources/intune_mam_androidmanagedappregistration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="013c5-103">Create a new [androidManagedAppRegistration](../resources/intune_mam_androidmanagedappregistration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="013c5-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="013c5-104">Prerequisites</span></span>
<span data-ttu-id="013c5-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="013c5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="013c5-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="013c5-107">Permission type</span></span>|<span data-ttu-id="013c5-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="013c5-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="013c5-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="013c5-109">Delegated (work or school account)</span></span>|<span data-ttu-id="013c5-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="013c5-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="013c5-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="013c5-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="013c5-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="013c5-112">Not supported.</span></span>|
|<span data-ttu-id="013c5-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="013c5-113">Application</span></span>|<span data-ttu-id="013c5-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="013c5-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="013c5-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="013c5-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppRegistrations
```

## <a name="request-headers"></a><span data-ttu-id="013c5-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="013c5-116">Request headers</span></span>
|<span data-ttu-id="013c5-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="013c5-117">Header</span></span>|<span data-ttu-id="013c5-118">値</span><span class="sxs-lookup"><span data-stu-id="013c5-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="013c5-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="013c5-119">Authorization</span></span>|<span data-ttu-id="013c5-120">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="013c5-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="013c5-121">Accept</span><span class="sxs-lookup"><span data-stu-id="013c5-121">Accept</span></span>|<span data-ttu-id="013c5-122">application/json</span><span class="sxs-lookup"><span data-stu-id="013c5-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="013c5-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="013c5-123">Request body</span></span>
<span data-ttu-id="013c5-124">要求本文で、androidManagedAppRegistration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="013c5-124">In the request body, supply a JSON representation for the androidManagedAppRegistration object.</span></span>

<span data-ttu-id="013c5-125">次の表に、androidManagedAppRegistration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="013c5-125">The following table shows the properties that are required when you create the androidManagedAppRegistration.</span></span>

|<span data-ttu-id="013c5-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="013c5-126">Property</span></span>|<span data-ttu-id="013c5-127">型</span><span class="sxs-lookup"><span data-stu-id="013c5-127">Type</span></span>|<span data-ttu-id="013c5-128">説明</span><span class="sxs-lookup"><span data-stu-id="013c5-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="013c5-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="013c5-129">createdDateTime</span></span>|<span data-ttu-id="013c5-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="013c5-130">DateTimeOffset</span></span>|<span data-ttu-id="013c5-131">作成日時 ([managedAppRegistration](../resources/intune_mam_managedappregistration.md) から継承)。</span><span class="sxs-lookup"><span data-stu-id="013c5-131">Date and time of creation Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="013c5-132">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="013c5-132">lastSyncDateTime</span></span>|<span data-ttu-id="013c5-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="013c5-133">DateTimeOffset</span></span>|<span data-ttu-id="013c5-134">アプリが管理サービスと最後に同期した日時。</span><span class="sxs-lookup"><span data-stu-id="013c5-134">Date and time of last the app synced with management service.</span></span> <span data-ttu-id="013c5-135">[managedAppRegistration](../resources/intune_mam_managedappregistration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="013c5-135">Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="013c5-136">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="013c5-136">applicationVersion</span></span>|<span data-ttu-id="013c5-137">String</span><span class="sxs-lookup"><span data-stu-id="013c5-137">String</span></span>|<span data-ttu-id="013c5-138">アプリのバージョン ([managedAppRegistration](../resources/intune_mam_managedappregistration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="013c5-138">App version Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="013c5-139">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="013c5-139">managementSdkVersion</span></span>|<span data-ttu-id="013c5-140">String</span><span class="sxs-lookup"><span data-stu-id="013c5-140">String</span></span>|<span data-ttu-id="013c5-141">アプリ管理 SDK のバージョン ([managedAppRegistration](../resources/intune_mam_managedappregistration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="013c5-141">App management SDK version Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="013c5-142">platformVersion</span><span class="sxs-lookup"><span data-stu-id="013c5-142">platformVersion</span></span>|<span data-ttu-id="013c5-143">String</span><span class="sxs-lookup"><span data-stu-id="013c5-143">String</span></span>|<span data-ttu-id="013c5-144">オペレーティング システムのバージョン ([managedAppRegistration](../resources/intune_mam_managedappregistration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="013c5-144">Operating System version Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="013c5-145">deviceType</span><span class="sxs-lookup"><span data-stu-id="013c5-145">deviceType</span></span>|<span data-ttu-id="013c5-146">String</span><span class="sxs-lookup"><span data-stu-id="013c5-146">String</span></span>|<span data-ttu-id="013c5-147">ホスト デバイスの種類 ([managedAppRegistration](../resources/intune_mam_managedappregistration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="013c5-147">Host device type Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="013c5-148">deviceTag</span><span class="sxs-lookup"><span data-stu-id="013c5-148">deviceTag</span></span>|<span data-ttu-id="013c5-149">String</span><span class="sxs-lookup"><span data-stu-id="013c5-149">String</span></span>|<span data-ttu-id="013c5-150">アプリ管理 SDK が生成したタグ。同じデバイスでホストされているアプリの関連付けに役立ちます。</span><span class="sxs-lookup"><span data-stu-id="013c5-150">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="013c5-151">あらゆる状況でのアプリの関連付けを保証するものではありません。</span><span class="sxs-lookup"><span data-stu-id="013c5-151">Not guaranteed to relate apps in all conditions.</span></span> <span data-ttu-id="013c5-152">[managedAppRegistration](../resources/intune_mam_managedappregistration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="013c5-152">Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="013c5-153">deviceName</span><span class="sxs-lookup"><span data-stu-id="013c5-153">deviceName</span></span>|<span data-ttu-id="013c5-154">String</span><span class="sxs-lookup"><span data-stu-id="013c5-154">String</span></span>|<span data-ttu-id="013c5-155">ホスト デバイスの名前 ([managedAppRegistration](../resources/intune_mam_managedappregistration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="013c5-155">Host device name Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="013c5-156">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="013c5-156">flaggedReasons</span></span>|<span data-ttu-id="013c5-157">[managedAppFlaggedReason](../resources/intune_mam_managedappflaggedreason.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="013c5-157">[managedAppFlaggedReason](../resources/intune_mam_managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="013c5-158">アプリ登録にフラグが設定された、0 個以上の理由。</span><span class="sxs-lookup"><span data-stu-id="013c5-158">Zero or more reasons an app registration is flagged.</span></span> <span data-ttu-id="013c5-159">例: </span><span class="sxs-lookup"><span data-stu-id="013c5-159">E.g.</span></span> <span data-ttu-id="013c5-160">[managedAppRegistration](../resources/intune_mam_managedappregistration.md)から継承のルート デバイス上で実行されているアプリケーションです。</span><span class="sxs-lookup"><span data-stu-id="013c5-160">app running on rooted device Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md).</span></span> <span data-ttu-id="013c5-161">使用可能な値は、`none`、`rootedDevice` です。</span><span class="sxs-lookup"><span data-stu-id="013c5-161">Possible values are: `none`, `rootedDevice`.</span></span>|
|<span data-ttu-id="013c5-162">userId</span><span class="sxs-lookup"><span data-stu-id="013c5-162">userId</span></span>|<span data-ttu-id="013c5-163">String</span><span class="sxs-lookup"><span data-stu-id="013c5-163">String</span></span>|<span data-ttu-id="013c5-164">このアプリの登録が属するユーザー ID。</span><span class="sxs-lookup"><span data-stu-id="013c5-164">The user Id to who this app registration belongs.</span></span> <span data-ttu-id="013c5-165">[managedAppRegistration](../resources/intune_mam_managedappregistration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="013c5-165">Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="013c5-166">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="013c5-166">appIdentifier</span></span>|[<span data-ttu-id="013c5-167">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="013c5-167">mobileAppIdentifier</span></span>](../resources/intune_mam_mobileappidentifier.md)|<span data-ttu-id="013c5-168">アプリ パッケージの識別子 ([managedAppRegistration](../resources/intune_mam_managedappregistration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="013c5-168">The app package Identifier Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="013c5-169">id</span><span class="sxs-lookup"><span data-stu-id="013c5-169">id</span></span>|<span data-ttu-id="013c5-170">String</span><span class="sxs-lookup"><span data-stu-id="013c5-170">String</span></span>|<span data-ttu-id="013c5-171">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="013c5-171">Key of the entity.</span></span> <span data-ttu-id="013c5-172">[managedAppRegistration](../resources/intune_mam_managedappregistration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="013c5-172">Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="013c5-173">version</span><span class="sxs-lookup"><span data-stu-id="013c5-173">version</span></span>|<span data-ttu-id="013c5-174">String</span><span class="sxs-lookup"><span data-stu-id="013c5-174">String</span></span>|<span data-ttu-id="013c5-175">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="013c5-175">Version of the entity.</span></span> <span data-ttu-id="013c5-176">[managedAppRegistration](../resources/intune_mam_managedappregistration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="013c5-176">Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="013c5-177">応答</span><span class="sxs-lookup"><span data-stu-id="013c5-177">Response</span></span>
<span data-ttu-id="013c5-178">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [androidManagedAppRegistration](../resources/intune_mam_androidmanagedappregistration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="013c5-178">If successful, this method returns a `201 Created` response code and a [androidManagedAppRegistration](../resources/intune_mam_androidmanagedappregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="013c5-179">例</span><span class="sxs-lookup"><span data-stu-id="013c5-179">Example</span></span>
### <a name="request"></a><span data-ttu-id="013c5-180">要求</span><span class="sxs-lookup"><span data-stu-id="013c5-180">Request</span></span>
<span data-ttu-id="013c5-181">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="013c5-181">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppRegistrations
Content-type: application/json
Content-length: 645

{
  "@odata.type": "#microsoft.graph.androidManagedAppRegistration",
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

### <a name="response"></a><span data-ttu-id="013c5-182">応答</span><span class="sxs-lookup"><span data-stu-id="013c5-182">Response</span></span>
<span data-ttu-id="013c5-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="013c5-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



