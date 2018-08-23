# <a name="update-deviceappmanagement"></a><span data-ttu-id="3b0ec-101">Update deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="3b0ec-101">Update deviceAppManagement</span></span>

> <span data-ttu-id="3b0ec-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="3b0ec-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3b0ec-103">[deviceAppManagement](../resources/intune_shared_deviceappmanagement.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="3b0ec-103">Update the properties of a [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3b0ec-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="3b0ec-104">Prerequisites</span></span>
<span data-ttu-id="3b0ec-105">この API を呼び出すには次のアクセス許可のいずれかが必要です。</span><span class="sxs-lookup"><span data-stu-id="3b0ec-105">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see Permissions.</span></span> <span data-ttu-id="3b0ec-106">アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3b0ec-106">To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>  <span data-ttu-id="3b0ec-107">ワークフローに従って、適切なアクセス許可が異なることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="3b0ec-107">Note that the appropriate permission varies according to the workflow.</span></span>

|<span data-ttu-id="3b0ec-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3b0ec-108">Permission type</span></span>|<span data-ttu-id="3b0ec-109">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="3b0ec-109">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3b0ec-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3b0ec-110">Delegated (work or school account)</span></span>|<span data-ttu-id="3b0ec-111">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3b0ec-111">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3b0ec-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3b0ec-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3b0ec-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3b0ec-113">Not supported.</span></span>|
|<span data-ttu-id="3b0ec-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3b0ec-114">Application</span></span>|<span data-ttu-id="3b0ec-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3b0ec-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3b0ec-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3b0ec-116">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement
```

## <a name="request-headers"></a><span data-ttu-id="3b0ec-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3b0ec-117">Request headers</span></span>
|<span data-ttu-id="3b0ec-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3b0ec-118">Header</span></span>|<span data-ttu-id="3b0ec-119">値</span><span class="sxs-lookup"><span data-stu-id="3b0ec-119">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3b0ec-120">承認</span><span class="sxs-lookup"><span data-stu-id="3b0ec-120">Authorization</span></span>|<span data-ttu-id="3b0ec-121">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="3b0ec-121">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3b0ec-122">受け入れ</span><span class="sxs-lookup"><span data-stu-id="3b0ec-122">Accept</span></span>|<span data-ttu-id="3b0ec-123">アプリケーション /json</span><span class="sxs-lookup"><span data-stu-id="3b0ec-123">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3b0ec-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="3b0ec-124">Request body</span></span>
<span data-ttu-id="3b0ec-125">要求本文で、[deviceAppManagement](../resources/intune_shared_deviceappmanagement.md) オブジェクトの JSON 表記を提供します。</span><span class="sxs-lookup"><span data-stu-id="3b0ec-125">In the request body, supply a JSON representation for the [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md) object.</span></span>

<span data-ttu-id="3b0ec-126">次の表に、[deviceAppManagement](../resources/intune_shared_deviceappmanagement.md) 作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="3b0ec-126">The following table shows the properties that are required when you create the [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md).</span></span>

|<span data-ttu-id="3b0ec-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3b0ec-127">Property</span></span>|<span data-ttu-id="3b0ec-128">型</span><span class="sxs-lookup"><span data-stu-id="3b0ec-128">Type</span></span>|<span data-ttu-id="3b0ec-129">説明</span><span class="sxs-lookup"><span data-stu-id="3b0ec-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3b0ec-130">id</span><span class="sxs-lookup"><span data-stu-id="3b0ec-130">id</span></span>|<span data-ttu-id="3b0ec-131">文字列</span><span class="sxs-lookup"><span data-stu-id="3b0ec-131">String</span></span>|<span data-ttu-id="3b0ec-132">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="3b0ec-132">Key of the entity.</span></span>|
|<span data-ttu-id="3b0ec-133">**採用**</span><span class="sxs-lookup"><span data-stu-id="3b0ec-133">**On-boarding**</span></span>|
|<span data-ttu-id="3b0ec-134">isEnabledForMicrosoftStoreForBusiness</span><span class="sxs-lookup"><span data-stu-id="3b0ec-134">isEnabledForMicrosoftStoreForBusiness</span></span>|<span data-ttu-id="3b0ec-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="3b0ec-135">Boolean</span></span>|<span data-ttu-id="3b0ec-136">アカウントと、ビジネス向け Microsoft Store からのアプリケーションとの同期が有効にされているかどうか。</span><span class="sxs-lookup"><span data-stu-id="3b0ec-136">Whether the account is enabled for syncing applications from the Microsoft Store for Business.</span></span>|
|<span data-ttu-id="3b0ec-137">microsoftStoreForBusinessLanguage</span><span class="sxs-lookup"><span data-stu-id="3b0ec-137">microsoftStoreForBusinessLanguage</span></span>|<span data-ttu-id="3b0ec-138">文字列</span><span class="sxs-lookup"><span data-stu-id="3b0ec-138">String</span></span>|<span data-ttu-id="3b0ec-139">ビジネス向け Microsoft Store からのアプリケーションの同期に使用されたロケール情報。</span><span class="sxs-lookup"><span data-stu-id="3b0ec-139">The locale information used to sync applications from the Microsoft Store for Business.</span></span> <span data-ttu-id="3b0ec-140">国/地域固有のカルチャ。</span><span class="sxs-lookup"><span data-stu-id="3b0ec-140">Cultures that are specific to a country/region.</span></span> <span data-ttu-id="3b0ec-141">カルチャの名前は RFC 4646 に準拠します (Windows Vista 以降)。</span><span class="sxs-lookup"><span data-stu-id="3b0ec-141">The names of these cultures follow RFC 4646 (Windows Vista and later).</span></span> <span data-ttu-id="3b0ec-142">形式の <languagecode2>-<country/regioncode2> は<languagecode2>  ISO 639-1 に基づく小文字 2 文字のコードで、<country/regioncode2> は ISO 3166 に基づく大文字 2 文字のコードです。</span><span class="sxs-lookup"><span data-stu-id="3b0ec-142">The format is <languagecode2>-<country/regioncode2>, where <languagecode2> is a lowercase two-letter code derived from ISO 639-1 and <country/regioncode2> is an uppercase two-letter code derived from ISO 3166.</span></span> <span data-ttu-id="3b0ec-143">たとえば、英語 (米国) 固有のカルチャは en-US です。</span><span class="sxs-lookup"><span data-stu-id="3b0ec-143">For example, en-US for English (United States) is a specific culture.</span></span>|
|<span data-ttu-id="3b0ec-144">microsoftStoreForBusinessLastCompletedApplicationSyncTime</span><span class="sxs-lookup"><span data-stu-id="3b0ec-144">microsoftStoreForBusinessLastCompletedApplicationSyncTime</span></span>|<span data-ttu-id="3b0ec-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3b0ec-145">DateTimeOffset</span></span>|<span data-ttu-id="3b0ec-146">ビジネス向け Microsoft Store からのアプリケーション同期が最後に実行された日時。</span><span class="sxs-lookup"><span data-stu-id="3b0ec-146">The last time an application sync from the Microsoft Store for Business was completed.</span></span>|
|<span data-ttu-id="3b0ec-147">microsoftStoreForBusinessLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="3b0ec-147">microsoftStoreForBusinessLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="3b0ec-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3b0ec-148">DateTimeOffset</span></span>|<span data-ttu-id="3b0ec-149">ビジネス向け Microsoft Store のアプリがアカウントに正常に同期された最終日時。</span><span class="sxs-lookup"><span data-stu-id="3b0ec-149">The last time the apps from the Microsoft Store for Business were synced successfully for the account.</span></span>|

## <a name="response"></a><span data-ttu-id="3b0ec-150">応答</span><span class="sxs-lookup"><span data-stu-id="3b0ec-150">Response</span></span>
<span data-ttu-id="3b0ec-151">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="3b0ec-151">If successful, this method returns a `200 OK` response code and an updated [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3b0ec-152">例</span><span class="sxs-lookup"><span data-stu-id="3b0ec-152">Example</span></span>
### <a name="request"></a><span data-ttu-id="3b0ec-153">要求</span><span class="sxs-lookup"><span data-stu-id="3b0ec-153">Request</span></span>
<span data-ttu-id="3b0ec-154">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3b0ec-154">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="3b0ec-155">応答</span><span class="sxs-lookup"><span data-stu-id="3b0ec-155">Response</span></span>
<span data-ttu-id="3b0ec-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3b0ec-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 110

{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "bbb801a3-01a3-bbb8-a301-b8bba301b8bb"
}
```



