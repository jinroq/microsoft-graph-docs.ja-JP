# <a name="update-androidforworksettings"></a><span data-ttu-id="535e8-101">Update androidForWorkSettings</span><span class="sxs-lookup"><span data-stu-id="535e8-101">Update androidForWorkSettings</span></span>

> <span data-ttu-id="535e8-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="535e8-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="535e8-103">[androidForWorkSettings](../resources/intune_androidforwork_androidforworksettings.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="535e8-103">Update the properties of a [calendar](../resources/intune_androidforwork_androidforworksettings.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="535e8-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="535e8-104">Prerequisites</span></span>
<span data-ttu-id="535e8-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="535e8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="535e8-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="535e8-107">Permission type</span></span>|<span data-ttu-id="535e8-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="535e8-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="535e8-109">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="535e8-109">Delegated (work or school account)</span></span>|<span data-ttu-id="535e8-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="535e8-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="535e8-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="535e8-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="535e8-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="535e8-112">Not supported.</span></span>|
|<span data-ttu-id="535e8-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="535e8-113">Application</span></span>|<span data-ttu-id="535e8-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="535e8-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="535e8-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="535e8-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/androidForWorkSettings
```

## <a name="request-headers"></a><span data-ttu-id="535e8-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="535e8-116">Request headers</span></span>
|<span data-ttu-id="535e8-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="535e8-117">Header</span></span>|<span data-ttu-id="535e8-118">値</span><span class="sxs-lookup"><span data-stu-id="535e8-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="535e8-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="535e8-119">Authorization</span></span>|<span data-ttu-id="535e8-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="535e8-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="535e8-121">Accept</span><span class="sxs-lookup"><span data-stu-id="535e8-121">Accept</span></span>|<span data-ttu-id="535e8-122">application/json</span><span class="sxs-lookup"><span data-stu-id="535e8-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="535e8-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="535e8-123">Request body</span></span>
<span data-ttu-id="535e8-124">要求本文で、[androidForWorkSettings](../resources/intune_androidforwork_androidforworksettings.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="535e8-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_androidforwork_androidforworksettings.md) object.</span></span>

<span data-ttu-id="535e8-125">次の表に、[androidForWorkSettings](../resources/intune_androidforwork_androidforworksettings.md) 作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="535e8-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="535e8-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="535e8-126">Property</span></span>|<span data-ttu-id="535e8-127">型</span><span class="sxs-lookup"><span data-stu-id="535e8-127">Type</span></span>|<span data-ttu-id="535e8-128">説明</span><span class="sxs-lookup"><span data-stu-id="535e8-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="535e8-129">id</span><span class="sxs-lookup"><span data-stu-id="535e8-129">id</span></span>|<span data-ttu-id="535e8-130">String</span><span class="sxs-lookup"><span data-stu-id="535e8-130">String</span></span>|<span data-ttu-id="535e8-131">Android for Work 設定の識別子</span><span class="sxs-lookup"><span data-stu-id="535e8-131">The Android for Work settings identifier</span></span>|
|<span data-ttu-id="535e8-132">bindStatus</span><span class="sxs-lookup"><span data-stu-id="535e8-132">bindStatus</span></span>|<span data-ttu-id="535e8-133">String</span><span class="sxs-lookup"><span data-stu-id="535e8-133">String</span></span>|<span data-ttu-id="535e8-134">Google EMM API を使ったテナントのバインド状態。可能な値は、`notBound`、`bound`、`boundAndValidated`、`unbinding` です。</span><span class="sxs-lookup"><span data-stu-id="535e8-134">Bind status of the tenant with the Google EMM API Possible values are: `notBound`, `bound`, `boundAndValidated`, `unbinding`.</span></span>|
|<span data-ttu-id="535e8-135">lastAppSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="535e8-135">lastAppSyncDateTime</span></span>|<span data-ttu-id="535e8-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="535e8-136">DateTimeOffset</span></span>|<span data-ttu-id="535e8-137">アプリ同期の最終完了時刻</span><span class="sxs-lookup"><span data-stu-id="535e8-137">Last completion time for app sync</span></span>|
|<span data-ttu-id="535e8-138">lastAppSyncStatus</span><span class="sxs-lookup"><span data-stu-id="535e8-138">lastAppSyncStatus</span></span>|<span data-ttu-id="535e8-139">String</span><span class="sxs-lookup"><span data-stu-id="535e8-139">String</span></span>|<span data-ttu-id="535e8-140">前回のアプリケーション同期の結果。可能な値は、`success`、`credentialsNotValid`、`androidForWorkApiError`、`managementServiceError`、`unknownError`、`none` です。</span><span class="sxs-lookup"><span data-stu-id="535e8-140">Last application sync result Possible values are: `success`, `credentialsNotValid`, `androidForWorkApiError`, `managementServiceError`, `unknownError`, `none`.</span></span>|
|<span data-ttu-id="535e8-141">ownerUserPrincipalName</span><span class="sxs-lookup"><span data-stu-id="535e8-141">ownerUserPrincipalName</span></span>|<span data-ttu-id="535e8-142">String</span><span class="sxs-lookup"><span data-stu-id="535e8-142">String</span></span>|<span data-ttu-id="535e8-143">エンタープライズを作成した所有者 UPN</span><span class="sxs-lookup"><span data-stu-id="535e8-143">Owner UPN that created the enterprise</span></span>|
|<span data-ttu-id="535e8-144">ownerOrganizationName</span><span class="sxs-lookup"><span data-stu-id="535e8-144">ownerOrganizationName</span></span>|<span data-ttu-id="535e8-145">String</span><span class="sxs-lookup"><span data-stu-id="535e8-145">String</span></span>|<span data-ttu-id="535e8-146">Android for Work の配布準備時に使用される組織名</span><span class="sxs-lookup"><span data-stu-id="535e8-146">Organization name used when onboarding Android for Work</span></span>|
|<span data-ttu-id="535e8-147">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="535e8-147">lastModifiedDateTime</span></span>|<span data-ttu-id="535e8-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="535e8-148">DateTimeOffset</span></span>|<span data-ttu-id="535e8-149">Android for Work 設定の最終変更時刻</span><span class="sxs-lookup"><span data-stu-id="535e8-149">Last modification time for Android for Work settings</span></span>|
|<span data-ttu-id="535e8-150">enrollmentTarget</span><span class="sxs-lookup"><span data-stu-id="535e8-150">enrollmentTarget</span></span>|<span data-ttu-id="535e8-151">String</span><span class="sxs-lookup"><span data-stu-id="535e8-151">String</span></span>|<span data-ttu-id="535e8-152">どのユーザーが Android for Work デバイス管理にデバイスを登録できるかを示します。可能な値は、`none`、`all`、`targeted`、`targetedAsEnrollmentRestrictions` です。</span><span class="sxs-lookup"><span data-stu-id="535e8-152">Indicates which users can enroll devices in Android for Work device management Possible values are: `none`, `all`, `targeted`, `targetedAsEnrollmentRestrictions`.</span></span>|
|<span data-ttu-id="535e8-153">targetGroupIds</span><span class="sxs-lookup"><span data-stu-id="535e8-153">targetGroupIds</span></span>|<span data-ttu-id="535e8-154">String コレクション</span><span class="sxs-lookup"><span data-stu-id="535e8-154">String collection</span></span>|<span data-ttu-id="535e8-155">enrollmentTarget が 'Targeted' に設定されている場合、どの AAD グループが Android for Work デバイス管理にデバイスを登録できるかを指定します。</span><span class="sxs-lookup"><span data-stu-id="535e8-155">Specifies which AAD groups can enroll devices in Android for Work device management if enrollmentTarget is set to 'Targeted'</span></span>|



## <a name="response"></a><span data-ttu-id="535e8-156">応答</span><span class="sxs-lookup"><span data-stu-id="535e8-156">Response</span></span>
<span data-ttu-id="535e8-157">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [androidForWorkSettings](../resources/intune_androidforwork_androidforworksettings.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="535e8-157">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_androidforwork_androidforworksettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="535e8-158">例</span><span class="sxs-lookup"><span data-stu-id="535e8-158">Example</span></span>
### <a name="request"></a><span data-ttu-id="535e8-159">要求</span><span class="sxs-lookup"><span data-stu-id="535e8-159">Request</span></span>
<span data-ttu-id="535e8-160">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="535e8-160">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/androidForWorkSettings
Content-type: application/json
Content-length: 417

{
  "bindStatus": "bound",
  "lastAppSyncDateTime": "2016-12-31T23:57:22.8606813-08:00",
  "lastAppSyncStatus": "credentialsNotValid",
  "ownerUserPrincipalName": "Owner User Principal Name value",
  "ownerOrganizationName": "Owner Organization Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "enrollmentTarget": "all",
  "targetGroupIds": [
    "Target Group Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="535e8-161">応答</span><span class="sxs-lookup"><span data-stu-id="535e8-161">Response</span></span>
<span data-ttu-id="535e8-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="535e8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 527

{
  "@odata.type": "#microsoft.graph.androidForWorkSettings",
  "id": "97adc169-c169-97ad-69c1-ad9769c1ad97",
  "bindStatus": "bound",
  "lastAppSyncDateTime": "2016-12-31T23:57:22.8606813-08:00",
  "lastAppSyncStatus": "credentialsNotValid",
  "ownerUserPrincipalName": "Owner User Principal Name value",
  "ownerOrganizationName": "Owner Organization Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "enrollmentTarget": "all",
  "targetGroupIds": [
    "Target Group Ids value"
  ]
}
```



