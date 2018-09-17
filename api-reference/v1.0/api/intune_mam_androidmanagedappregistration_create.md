# <a name="create-androidmanagedappregistration"></a><span data-ttu-id="ffa2c-101">androidManagedAppRegistration の作成</span><span class="sxs-lookup"><span data-stu-id="ffa2c-101">Create androidManagedAppRegistration</span></span>

> <span data-ttu-id="ffa2c-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ffa2c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ffa2c-103">新しい [androidManagedAppRegistration](../resources/intune_mam_androidmanagedappregistration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="ffa2c-103">Create a new [androidManagedAppRegistration](../resources/intune_mam_androidmanagedappregistration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ffa2c-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="ffa2c-104">Prerequisites</span></span>
<span data-ttu-id="ffa2c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ffa2c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ffa2c-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ffa2c-107">Permission type</span></span>|<span data-ttu-id="ffa2c-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ffa2c-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ffa2c-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ffa2c-109">Delegated (work or school account)</span></span>|<span data-ttu-id="ffa2c-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ffa2c-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ffa2c-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ffa2c-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ffa2c-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ffa2c-112">Not supported.</span></span>|
|<span data-ttu-id="ffa2c-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ffa2c-113">Application</span></span>|<span data-ttu-id="ffa2c-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ffa2c-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ffa2c-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ffa2c-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppRegistrations
```

## <a name="request-headers"></a><span data-ttu-id="ffa2c-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ffa2c-116">Request headers</span></span>
|<span data-ttu-id="ffa2c-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ffa2c-117">Header</span></span>|<span data-ttu-id="ffa2c-118">値</span><span class="sxs-lookup"><span data-stu-id="ffa2c-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ffa2c-119">承認</span><span class="sxs-lookup"><span data-stu-id="ffa2c-119">Authorization</span></span>|<span data-ttu-id="ffa2c-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="ffa2c-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ffa2c-121">承諾</span><span class="sxs-lookup"><span data-stu-id="ffa2c-121">Accept</span></span>|<span data-ttu-id="ffa2c-122">アプリケーションまたは JSON</span><span class="sxs-lookup"><span data-stu-id="ffa2c-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ffa2c-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="ffa2c-123">Request body</span></span>
<span data-ttu-id="ffa2c-124">要求本文で、androidManagedAppRegistration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="ffa2c-124">In the request body, supply a JSON representation for the androidManagedAppRegistration object.</span></span>

<span data-ttu-id="ffa2c-125">次の表に、androidManagedAppRegistration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="ffa2c-125">The following table shows the properties that are required when you create the androidManagedAppRegistration.</span></span>

|<span data-ttu-id="ffa2c-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ffa2c-126">Property</span></span>|<span data-ttu-id="ffa2c-127">タイプ</span><span class="sxs-lookup"><span data-stu-id="ffa2c-127">Type</span></span>|<span data-ttu-id="ffa2c-128">説明</span><span class="sxs-lookup"><span data-stu-id="ffa2c-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ffa2c-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ffa2c-129">createdDateTime</span></span>|<span data-ttu-id="ffa2c-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ffa2c-130">DateTimeOffset</span></span>|<span data-ttu-id="ffa2c-131">作成日時 ([managedAppRegistration](../resources/intune_mam_managedappregistration.md) から継承)。</span><span class="sxs-lookup"><span data-stu-id="ffa2c-131">Date and time of creation Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="ffa2c-132">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="ffa2c-132">lastSyncDateTime</span></span>|<span data-ttu-id="ffa2c-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ffa2c-133">DateTimeOffset</span></span>|<span data-ttu-id="ffa2c-134">アプリが管理サービスと最後に同期した日時。</span><span class="sxs-lookup"><span data-stu-id="ffa2c-134">Date and time of last the app synced with management service.</span></span> <span data-ttu-id="ffa2c-135">[managedAppRegistration](../resources/intune_mam_managedappregistration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ffa2c-135">Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="ffa2c-136">applicationVersion</span><span class="sxs-lookup"><span data-stu-id="ffa2c-136">applicationVersion</span></span>|<span data-ttu-id="ffa2c-137">文字列</span><span class="sxs-lookup"><span data-stu-id="ffa2c-137">String</span></span>|<span data-ttu-id="ffa2c-138">アプリのバージョン ([managedAppRegistration](../resources/intune_mam_managedappregistration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="ffa2c-138">App version Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="ffa2c-139">managementSdkVersion</span><span class="sxs-lookup"><span data-stu-id="ffa2c-139">managementSdkVersion</span></span>|<span data-ttu-id="ffa2c-140">文字列</span><span class="sxs-lookup"><span data-stu-id="ffa2c-140">String</span></span>|<span data-ttu-id="ffa2c-141">アプリ管理 SDK のバージョン ([managedAppRegistration](../resources/intune_mam_managedappregistration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="ffa2c-141">App management SDK version Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="ffa2c-142">platformVersion</span><span class="sxs-lookup"><span data-stu-id="ffa2c-142">platformVersion</span></span>|<span data-ttu-id="ffa2c-143">文字列</span><span class="sxs-lookup"><span data-stu-id="ffa2c-143">String</span></span>|<span data-ttu-id="ffa2c-144">オペレーティング システムのバージョン ([managedAppRegistration](../resources/intune_mam_managedappregistration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="ffa2c-144">Operating System version Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="ffa2c-145">deviceType</span><span class="sxs-lookup"><span data-stu-id="ffa2c-145">deviceType</span></span>|<span data-ttu-id="ffa2c-146">文字列</span><span class="sxs-lookup"><span data-stu-id="ffa2c-146">String</span></span>|<span data-ttu-id="ffa2c-147">ホスト デバイスの種類 ([managedAppRegistration](../resources/intune_mam_managedappregistration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="ffa2c-147">Host device type Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="ffa2c-148">deviceTag</span><span class="sxs-lookup"><span data-stu-id="ffa2c-148">deviceTag</span></span>|<span data-ttu-id="ffa2c-149">文字列</span><span class="sxs-lookup"><span data-stu-id="ffa2c-149">String</span></span>|<span data-ttu-id="ffa2c-150">アプリ管理 SDK が生成したタグ。同じデバイスでホストされているアプリの関連付けに役立ちます。</span><span class="sxs-lookup"><span data-stu-id="ffa2c-150">App management SDK generated tag, which helps relate apps hosted on the same device.</span></span> <span data-ttu-id="ffa2c-151">あらゆる状況でのアプリの関連付けを保証するものではありません。</span><span class="sxs-lookup"><span data-stu-id="ffa2c-151">Not guaranteed to relate apps in all conditions.</span></span> <span data-ttu-id="ffa2c-152">[managedAppRegistration](../resources/intune_mam_managedappregistration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ffa2c-152">Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="ffa2c-153">deviceName</span><span class="sxs-lookup"><span data-stu-id="ffa2c-153">deviceName</span></span>|<span data-ttu-id="ffa2c-154">文字列</span><span class="sxs-lookup"><span data-stu-id="ffa2c-154">String</span></span>|<span data-ttu-id="ffa2c-155">ホスト デバイスの名前 ([managedAppRegistration](../resources/intune_mam_managedappregistration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="ffa2c-155">Host device name Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="ffa2c-156">flaggedReasons</span><span class="sxs-lookup"><span data-stu-id="ffa2c-156">flaggedReasons</span></span>|<span data-ttu-id="ffa2c-157">[managedAppFlaggedReason](../resources/intune_mam_managedappflaggedreason.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ffa2c-157">[managedAppFlaggedReason enum](../resources/intune_mam_managedappflaggedreason.md) collection</span></span>|<span data-ttu-id="ffa2c-p104">アプリの登録にフラグが設定されている0個以上の理由。例えば、 [managedAppRegistration](../resources/intune_mam_managedappregistration.md)から継承されたルートデバイス上で実行されているアプリケーションです。使用可能な値: `none`、 `rootedDevice`。</span><span class="sxs-lookup"><span data-stu-id="ffa2c-p104">Zero or more reasons an app registration is flagged. E.g. app running on rooted device Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md). The possible values are: `none`, `rootedDevice`.</span></span>|
|<span data-ttu-id="ffa2c-162">userId</span><span class="sxs-lookup"><span data-stu-id="ffa2c-162">userId</span></span>|<span data-ttu-id="ffa2c-163">文字列</span><span class="sxs-lookup"><span data-stu-id="ffa2c-163">String</span></span>|<span data-ttu-id="ffa2c-164">このアプリの登録が属するユーザー ID。</span><span class="sxs-lookup"><span data-stu-id="ffa2c-164">The user Id to who this app registration belongs.</span></span> <span data-ttu-id="ffa2c-165">[managedAppRegistration](../resources/intune_mam_managedappregistration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ffa2c-165">Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="ffa2c-166">appIdentifier</span><span class="sxs-lookup"><span data-stu-id="ffa2c-166">appIdentifier</span></span>|[<span data-ttu-id="ffa2c-167">mobileAppIdentifier</span><span class="sxs-lookup"><span data-stu-id="ffa2c-167">mobileAppIdentifier</span></span>](../resources/intune_mam_mobileappidentifier.md)|<span data-ttu-id="ffa2c-168">アプリ パッケージの識別子 ([managedAppRegistration](../resources/intune_mam_managedappregistration.md) から継承)</span><span class="sxs-lookup"><span data-stu-id="ffa2c-168">The app package Identifier Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="ffa2c-169">ID</span><span class="sxs-lookup"><span data-stu-id="ffa2c-169">id</span></span>|<span data-ttu-id="ffa2c-170">文字列</span><span class="sxs-lookup"><span data-stu-id="ffa2c-170">String</span></span>|<span data-ttu-id="ffa2c-171">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="ffa2c-171">Key of the entity.</span></span> <span data-ttu-id="ffa2c-172">[managedAppRegistration](../resources/intune_mam_managedappregistration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ffa2c-172">Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|
|<span data-ttu-id="ffa2c-173">バージョン</span><span class="sxs-lookup"><span data-stu-id="ffa2c-173">version</span></span>|<span data-ttu-id="ffa2c-174">文字列</span><span class="sxs-lookup"><span data-stu-id="ffa2c-174">String</span></span>|<span data-ttu-id="ffa2c-175">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="ffa2c-175">Version of the entity.</span></span> <span data-ttu-id="ffa2c-176">[managedAppRegistration](../resources/intune_mam_managedappregistration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ffa2c-176">Inherited from [managedAppRegistration](../resources/intune_mam_managedappregistration.md)</span></span>|



## <a name="response"></a><span data-ttu-id="ffa2c-177">応答</span><span class="sxs-lookup"><span data-stu-id="ffa2c-177">Response</span></span>
<span data-ttu-id="ffa2c-178">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [androidManagedAppRegistration](../resources/intune_mam_androidmanagedappregistration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ffa2c-178">If successful, this method returns a `201 Created` response code and a [androidManagedAppRegistration](../resources/intune_mam_androidmanagedappregistration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ffa2c-179">例</span><span class="sxs-lookup"><span data-stu-id="ffa2c-179">Example</span></span>
### <a name="request"></a><span data-ttu-id="ffa2c-180">要求</span><span class="sxs-lookup"><span data-stu-id="ffa2c-180">Request</span></span>
<span data-ttu-id="ffa2c-181">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ffa2c-181">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ffa2c-182">応答</span><span class="sxs-lookup"><span data-stu-id="ffa2c-182">Response</span></span>
<span data-ttu-id="ffa2c-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ffa2c-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








