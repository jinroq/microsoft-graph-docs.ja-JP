# <a name="update-androidforworkenrollmentprofile"></a><span data-ttu-id="8216c-101">androidForWorkEnrollmentProfile の更新</span><span class="sxs-lookup"><span data-stu-id="8216c-101">Update androidForWorkEnrollmentProfile</span></span>

> <span data-ttu-id="8216c-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="8216c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8216c-103">[androidForWorkEnrollmentProfile](../resources/intune_androidforwork_androidforworkenrollmentprofile.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="8216c-103">Update the properties of a [calendar](../resources/intune_androidforwork_androidforworkenrollmentprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8216c-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="8216c-104">Prerequisites</span></span>
<span data-ttu-id="8216c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8216c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8216c-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8216c-107">Permission type</span></span>|<span data-ttu-id="8216c-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="8216c-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8216c-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8216c-109">Delegated (work or school account)</span></span>|<span data-ttu-id="8216c-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8216c-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="8216c-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8216c-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8216c-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8216c-112">Not supported.</span></span>|
|<span data-ttu-id="8216c-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8216c-113">Application</span></span>|<span data-ttu-id="8216c-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8216c-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8216c-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8216c-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidForWorkEnrollmentProfiles/{androidForWorkEnrollmentProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="8216c-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8216c-116">Request headers</span></span>
|<span data-ttu-id="8216c-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8216c-117">Header</span></span>|<span data-ttu-id="8216c-118">値</span><span class="sxs-lookup"><span data-stu-id="8216c-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8216c-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="8216c-119">Authorization</span></span>|<span data-ttu-id="8216c-120">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="8216c-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="8216c-121">Accept</span><span class="sxs-lookup"><span data-stu-id="8216c-121">Accept</span></span>|<span data-ttu-id="8216c-122">application/json</span><span class="sxs-lookup"><span data-stu-id="8216c-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8216c-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="8216c-123">Request body</span></span>
<span data-ttu-id="8216c-124">要求本文で、[androidForWorkEnrollmentProfile](../resources/intune_androidforwork_androidforworkenrollmentprofile.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="8216c-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_androidforwork_androidforworkenrollmentprofile.md) object.</span></span>

<span data-ttu-id="8216c-125">次の表に、[androidForWorkEnrollmentProfile](../resources/intune_androidforwork_androidforworkenrollmentprofile.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="8216c-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="8216c-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8216c-126">Property</span></span>|<span data-ttu-id="8216c-127">型</span><span class="sxs-lookup"><span data-stu-id="8216c-127">Type</span></span>|<span data-ttu-id="8216c-128">説明</span><span class="sxs-lookup"><span data-stu-id="8216c-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8216c-129">accountId</span><span class="sxs-lookup"><span data-stu-id="8216c-129">accountId</span></span>|<span data-ttu-id="8216c-130">String</span><span class="sxs-lookup"><span data-stu-id="8216c-130">String</span></span>|<span data-ttu-id="8216c-131">登録プロファイルが属するテナント GUID。</span><span class="sxs-lookup"><span data-stu-id="8216c-131">Tenant GUID the enrollment profile belongs to.</span></span>|
|<span data-ttu-id="8216c-132">id</span><span class="sxs-lookup"><span data-stu-id="8216c-132">id</span></span>|<span data-ttu-id="8216c-133">String</span><span class="sxs-lookup"><span data-stu-id="8216c-133">String</span></span>|<span data-ttu-id="8216c-134">登録プロファイルの一意の GUID。</span><span class="sxs-lookup"><span data-stu-id="8216c-134">Unique GUID for the enrollment profile.</span></span>|
|<span data-ttu-id="8216c-135">name</span><span class="sxs-lookup"><span data-stu-id="8216c-135">name</span></span>|<span data-ttu-id="8216c-136">String</span><span class="sxs-lookup"><span data-stu-id="8216c-136">String</span></span>|<span data-ttu-id="8216c-137">(使用されていない) 登録プロファイルの表示名。</span><span class="sxs-lookup"><span data-stu-id="8216c-137">(Deprecated) Display name for the enrollment profile.</span></span>|
|<span data-ttu-id="8216c-138">displayName</span><span class="sxs-lookup"><span data-stu-id="8216c-138">displayName</span></span>|<span data-ttu-id="8216c-139">String</span><span class="sxs-lookup"><span data-stu-id="8216c-139">String</span></span>|<span data-ttu-id="8216c-140">登録プロファイルの表示名。</span><span class="sxs-lookup"><span data-stu-id="8216c-140">Display name for the enrollment profile.</span></span>|
|<span data-ttu-id="8216c-141">description</span><span class="sxs-lookup"><span data-stu-id="8216c-141">description</span></span>|<span data-ttu-id="8216c-142">String</span><span class="sxs-lookup"><span data-stu-id="8216c-142">String</span></span>|<span data-ttu-id="8216c-143">登録プロファイルの説明。</span><span class="sxs-lookup"><span data-stu-id="8216c-143">Description for the enrollment profile.</span></span>|
|<span data-ttu-id="8216c-144">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="8216c-144">createdDateTime</span></span>|<span data-ttu-id="8216c-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8216c-145">DateTimeOffset</span></span>|<span data-ttu-id="8216c-146">登録プロファイルが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="8216c-146">Date time the enrollment profile was created.</span></span>|
|<span data-ttu-id="8216c-147">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8216c-147">modifiedDateTime</span></span>|<span data-ttu-id="8216c-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8216c-148">DateTimeOffset</span></span>|<span data-ttu-id="8216c-149">(使用されていない) 登録プロファイルが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="8216c-149">(Deprecated) Date time the enrollment profile was last modified.</span></span>|
|<span data-ttu-id="8216c-150">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="8216c-150">lastModifiedDateTime</span></span>|<span data-ttu-id="8216c-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8216c-151">DateTimeOffset</span></span>|<span data-ttu-id="8216c-152">登録プロファイルが最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="8216c-152">Date time the enrollment profile was last modified.</span></span>|
|<span data-ttu-id="8216c-153">tokenValue</span><span class="sxs-lookup"><span data-stu-id="8216c-153">tokenValue</span></span>|<span data-ttu-id="8216c-154">String</span><span class="sxs-lookup"><span data-stu-id="8216c-154">String</span></span>|<span data-ttu-id="8216c-155">この登録プロファイル用に最後に作成されたトークンの値。</span><span class="sxs-lookup"><span data-stu-id="8216c-155">Value of the most recently created token for this enrollment profile.</span></span>|
|<span data-ttu-id="8216c-156">tokenExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="8216c-156">tokenExpirationDateTime</span></span>|<span data-ttu-id="8216c-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8216c-157">DateTimeOffset</span></span>|<span data-ttu-id="8216c-158">最後に作成されたトークンの有効期限が切れる日時。</span><span class="sxs-lookup"><span data-stu-id="8216c-158">Date time the most recently created token will expire.</span></span>|
|<span data-ttu-id="8216c-159">totalEnrollmentCount</span><span class="sxs-lookup"><span data-stu-id="8216c-159">totalEnrollmentCount</span></span>|<span data-ttu-id="8216c-160">Int32</span><span class="sxs-lookup"><span data-stu-id="8216c-160">Int32</span></span>|<span data-ttu-id="8216c-161">(使用されていない) この登録プロファイルを使用して登録した Android デバイスの合計数。</span><span class="sxs-lookup"><span data-stu-id="8216c-161">(Deprecated) Total number of Android devices that have enrolled using this enrollment profile.</span></span>|
|<span data-ttu-id="8216c-162">enrolledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8216c-162">enrolledDeviceCount</span></span>|<span data-ttu-id="8216c-163">Int32</span><span class="sxs-lookup"><span data-stu-id="8216c-163">Int32</span></span>|<span data-ttu-id="8216c-164">この登録プロファイルを使用して登録した Android デバイスの合計数。</span><span class="sxs-lookup"><span data-stu-id="8216c-164">Total number of Android devices that have enrolled using this enrollment profile.</span></span>|
|<span data-ttu-id="8216c-165">qrCode</span><span class="sxs-lookup"><span data-stu-id="8216c-165">qrCode</span></span>|<span data-ttu-id="8216c-166">String</span><span class="sxs-lookup"><span data-stu-id="8216c-166">String</span></span>|<span data-ttu-id="8216c-167">(使用されていない) トークンの QR コードを生成するために使用する文字列。</span><span class="sxs-lookup"><span data-stu-id="8216c-167">(Deprecated) String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="8216c-168">qrCodeContent</span><span class="sxs-lookup"><span data-stu-id="8216c-168">qrCodeContent</span></span>|<span data-ttu-id="8216c-169">String</span><span class="sxs-lookup"><span data-stu-id="8216c-169">String</span></span>|<span data-ttu-id="8216c-170">トークンの QR コードを生成するために使用する文字列。</span><span class="sxs-lookup"><span data-stu-id="8216c-170">String used to generate a QR code for the token.</span></span>|
|<span data-ttu-id="8216c-171">qrCodeImage</span><span class="sxs-lookup"><span data-stu-id="8216c-171">qrCodeImage</span></span>|[<span data-ttu-id="8216c-172">mimeContent</span><span class="sxs-lookup"><span data-stu-id="8216c-172">MimeContent</span></span>](../resources/intune_androidforwork_mimecontent.md)|<span data-ttu-id="8216c-173">トークンの QR コードを生成するために使用する文字列。</span><span class="sxs-lookup"><span data-stu-id="8216c-173">String used to generate a QR code for the token.</span></span>|



## <a name="response"></a><span data-ttu-id="8216c-174">応答</span><span class="sxs-lookup"><span data-stu-id="8216c-174">Response</span></span>
<span data-ttu-id="8216c-175">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [androidForWorkEnrollmentProfile](../resources/intune_androidforwork_androidforworkenrollmentprofile.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="8216c-175">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_androidforwork_androidforworkenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8216c-176">例</span><span class="sxs-lookup"><span data-stu-id="8216c-176">Example</span></span>
### <a name="request"></a><span data-ttu-id="8216c-177">要求</span><span class="sxs-lookup"><span data-stu-id="8216c-177">Request</span></span>
<span data-ttu-id="8216c-178">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8216c-178">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/androidForWorkEnrollmentProfiles/{androidForWorkEnrollmentProfileId}
Content-type: application/json
Content-length: 575

{
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

### <a name="response"></a><span data-ttu-id="8216c-179">応答</span><span class="sxs-lookup"><span data-stu-id="8216c-179">Response</span></span>
<span data-ttu-id="8216c-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8216c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



