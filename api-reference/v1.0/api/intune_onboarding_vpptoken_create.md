# <a name="create-vpptoken"></a><span data-ttu-id="73437-101">vppToken の作成</span><span class="sxs-lookup"><span data-stu-id="73437-101">Create vppToken</span></span>

> <span data-ttu-id="73437-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="73437-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="73437-103">新規に[vppToken](../resources/intune_onboarding_vpptoken.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="73437-103">Create a new [vppToken](../resources/intune_onboarding_vpptoken.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="73437-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="73437-104">Prerequisites</span></span>
<span data-ttu-id="73437-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="73437-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="73437-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="73437-107">Permission type</span></span>|<span data-ttu-id="73437-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="73437-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="73437-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="73437-109">Delegated (work or school account)</span></span>|<span data-ttu-id="73437-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73437-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="73437-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="73437-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="73437-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="73437-112">Not supported.</span></span>|
|<span data-ttu-id="73437-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="73437-113">Application</span></span>|<span data-ttu-id="73437-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="73437-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="73437-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="73437-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/vppTokens
```

## <a name="request-headers"></a><span data-ttu-id="73437-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="73437-116">Request headers</span></span>
|<span data-ttu-id="73437-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="73437-117">Header</span></span>|<span data-ttu-id="73437-118">値</span><span class="sxs-lookup"><span data-stu-id="73437-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="73437-119">承認</span><span class="sxs-lookup"><span data-stu-id="73437-119">Authorization</span></span>|<span data-ttu-id="73437-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="73437-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="73437-121">承諾</span><span class="sxs-lookup"><span data-stu-id="73437-121">Accept</span></span>|<span data-ttu-id="73437-122">application/json</span><span class="sxs-lookup"><span data-stu-id="73437-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="73437-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="73437-123">Request body</span></span>
<span data-ttu-id="73437-124">要求本文で、vppToken オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="73437-124">In the request body, supply a JSON representation for the vppToken object.</span></span>

<span data-ttu-id="73437-125">次の表に、vppToken 作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="73437-125">The following table shows the properties that are required when you create the vppToken.</span></span>

|<span data-ttu-id="73437-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="73437-126">Property</span></span>|<span data-ttu-id="73437-127">タイプ</span><span class="sxs-lookup"><span data-stu-id="73437-127">Type</span></span>|<span data-ttu-id="73437-128">説明</span><span class="sxs-lookup"><span data-stu-id="73437-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="73437-129">id</span><span class="sxs-lookup"><span data-stu-id="73437-129">id</span></span>|<span data-ttu-id="73437-130">文字列</span><span class="sxs-lookup"><span data-stu-id="73437-130">String</span></span>|<span data-ttu-id="73437-131">appleVolumePurchaseProgramToken 作成時に自動的に生成されます。</span><span class="sxs-lookup"><span data-stu-id="73437-131">This is automatically generated when the appleVolumePurchaseProgramToken is created.</span></span> <span data-ttu-id="73437-132">エンティティのキーになります。</span><span class="sxs-lookup"><span data-stu-id="73437-132">It is the Key of the entity.</span></span>|
|<span data-ttu-id="73437-133">organizationName</span><span class="sxs-lookup"><span data-stu-id="73437-133">organizationName</span></span>|<span data-ttu-id="73437-134">文字列</span><span class="sxs-lookup"><span data-stu-id="73437-134">String</span></span>|<span data-ttu-id="73437-135">Apple Volume Purchase Program のトークンに関連付けられている組織</span><span class="sxs-lookup"><span data-stu-id="73437-135">The organization associated with the Apple Volume Purchase Program Token</span></span>|
|<span data-ttu-id="73437-136">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="73437-136">vppTokenAccountType</span></span>|[<span data-ttu-id="73437-137">vppTokenAccountType</span><span class="sxs-lookup"><span data-stu-id="73437-137">vppTokenAccountType</span></span>](../resources/intune_shared_vpptokenaccounttype.md)|<span data-ttu-id="73437-138">特定の Apple Volume Purchase Program のトークンが関連付けられている、ボリューム購入プログラムの種類。</span><span class="sxs-lookup"><span data-stu-id="73437-138">The type of volume purchase program which the given Apple Volume Purchase Program Token is associated with.</span></span> <span data-ttu-id="73437-139">可能な値は、`business`、`education` です。</span><span class="sxs-lookup"><span data-stu-id="73437-139">The possible values are:</span></span> <span data-ttu-id="73437-140">可能な値は、`business`、`education` です。</span><span class="sxs-lookup"><span data-stu-id="73437-140">The possible values are:</span></span>|
|<span data-ttu-id="73437-141">appleId</span><span class="sxs-lookup"><span data-stu-id="73437-141">appleId</span></span>|<span data-ttu-id="73437-142">文字列</span><span class="sxs-lookup"><span data-stu-id="73437-142">String</span></span>|<span data-ttu-id="73437-143">特定の Apple Volume Purchase Program のトークンに関連付けられている Apple ID。</span><span class="sxs-lookup"><span data-stu-id="73437-143">The apple Id associated with the given Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="73437-144">expirationDateTime</span><span class="sxs-lookup"><span data-stu-id="73437-144">expirationDateTime</span></span>|<span data-ttu-id="73437-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="73437-145">DateTimeOffset</span></span>|<span data-ttu-id="73437-146">Apple Volume Purchase Program のトークンの有効期限。</span><span class="sxs-lookup"><span data-stu-id="73437-146">The expiration date time of the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="73437-147">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="73437-147">lastSyncDateTime</span></span>|<span data-ttu-id="73437-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="73437-148">DateTimeOffset</span></span>|<span data-ttu-id="73437-149">Apple Volume Purchase Program のトークンを使用して、Apple ボリューム購入プログラム サービスと最後にアプリケーションの同期を行った日時。</span><span class="sxs-lookup"><span data-stu-id="73437-149">The last time when an application sync was done with the Apple volume purchase program service using the the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="73437-150">token</span><span class="sxs-lookup"><span data-stu-id="73437-150">token</span></span>|<span data-ttu-id="73437-151">文字列</span><span class="sxs-lookup"><span data-stu-id="73437-151">String</span></span>|<span data-ttu-id="73437-152">Apple Volume Purchase Program からダウンロードした Apple ボリューム購入プログラムのトークン文字列。</span><span class="sxs-lookup"><span data-stu-id="73437-152">The Apple Volume Purchase Program Token string downloaded from the Apple Volume Purchase Program.</span></span>|
|<span data-ttu-id="73437-153">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="73437-153">lastModifiedDateTime</span></span>|<span data-ttu-id="73437-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="73437-154">DateTimeOffset</span></span>|<span data-ttu-id="73437-155">Apple Volume Purchase Program のトークンに関連付けられている最終変更日時。</span><span class="sxs-lookup"><span data-stu-id="73437-155">Last modification date time associated with the Apple Volume Purchase Program Token.</span></span>|
|<span data-ttu-id="73437-156">状態</span><span class="sxs-lookup"><span data-stu-id="73437-156">state</span></span>|[<span data-ttu-id="73437-157">vppTokenState</span><span class="sxs-lookup"><span data-stu-id="73437-157">vppTokenState</span></span>](../resources/intune_onboarding_vpptokenstate.md)|<span data-ttu-id="73437-158">Apple Volume Purchase Program のトークンの現在の状態。</span><span class="sxs-lookup"><span data-stu-id="73437-158">Current state of the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="73437-159">可能な値は、`unknown`、`valid`、`expired`、`invalid` です。</span><span class="sxs-lookup"><span data-stu-id="73437-159">The possible values are `unknown`, `valid`, `expired`, `invalid`, , , , , , , , or .</span></span> <span data-ttu-id="73437-160">可能な値は、`unknown`、`valid`、`expired`、`invalid` です。</span><span class="sxs-lookup"><span data-stu-id="73437-160">The possible values are `unknown`, `valid`, `expired`, `invalid`, , , , , , , , or .</span></span>|
|<span data-ttu-id="73437-161">lastSyncStatus</span><span class="sxs-lookup"><span data-stu-id="73437-161">lastSyncStatus</span></span>|[<span data-ttu-id="73437-162">vppTokenSyncStatus</span><span class="sxs-lookup"><span data-stu-id="73437-162">vppTokenSyncStatus</span></span>](../resources/intune_onboarding_vpptokensyncstatus.md)|<span data-ttu-id="73437-163">Apple Volume Purchase Program のトークンを使用して行われた最後のアプリケーションの同期の現在の同期状態。</span><span class="sxs-lookup"><span data-stu-id="73437-163">Current sync status of the last application sync which was triggered using the Apple Volume Purchase Program Token.</span></span> <span data-ttu-id="73437-164">可能な値は、`none`、`inProgress`、`completed`、`failed` です。</span><span class="sxs-lookup"><span data-stu-id="73437-164">The possible values are `none`, `inProgress`, `completed`, `failed`, , , , , , , , or .</span></span> <span data-ttu-id="73437-165">可能な値は、`none`、`inProgress`、`completed`、`failed` です。</span><span class="sxs-lookup"><span data-stu-id="73437-165">The possible values are `none`, `inProgress`, `completed`, `failed`, , , , , , , , or .</span></span>|
|<span data-ttu-id="73437-166">automaticallyUpdateApps</span><span class="sxs-lookup"><span data-stu-id="73437-166">automaticallyUpdateApps</span></span>|<span data-ttu-id="73437-167">ブール型</span><span class="sxs-lookup"><span data-stu-id="73437-167">Boolean</span></span>|<span data-ttu-id="73437-168">VPP トークンのアプリを自動で更新するかどうか。</span><span class="sxs-lookup"><span data-stu-id="73437-168">Whether or not apps for the VPP token will be automatically updated.</span></span>|
|<span data-ttu-id="73437-169">countryOrRegion</span><span class="sxs-lookup"><span data-stu-id="73437-169">countryOrRegion</span></span>|<span data-ttu-id="73437-170">文字列</span><span class="sxs-lookup"><span data-stu-id="73437-170">String</span></span>|<span data-ttu-id="73437-171">VPP トークンのアプリを自動で更新するかどうか。</span><span class="sxs-lookup"><span data-stu-id="73437-171">Whether or not apps for the VPP token will be automatically updated.</span></span>|



## <a name="response"></a><span data-ttu-id="73437-172">応答</span><span class="sxs-lookup"><span data-stu-id="73437-172">Response</span></span>
<span data-ttu-id="73437-173">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [vppToken](../resources/intune_onboarding_vpptoken.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="73437-173">If successful, this method returns a `201 Created` response code and a [vppToken](../resources/intune_onboarding_vpptoken.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="73437-174">例</span><span class="sxs-lookup"><span data-stu-id="73437-174">Example</span></span>
### <a name="request"></a><span data-ttu-id="73437-175">要求</span><span class="sxs-lookup"><span data-stu-id="73437-175">Request</span></span>
<span data-ttu-id="73437-176">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="73437-176">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/vppTokens
Content-type: application/json
Content-length: 525

{
  "@odata.type": "#microsoft.graph.vppToken",
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

### <a name="response"></a><span data-ttu-id="73437-177">応答</span><span class="sxs-lookup"><span data-stu-id="73437-177">Response</span></span>
<span data-ttu-id="73437-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="73437-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



