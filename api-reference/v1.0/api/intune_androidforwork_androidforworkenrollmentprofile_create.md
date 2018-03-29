# <a name="create-androidforworkenrollmentprofile"></a><span data-ttu-id="5639b-101">Create androidForWorkEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="5639b-101">Create androidForWorkEnrollmentProfile</span></span>

> <span data-ttu-id="5639b-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="5639b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5639b-103">新しい [androidForWorkEnrollmentProfile](../resources/intune_androidforwork_androidforworkenrollmentprofile.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="5639b-103">Create a new [plannerBucket](../resources/intune_androidforwork_androidforworkenrollmentprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5639b-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="5639b-104">Prerequisites</span></span>
<span data-ttu-id="5639b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5639b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5639b-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5639b-107">Permission type</span></span>|<span data-ttu-id="5639b-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="5639b-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5639b-109">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="5639b-109">Delegated (work or school account)</span></span>|<span data-ttu-id="5639b-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5639b-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5639b-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5639b-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5639b-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5639b-112">Not supported.</span></span>|
|<span data-ttu-id="5639b-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5639b-113">Application</span></span>|<span data-ttu-id="5639b-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5639b-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5639b-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5639b-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/androidForWorkEnrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="5639b-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5639b-116">Request headers</span></span>
|<span data-ttu-id="5639b-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5639b-117">Header</span></span>|<span data-ttu-id="5639b-118">値</span><span class="sxs-lookup"><span data-stu-id="5639b-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5639b-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="5639b-119">Authorization</span></span>|<span data-ttu-id="5639b-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="5639b-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="5639b-121">Accept</span><span class="sxs-lookup"><span data-stu-id="5639b-121">Accept</span></span>|<span data-ttu-id="5639b-122">application/json</span><span class="sxs-lookup"><span data-stu-id="5639b-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5639b-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="5639b-123">Request body</span></span>
<span data-ttu-id="5639b-124">要求本文に、androidForWorkEnrollmentProfile オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="5639b-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="5639b-125">次の表に、androidForWorkEnrollmentProfile 作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="5639b-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="5639b-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5639b-126">Property</span></span>|<span data-ttu-id="5639b-127">型</span><span class="sxs-lookup"><span data-stu-id="5639b-127">Type</span></span>|<span data-ttu-id="5639b-128">説明</span><span class="sxs-lookup"><span data-stu-id="5639b-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5639b-129">accountId</span><span class="sxs-lookup"><span data-stu-id="5639b-129">accountId</span></span>|<span data-ttu-id="5639b-130">String</span><span class="sxs-lookup"><span data-stu-id="5639b-130">String</span></span>|<span data-ttu-id="5639b-131">登録プロファイルが属するテナント GUID。</span><span class="sxs-lookup"><span data-stu-id="5639b-131">Tenant GUID the enrollment profile belongs to.</span></span>|
|<span data-ttu-id="5639b-132">id</span><span class="sxs-lookup"><span data-stu-id="5639b-132">id</span></span>|<span data-ttu-id="5639b-133">String</span><span class="sxs-lookup"><span data-stu-id="5639b-133">String</span></span>|<span data-ttu-id="5639b-134">登録プロファイル用の一意な GUID。</span><span class="sxs-lookup"><span data-stu-id="5639b-134">Unique GUID for the enrollment profile.</span></span>|
|<span data-ttu-id="5639b-135">name</span><span class="sxs-lookup"><span data-stu-id="5639b-135">name</span></span>|<span data-ttu-id="5639b-136">String</span><span class="sxs-lookup"><span data-stu-id="5639b-136">String</span></span>|<span data-ttu-id="5639b-137">(使用されていない) 登録プロファイルの表示名。</span><span class="sxs-lookup"><span data-stu-id="5639b-137">(Deprecated) Display name for the enrollment profile.</span></span>|
|<span data-ttu-id="5639b-138">displayName</span><span class="sxs-lookup"><span data-stu-id="5639b-138">displayName</span></span>|<span data-ttu-id="5639b-139">String</span><span class="sxs-lookup"><span data-stu-id="5639b-139">String</span></span>|<span data-ttu-id="5639b-140">登録プロファイルの表示名。</span><span class="sxs-lookup"><span data-stu-id="5639b-140">Display name for the enrollment profile.</span></span>|
|<span data-ttu-id="5639b-141">description</span><span class="sxs-lookup"><span data-stu-id="5639b-141">description</span></span>|<span data-ttu-id="5639b-142">String</span><span class="sxs-lookup"><span data-stu-id="5639b-142">String</span></span>|<span data-ttu-id="5639b-143">登録プロファイルの説明。</span><span class="sxs-lookup"><span data-stu-id="5639b-143">Description for the enrollment profile.</span></span>|
|<span data-ttu-id="5639b-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5639b-144">createdDateTime</span></span>|<span data-ttu-id="5639b-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5639b-145">DateTimeOffset</span></span>|<span data-ttu-id="5639b-146">登録プロファイルが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="5639b-146">Date time the enrollment profile was created.</span></span>|
|<span data-ttu-id="5639b-147">変更された日時</span><span class="sxs-lookup"><span data-stu-id="5639b-147">modifiedDateTime</span></span>|<span data-ttu-id="5639b-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5639b-148">DateTimeOffset</span></span>|<span data-ttu-id="5639b-149">(使用されていない) 登録プロファイルが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="5639b-149">(Deprecated) Date time the enrollment profile was last modified.</span></span>|
|<span data-ttu-id="5639b-150">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5639b-150">lastModifiedDateTime</span></span>|<span data-ttu-id="5639b-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5639b-151">DateTimeOffset</span></span>|<span data-ttu-id="5639b-152">登録プロファイルが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="5639b-152">Date time the enrollment profile was last modified.</span></span>|
|<span data-ttu-id="5639b-153">tokenValue</span><span class="sxs-lookup"><span data-stu-id="5639b-153">tokenValue</span></span>|<span data-ttu-id="5639b-154">String</span><span class="sxs-lookup"><span data-stu-id="5639b-154">String</span></span>|<span data-ttu-id="5639b-155">この登録プロファイル用に最後に作成されたトークンの値。</span><span class="sxs-lookup"><span data-stu-id="5639b-155">Value of the most recently created token for this enrollment profile.</span></span>|
|<span data-ttu-id="5639b-156">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="5639b-156">tokenExpirationDateTime</span></span>|<span data-ttu-id="5639b-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5639b-157">DateTimeOffset</span></span>|<span data-ttu-id="5639b-158">最後に作成されたトークンの有効期限が切れる日時。</span><span class="sxs-lookup"><span data-stu-id="5639b-158">Date time the most recently created token will expire.</span></span>|
|<span data-ttu-id="5639b-159">totalEnrollmentCount</span><span class="sxs-lookup"><span data-stu-id="5639b-159">totalEnrollmentCount</span></span>|<span data-ttu-id="5639b-160">Int32</span><span class="sxs-lookup"><span data-stu-id="5639b-160">Int32</span></span>|<span data-ttu-id="5639b-161">(使用されていない) この登録プロファイルを使用して登録した Android デバイスの合計数。</span><span class="sxs-lookup"><span data-stu-id="5639b-161">(Deprecated) Total number of Android devices that have enrolled using this enrollment profile.</span></span>|
|<span data-ttu-id="5639b-162">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5639b-162">enrolledDeviceCount</span></span>|<span data-ttu-id="5639b-163">Int32</span><span class="sxs-lookup"><span data-stu-id="5639b-163">Int32</span></span>|<span data-ttu-id="5639b-164">この登録プロファイルを使用して登録した Android デバイスの合計数。</span><span class="sxs-lookup"><span data-stu-id="5639b-164">Total number of Android devices that have enrolled using this enrollment profile.</span></span>|
|<span data-ttu-id="5639b-165">qrCode</span><span class="sxs-lookup"><span data-stu-id="5639b-165">qrCode</span></span>|<span data-ttu-id="5639b-166">String</span><span class="sxs-lookup"><span data-stu-id="5639b-166">String</span></span>|<span data-ttu-id="5639b-167">(使用されていない) トークン用の QR コードを生成するために使用された文字列。</span><span class="sxs-lookup"><span data-stu-id="5639b-167">(Deprecated) String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="5639b-168">qrCodeContent</span><span class="sxs-lookup"><span data-stu-id="5639b-168">qrCodeContent</span></span>|<span data-ttu-id="5639b-169">String</span><span class="sxs-lookup"><span data-stu-id="5639b-169">String</span></span>|<span data-ttu-id="5639b-170">トークン用の QR コードを生成するために使用された文字列。</span><span class="sxs-lookup"><span data-stu-id="5639b-170">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="5639b-171">qrCodeImage</span><span class="sxs-lookup"><span data-stu-id="5639b-171">qrCodeImage</span></span>|[<span data-ttu-id="5639b-172">mimeContent</span><span class="sxs-lookup"><span data-stu-id="5639b-172">MimeContent</span></span>](../resources/intune_androidforwork_mimecontent.md)|<span data-ttu-id="5639b-173">トークン用の QR コードを生成するために使用された文字列。</span><span class="sxs-lookup"><span data-stu-id="5639b-173">String used to generate a QR code for the token.</span></span>|



## <a name="response"></a><span data-ttu-id="5639b-174">応答</span><span class="sxs-lookup"><span data-stu-id="5639b-174">Response</span></span>
<span data-ttu-id="5639b-175">このメソッドが成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [androidForWorkEnrollmentProfile](../resources/intune_androidforwork_androidforworkenrollmentprofile.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="5639b-175">If successful, this method returns a `201 Created` response code and a [section](../resources/intune_androidforwork_androidforworkenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5639b-176">例</span><span class="sxs-lookup"><span data-stu-id="5639b-176">Example</span></span>
### <a name="request"></a><span data-ttu-id="5639b-177">要求</span><span class="sxs-lookup"><span data-stu-id="5639b-177">Request</span></span>
<span data-ttu-id="5639b-178">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5639b-178">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/androidForWorkEnrollmentProfiles
Content-type: application/json
Content-length: 645

{
  "@odata.type": "#microsoft.graph.androidForWorkEnrollmentProfile",
  "accountId": "Account Id value",
  "name": "Name value",
  "displayName": "Display Name value",
  "description": "Description value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "tokenValue": "Token Value value",
  "tokenExpirationDateTime": "2016-12-31T23:59:54.0590989-08:00",
  "totalEnrollmentCount": 4,
  "enrolledDeviceCount": 3,
  "qrCode": "Qr Code value",
  "qrCodeContent": "Qr Code Content value",
  "qrCodeImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  }
}
```

### <a name="response"></a><span data-ttu-id="5639b-179">応答</span><span class="sxs-lookup"><span data-stu-id="5639b-179">Response</span></span>
<span data-ttu-id="5639b-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="5639b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 813

{
  "@odata.type": "#microsoft.graph.androidForWorkEnrollmentProfile",
  "accountId": "Account Id value",
  "id": "e6742553-2553-e674-5325-74e6532574e6",
  "name": "Name value",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "tokenValue": "Token Value value",
  "tokenExpirationDateTime": "2016-12-31T23:59:54.0590989-08:00",
  "totalEnrollmentCount": 4,
  "enrolledDeviceCount": 3,
  "qrCode": "Qr Code value",
  "qrCodeContent": "Qr Code Content value",
  "qrCodeImage": {
    "@odata.type": "microsoft.graph.mimeContent",
    "type": "Type value",
    "value": "dmFsdWU="
  }
}
```



