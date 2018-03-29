# <a name="update-deviceappmanagement"></a><span data-ttu-id="e4a3e-101">Update deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="e4a3e-101">Update deviceAppManagement</span></span>

> <span data-ttu-id="e4a3e-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e4a3e-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e4a3e-103">[deviceAppManagement](../resources/intune_onboarding_deviceappmanagement.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="e4a3e-103">Update the properties of a [calendar](../resources/intune_onboarding_deviceappmanagement.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e4a3e-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="e4a3e-104">Prerequisites</span></span>
<span data-ttu-id="e4a3e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e4a3e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e4a3e-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e4a3e-107">Permission type</span></span>|<span data-ttu-id="e4a3e-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="e4a3e-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e4a3e-109">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="e4a3e-109">Delegated (work or school account)</span></span>|<span data-ttu-id="e4a3e-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4a3e-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e4a3e-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e4a3e-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e4a3e-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e4a3e-112">Not supported.</span></span>|
|<span data-ttu-id="e4a3e-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e4a3e-113">Application</span></span>|<span data-ttu-id="e4a3e-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e4a3e-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e4a3e-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e4a3e-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement
```

## <a name="request-headers"></a><span data-ttu-id="e4a3e-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e4a3e-116">Request headers</span></span>
|<span data-ttu-id="e4a3e-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e4a3e-117">Header</span></span>|<span data-ttu-id="e4a3e-118">値</span><span class="sxs-lookup"><span data-stu-id="e4a3e-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e4a3e-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="e4a3e-119">Authorization</span></span>|<span data-ttu-id="e4a3e-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="e4a3e-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="e4a3e-121">Accept</span><span class="sxs-lookup"><span data-stu-id="e4a3e-121">Accept</span></span>|<span data-ttu-id="e4a3e-122">application/json</span><span class="sxs-lookup"><span data-stu-id="e4a3e-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e4a3e-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="e4a3e-123">Request body</span></span>
<span data-ttu-id="e4a3e-124">要求本文で、[deviceAppManagement](../resources/intune_onboarding_deviceappmanagement.md) オブジェクトの JSON 表記を提供します。</span><span class="sxs-lookup"><span data-stu-id="e4a3e-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_onboarding_deviceappmanagement.md) object.</span></span>

<span data-ttu-id="e4a3e-125">次の表に、[deviceAppManagement](../resources/intune_onboarding_deviceappmanagement.md) 作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="e4a3e-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="e4a3e-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e4a3e-126">Property</span></span>|<span data-ttu-id="e4a3e-127">型</span><span class="sxs-lookup"><span data-stu-id="e4a3e-127">Type</span></span>|<span data-ttu-id="e4a3e-128">説明</span><span class="sxs-lookup"><span data-stu-id="e4a3e-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4a3e-129">id</span><span class="sxs-lookup"><span data-stu-id="e4a3e-129">id</span></span>|<span data-ttu-id="e4a3e-130">String</span><span class="sxs-lookup"><span data-stu-id="e4a3e-130">String</span></span>|<span data-ttu-id="e4a3e-131">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="e4a3e-131">Not yet documented</span></span>|
|<span data-ttu-id="e4a3e-132">microsoftStoreForBusinessLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="e4a3e-132">microsoftStoreForBusinessLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="e4a3e-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e4a3e-133">DateTimeOffset</span></span>|<span data-ttu-id="e4a3e-134">Microsoft Store for Business のアプリがアカウントに正常に同期された最終日時。</span><span class="sxs-lookup"><span data-stu-id="e4a3e-134">The last time the apps from the Microsoft Store for Business were synced successfully for the account.</span></span>|
|<span data-ttu-id="e4a3e-135">isEnabledForMicrosoftStoreForBusiness</span><span class="sxs-lookup"><span data-stu-id="e4a3e-135">isEnabledForMicrosoftStoreForBusiness</span></span>|<span data-ttu-id="e4a3e-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="e4a3e-136">Boolean</span></span>|<span data-ttu-id="e4a3e-137">アカウントと、ビジネス向け Microsoft Store からのアプリケーションとの同期が有効にされているかどうか。</span><span class="sxs-lookup"><span data-stu-id="e4a3e-137">Whether the account is enabled for syncing applications from the Microsoft Store for Business.</span></span>|
|<span data-ttu-id="e4a3e-138">microsoftStoreForBusinessLanguage</span><span class="sxs-lookup"><span data-stu-id="e4a3e-138">microsoftStoreForBusinessLanguage</span></span>|<span data-ttu-id="e4a3e-139">String</span><span class="sxs-lookup"><span data-stu-id="e4a3e-139">String</span></span>|<span data-ttu-id="e4a3e-140">ビジネス向け Microsoft Store からのアプリケーションの同期に使用されたロケール情報。</span><span class="sxs-lookup"><span data-stu-id="e4a3e-140">The locale information used to sync applications from the Microsoft Store for Business.</span></span> <span data-ttu-id="e4a3e-141">国/地域固有のカルチャ。</span><span class="sxs-lookup"><span data-stu-id="e4a3e-141">Cultures that are specific to a country/region.</span></span> <span data-ttu-id="e4a3e-142">カルチャの名前は RFC 4646 に準拠します (Windows Vista 以降)。</span><span class="sxs-lookup"><span data-stu-id="e4a3e-142">The names of these cultures follow RFC 4646 (Windows Vista and later).</span></span> <span data-ttu-id="e4a3e-143">形式は <languagecode2>-<country/regioncode2> です。<languagecode2> は ISO 639-1 に基づく小文字 2 文字で構成されるコードで、<country/regioncode2> は ISO 3166 の基づく大文字 2 文字で構成されるコードです。</span><span class="sxs-lookup"><span data-stu-id="e4a3e-143">The format is <languagecode2>-<country/regioncode2>, where <languagecode2> is a lowercase two-letter code derived from ISO 639-1 and <country/regioncode2> is an uppercase two-letter code derived from ISO 3166.</span></span> <span data-ttu-id="e4a3e-144">たとえば、英語 (米国) 固有のカルチャは en-US です。</span><span class="sxs-lookup"><span data-stu-id="e4a3e-144">For example, en-US for English (United States) is a specific culture.</span></span>|
|<span data-ttu-id="e4a3e-145">microsoftStoreForBusinessLastCompletedApplicationSyncTime</span><span class="sxs-lookup"><span data-stu-id="e4a3e-145">microsoftStoreForBusinessLastCompletedApplicationSyncTime</span></span>|<span data-ttu-id="e4a3e-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e4a3e-146">DateTimeOffset</span></span>|<span data-ttu-id="e4a3e-147">ビジネス向け Microsoft Store からのアプリケーションの同期が最後に実行された日時。</span><span class="sxs-lookup"><span data-stu-id="e4a3e-147">The last time an application sync from the Microsoft Store for Business was completed.</span></span>|



## <a name="response"></a><span data-ttu-id="e4a3e-148">応答</span><span class="sxs-lookup"><span data-stu-id="e4a3e-148">Response</span></span>
<span data-ttu-id="e4a3e-149">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [deviceAppManagement](../resources/intune_onboarding_deviceappmanagement.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e4a3e-149">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_onboarding_deviceappmanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e4a3e-150">例</span><span class="sxs-lookup"><span data-stu-id="e4a3e-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="e4a3e-151">要求</span><span class="sxs-lookup"><span data-stu-id="e4a3e-151">Request</span></span>
<span data-ttu-id="e4a3e-152">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e4a3e-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement
Content-type: application/json
Content-length: 336

{
  "microsoftStoreForBusinessLastSuccessfulSyncDateTime": "2016-12-31T23:57:45.2453148-08:00",
  "isEnabledForMicrosoftStoreForBusiness": true,
  "microsoftStoreForBusinessLanguage": "Microsoft Store For Business Language value",
  "microsoftStoreForBusinessLastCompletedApplicationSyncTime": "2017-01-01T00:02:00.0421137-08:00"
}
```

### <a name="response"></a><span data-ttu-id="e4a3e-153">応答</span><span class="sxs-lookup"><span data-stu-id="e4a3e-153">Response</span></span>
<span data-ttu-id="e4a3e-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e4a3e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 443

{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "bbb801a3-01a3-bbb8-a301-b8bba301b8bb",
  "microsoftStoreForBusinessLastSuccessfulSyncDateTime": "2016-12-31T23:57:45.2453148-08:00",
  "isEnabledForMicrosoftStoreForBusiness": true,
  "microsoftStoreForBusinessLanguage": "Microsoft Store For Business Language value",
  "microsoftStoreForBusinessLastCompletedApplicationSyncTime": "2017-01-01T00:02:00.0421137-08:00"
}
```



