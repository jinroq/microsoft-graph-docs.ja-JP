# <a name="update-vpptoken"></a><span data-ttu-id="ad36d-101">VPPトークンの更新</span><span class="sxs-lookup"><span data-stu-id="ad36d-101">Update vppToken</span></span>

> <span data-ttu-id="ad36d-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ad36d-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ad36d-103">[VPPトークン](../resources/intune_onboarding_vpptoken.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="ad36d-103">Update the properties of a [vppToken](../resources/intune_onboarding_vpptoken.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ad36d-104">必要条件</span><span class="sxs-lookup"><span data-stu-id="ad36d-104">Prerequisites</span></span>
<span data-ttu-id="ad36d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ad36d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ad36d-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ad36d-107">Permission type</span></span>|<span data-ttu-id="ad36d-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ad36d-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ad36d-109">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="ad36d-109">Delegated (work or school account)</span></span>|<span data-ttu-id="ad36d-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad36d-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ad36d-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ad36d-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ad36d-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ad36d-112">Not supported.</span></span>|
|<span data-ttu-id="ad36d-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ad36d-113">Application</span></span>|<span data-ttu-id="ad36d-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ad36d-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ad36d-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ad36d-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/vppTokens/{vppTokenId}
```

## <a name="request-headers"></a><span data-ttu-id="ad36d-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ad36d-116">Request headers</span></span>
|<span data-ttu-id="ad36d-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ad36d-117">Header</span></span>|<span data-ttu-id="ad36d-118">値</span><span class="sxs-lookup"><span data-stu-id="ad36d-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ad36d-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="ad36d-119">Authorization</span></span>|<span data-ttu-id="ad36d-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="ad36d-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ad36d-121">Accept</span><span class="sxs-lookup"><span data-stu-id="ad36d-121">Accept</span></span>|<span data-ttu-id="ad36d-122">application/json</span><span class="sxs-lookup"><span data-stu-id="ad36d-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ad36d-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="ad36d-123">Request body</span></span>
<span data-ttu-id="ad36d-124">要求本文で、[VPPトークン](../resources/intune_onboarding_vpptoken.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="ad36d-124">In the request body, supply a JSON representation for the [vppToken](../resources/intune_onboarding_vpptoken.md) object.</span></span>

<span data-ttu-id="ad36d-125">次の表に、[VPPトークン](../resources/intune_onboarding_vpptoken.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="ad36d-125">The following table shows the properties that are required when you create the [vppToken](../resources/intune_onboarding_vpptoken.md).</span></span>

|<span data-ttu-id="ad36d-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ad36d-126">Property</span></span>|<span data-ttu-id="ad36d-127">型</span><span class="sxs-lookup"><span data-stu-id="ad36d-127">Type</span></span>|<span data-ttu-id="ad36d-128">説明</span><span class="sxs-lookup"><span data-stu-id="ad36d-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ad36d-129">id</span><span class="sxs-lookup"><span data-stu-id="ad36d-129">id</span></span>|<span data-ttu-id="ad36d-130">文字列</span><span class="sxs-lookup"><span data-stu-id="ad36d-130">String</span></span>|<span data-ttu-id="ad36d-131">appleVolumePurchaseProgramToken 作成時に自動的に生成されます。</span><span class="sxs-lookup"><span data-stu-id="ad36d-131">This is automatically generated when the appleVolumePurchaseProgramToken is created.</span></span> <span data-ttu-id="ad36d-132">エンティティのキーになります。</span><span class="sxs-lookup"><span data-stu-id="ad36d-132">It is the Key of the entity.</span></span>|
|<span data-ttu-id="ad36d-133">organizationName</span><span class="sxs-lookup"><span data-stu-id="ad36d-133">organizationName</span></span>|<span data-ttu-id="ad36d-134">文字列</span><span class="sxs-lookup"><span data-stu-id="ad36d-134">String</span></span>|<span data-ttu-id="ad36d-135">Apple ボリューム購入プログラムのトークンに関連付けられている組織</span><span class="sxs-lookup"><span data-stu-id="ad36d-135">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="ad36d-136">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="ad36d-136">vppTokenAccountType</span></span>|[<span data-ttu-id="ad36d-137">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="ad36d-137">vppTokenAccountType</span></span>](../resources/intune_shared_vpptokenaccounttype.md)|<span data-ttu-id="ad36d-138">特定の Apple ボリューム購入プログラムのトークンが関連付けられている、ボリューム購入プログラムの種類。</span><span class="sxs-lookup"><span data-stu-id="ad36d-138">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="ad36d-139">可能な値は、`business`、`education` です。</span><span class="sxs-lookup"><span data-stu-id="ad36d-139">Possible values are: `business`, `education`.</span></span> <span data-ttu-id="ad36d-140">可能な値は、`business`、`education` です。</span><span class="sxs-lookup"><span data-stu-id="ad36d-140">Possible values are: `business`, `education`.</span></span>|
|<span data-ttu-id="ad36d-141">appleId</span><span class="sxs-lookup"><span data-stu-id="ad36d-141">appleId</span></span>|<span data-ttu-id="ad36d-142">文字列</span><span class="sxs-lookup"><span data-stu-id="ad36d-142">String</span></span>|<span data-ttu-id="ad36d-143">特定の Apple ボリューム購入プログラムのトークンに関連付けられている Apple ID。</span><span class="sxs-lookup"><span data-stu-id="ad36d-143">The apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="ad36d-144">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="ad36d-144">expirationDateTime</span></span>|<span data-ttu-id="ad36d-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ad36d-145">DateTimeOffset</span></span>|<span data-ttu-id="ad36d-146">Apple ボリューム購入プログラムのトークンの有効期限。</span><span class="sxs-lookup"><span data-stu-id="ad36d-146">The expiration date time of the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="ad36d-147">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="ad36d-147">lastSyncDateTime</span></span>|<span data-ttu-id="ad36d-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ad36d-148">DateTimeOffset</span></span>|<span data-ttu-id="ad36d-149">Apple ボリューム購入プログラムのトークンを使用して、Apple ボリューム購入プログラム サービスと最後にアプリケーションの同期を行った日時。</span><span class="sxs-lookup"><span data-stu-id="ad36d-149">The last time when an application sync was done with the Apple volume purchase program service using the the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="ad36d-150">トークン</span><span class="sxs-lookup"><span data-stu-id="ad36d-150">token</span></span>|<span data-ttu-id="ad36d-151">文字列</span><span class="sxs-lookup"><span data-stu-id="ad36d-151">String</span></span>|<span data-ttu-id="ad36d-152">Apple ボリューム購入プログラムからダウンロードした Apple ボリューム購入プログラムのトークン文字列。</span><span class="sxs-lookup"><span data-stu-id="ad36d-152">The Apple Volume Purchase Program Token string downloaded from the Apple Volume Purchase Program.</span></span>|
|<span data-ttu-id="ad36d-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ad36d-153">lastModifiedDateTime</span></span>|<span data-ttu-id="ad36d-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ad36d-154">DateTimeOffset</span></span>|<span data-ttu-id="ad36d-155">Apple ボリューム購入プログラムのトークンに関連付けられている最終変更日時。</span><span class="sxs-lookup"><span data-stu-id="ad36d-155">Last modification date time associated with the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="ad36d-156">状態
</span><span class="sxs-lookup"><span data-stu-id="ad36d-156">state</span></span>|[<span data-ttu-id="ad36d-157">vppTokenState</span><span class="sxs-lookup"><span data-stu-id="ad36d-157">vppTokenState</span></span>](../resources/intune_onboarding_vpptokenstate.md)|<span data-ttu-id="ad36d-158">Apple ボリューム購入プログラムのトークンの現在の状態。</span><span class="sxs-lookup"><span data-stu-id="ad36d-158">Current state of the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="ad36d-159">可能な値は、`unknown`、`valid`、`expired`、`invalid`、`assignedToExternalMDM` です。</span><span class="sxs-lookup"><span data-stu-id="ad36d-159">Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span></span> <span data-ttu-id="ad36d-160">可能な値は、`unknown`、`valid`、`expired`、`invalid`、`assignedToExternalMDM` です。</span><span class="sxs-lookup"><span data-stu-id="ad36d-160">Possible values are: `unknown`, `valid`, `expired`, `invalid`, `assignedToExternalMDM`.</span></span>|
|<span data-ttu-id="ad36d-161">lastSyncStatus</span><span class="sxs-lookup"><span data-stu-id="ad36d-161">lastSyncStatus</span></span>|[<span data-ttu-id="ad36d-162">vppTokenSyncStatus</span><span class="sxs-lookup"><span data-stu-id="ad36d-162">vppTokenSyncStatus</span></span>](../resources/intune_onboarding_vpptokensyncstatus.md)|<span data-ttu-id="ad36d-163">Apple ボリューム購入プログラム トークンを使用して行われた最後のアプリケーションの同期の現在の同期状態。</span><span class="sxs-lookup"><span data-stu-id="ad36d-163">Current sync status of the last application sync which was triggered using the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="ad36d-164">可能な値は、`none`、`inProgress`、`completed`、`failed` です。</span><span class="sxs-lookup"><span data-stu-id="ad36d-164">Possible values are: `none`, `inProgress`, `completed`, `failed`.</span></span> <span data-ttu-id="ad36d-165">可能な値は、`none`、`inProgress`、`completed`、`failed` です。</span><span class="sxs-lookup"><span data-stu-id="ad36d-165">Possible values are: `none`, `inProgress`, `completed`, `failed`.</span></span>|
|<span data-ttu-id="ad36d-166">automaticallyUpdateApps</span><span class="sxs-lookup"><span data-stu-id="ad36d-166">automaticallyUpdateApps</span></span>|<span data-ttu-id="ad36d-167">ブール型</span><span class="sxs-lookup"><span data-stu-id="ad36d-167">Boolean</span></span>|<span data-ttu-id="ad36d-168">VPP トークンのアプリを自動で更新するかどうか。</span><span class="sxs-lookup"><span data-stu-id="ad36d-168">Whether or not apps for the VPP token will be automatically updated.</span></span>|
|<span data-ttu-id="ad36d-169">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="ad36d-169">countryOrRegion</span></span>|<span data-ttu-id="ad36d-170">文字列</span><span class="sxs-lookup"><span data-stu-id="ad36d-170">String</span></span>|<span data-ttu-id="ad36d-171">VPP トークンのアプリを自動で更新するかどうか。</span><span class="sxs-lookup"><span data-stu-id="ad36d-171">Whether or not apps for the VPP token will be automatically updated.</span></span>|



## <a name="response"></a><span data-ttu-id="ad36d-172">応答</span><span class="sxs-lookup"><span data-stu-id="ad36d-172">Response</span></span>
<span data-ttu-id="ad36d-173">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [VPPトークン](../resources/intune_onboarding_vpptoken.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ad36d-173">If successful, this method returns a `200 OK` response code and an updated [vppToken](../resources/intune_onboarding_vpptoken.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ad36d-174">例</span><span class="sxs-lookup"><span data-stu-id="ad36d-174">Example</span></span>
### <a name="request"></a><span data-ttu-id="ad36d-175">要求</span><span class="sxs-lookup"><span data-stu-id="ad36d-175">Request</span></span>
<span data-ttu-id="ad36d-176">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ad36d-176">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/vppTokens/{vppTokenId}
Content-type: application/json
Content-length: 461

{
  "@odata.type": "#microsoft.graph.vppToken",
  "organizationName": "Organization Name value",
  "vppTokenAccountType": "education",
  "appleId": "Apple Id value",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "token": "Token value",
  "state": "valid",
  "lastSyncStatus": "inProgress",
  "automaticallyUpdateApps": true,
  "countryOrRegion": "Country Or Region value"
}
```

### <a name="response"></a><span data-ttu-id="ad36d-177">応答</span><span class="sxs-lookup"><span data-stu-id="ad36d-177">Response</span></span>
<span data-ttu-id="ad36d-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ad36d-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 574

{
  "@odata.type": "#microsoft.graph.vppToken",
  "id": "9ceb2f92-2f92-9ceb-922f-eb9c922feb9c",
  "organizationName": "Organization Name value",
  "vppTokenAccountType": "education",
  "appleId": "Apple Id value",
  "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "token": "Token value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "state": "valid",
  "lastSyncStatus": "inProgress",
  "automaticallyUpdateApps": true,
  "countryOrRegion": "Country Or Region value"
}
```



