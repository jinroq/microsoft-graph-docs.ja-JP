# <a name="update-deviceappmanagement"></a><span data-ttu-id="66c15-101">Update deviceAppManagement</span><span class="sxs-lookup"><span data-stu-id="66c15-101">Update deviceAppManagement</span></span>

> <span data-ttu-id="66c15-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="66c15-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="66c15-103">[deviceAppManagement](../resources/intune_shared_deviceappmanagement.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="66c15-103">Update the properties of a [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="66c15-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="66c15-104">Prerequisites</span></span>
<span data-ttu-id="66c15-105">この API を呼び出すには次のアクセス許可のいずれかが必要です。</span><span class="sxs-lookup"><span data-stu-id="66c15-105">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="66c15-106">アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="66c15-106">To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>  <span data-ttu-id="66c15-107">ワークフローに従って、適切なアクセス許可が異なることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="66c15-107">Note that the appropriate permission varies according to the workflow.</span></span>

|<span data-ttu-id="66c15-108">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="66c15-108">Permission type</span></span>|<span data-ttu-id="66c15-109">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="66c15-109">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="66c15-110">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="66c15-110">Delegated (work or school account)</span></span>|<span data-ttu-id="66c15-111">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66c15-111">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="66c15-112">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="66c15-112">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="66c15-113">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="66c15-113">Not supported.</span></span>|
|<span data-ttu-id="66c15-114">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="66c15-114">Application</span></span>|<span data-ttu-id="66c15-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="66c15-115">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="66c15-116">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="66c15-116">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement
```

## <a name="request-headers"></a><span data-ttu-id="66c15-117">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="66c15-117">Request headers</span></span>
|<span data-ttu-id="66c15-118">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="66c15-118">Header</span></span>|<span data-ttu-id="66c15-119">値</span><span class="sxs-lookup"><span data-stu-id="66c15-119">Value</span></span>|
|:---|:---|
|<span data-ttu-id="66c15-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="66c15-120">Authorization</span></span>|<span data-ttu-id="66c15-121">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="66c15-121">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="66c15-122">Accept</span><span class="sxs-lookup"><span data-stu-id="66c15-122">Accept</span></span>|<span data-ttu-id="66c15-123">application/json</span><span class="sxs-lookup"><span data-stu-id="66c15-123">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="66c15-124">要求本文</span><span class="sxs-lookup"><span data-stu-id="66c15-124">Request body</span></span>
<span data-ttu-id="66c15-125">要求本文で、[deviceAppManagement](../resources/intune_shared_deviceappmanagement.md) オブジェクトの JSON 表記を提供します。</span><span class="sxs-lookup"><span data-stu-id="66c15-125">In the request body, supply a JSON representation for the [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md) object.</span></span>

<span data-ttu-id="66c15-126">次の表に、[deviceAppManagement](../resources/intune_shared_deviceappmanagement.md) 作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="66c15-126">The following table shows the properties that are required when you create the [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md).</span></span>

|<span data-ttu-id="66c15-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="66c15-127">Property</span></span>|<span data-ttu-id="66c15-128">型</span><span class="sxs-lookup"><span data-stu-id="66c15-128">Type</span></span>|<span data-ttu-id="66c15-129">説明</span><span class="sxs-lookup"><span data-stu-id="66c15-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="66c15-130">id</span><span class="sxs-lookup"><span data-stu-id="66c15-130">id</span></span>|<span data-ttu-id="66c15-131">String</span><span class="sxs-lookup"><span data-stu-id="66c15-131">String</span></span>|<span data-ttu-id="66c15-132">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="66c15-132">Key of the entity.</span></span>|
|<span data-ttu-id="66c15-133">**契約時**</span><span class="sxs-lookup"><span data-stu-id="66c15-133">**Onboarding**</span></span>|
|<span data-ttu-id="66c15-134">isEnabledForMicrosoftStoreForBusiness</span><span class="sxs-lookup"><span data-stu-id="66c15-134">isEnabledForMicrosoftStoreForBusiness</span></span>|<span data-ttu-id="66c15-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="66c15-135">Boolean</span></span>|<span data-ttu-id="66c15-136">アカウントと、ビジネス向け Microsoft Store からのアプリケーションとの同期が有効にされているかどうか。</span><span class="sxs-lookup"><span data-stu-id="66c15-136">Whether the account is enabled for syncing applications from the Microsoft Store for Business.</span></span>|
|<span data-ttu-id="66c15-137">microsoftStoreForBusinessLanguage</span><span class="sxs-lookup"><span data-stu-id="66c15-137">microsoftStoreForBusinessLanguage</span></span>|<span data-ttu-id="66c15-138">String</span><span class="sxs-lookup"><span data-stu-id="66c15-138">String</span></span>|<span data-ttu-id="66c15-139">ビジネス向け Microsoft Store からのアプリケーションの同期に使用されたロケール情報。</span><span class="sxs-lookup"><span data-stu-id="66c15-139">The locale information used to sync applications from the Microsoft Store for Business.</span></span> <span data-ttu-id="66c15-140">国/地域固有のカルチャ。</span><span class="sxs-lookup"><span data-stu-id="66c15-140">Cultures that are specific to a country/region.</span></span> <span data-ttu-id="66c15-141">カルチャの名前は RFC 4646 に準拠します (Windows Vista 以降)。</span><span class="sxs-lookup"><span data-stu-id="66c15-141">The names of these cultures follow RFC 4646 (Windows Vista and later).</span></span> <span data-ttu-id="66c15-142">形式の <languagecode2>-<country/regioncode2> は<languagecode2>  ISO 639-1 に基づく小文字 2 文字のコードで、<country/regioncode2> は ISO 3166 に基づく大文字 2 文字のコードです。</span><span class="sxs-lookup"><span data-stu-id="66c15-142">The format is <languagecode2>-<country/regioncode2>, where <languagecode2> is a lowercase two-letter code derived from ISO 639-1 and <country/regioncode2> is an uppercase two-letter code derived from ISO 3166.</span></span> <span data-ttu-id="66c15-143">たとえば、英語 (米国) 固有のカルチャは en-US です。</span><span class="sxs-lookup"><span data-stu-id="66c15-143">For example, en-US for English (United States) is a specific culture.</span></span>|
|<span data-ttu-id="66c15-144">microsoftStoreForBusinessLastCompletedApplicationSyncTime</span><span class="sxs-lookup"><span data-stu-id="66c15-144">microsoftStoreForBusinessLastCompletedApplicationSyncTime</span></span>|<span data-ttu-id="66c15-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="66c15-145">DateTimeOffset</span></span>|<span data-ttu-id="66c15-146">ビジネス向け Microsoft Store からのアプリケーション同期が最後に実行された日時。</span><span class="sxs-lookup"><span data-stu-id="66c15-146">The last time an application sync from the Microsoft Store for Business was completed.</span></span>|
|<span data-ttu-id="66c15-147">microsoftStoreForBusinessLastSuccessfulSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="66c15-147">microsoftStoreForBusinessLastSuccessfulSyncDateTime</span></span>|<span data-ttu-id="66c15-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="66c15-148">DateTimeOffset</span></span>|<span data-ttu-id="66c15-149">ビジネス向け Microsoft Store のアプリがアカウントに正常に同期された最終日時。</span><span class="sxs-lookup"><span data-stu-id="66c15-149">The last time the apps from the Microsoft Store for Business were synced successfully for the account.</span></span>|

## <a name="response"></a><span data-ttu-id="66c15-150">応答</span><span class="sxs-lookup"><span data-stu-id="66c15-150">Response</span></span>
<span data-ttu-id="66c15-151">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="66c15-151">If successful, this method returns a `200 OK` response code and an updated [deviceAppManagement](../resources/intune_shared_deviceappmanagement.md) object in the response body.</span></span>

## <a name="example-request"></a><span data-ttu-id="66c15-152">要求の例</span><span class="sxs-lookup"><span data-stu-id="66c15-152">Example request</span></span>

``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement
Content-type: application/json
Content-length: 2

{}
```

## <a name="example-response"></a><span data-ttu-id="66c15-153">応答の例</span><span class="sxs-lookup"><span data-stu-id="66c15-153">Example response</span></span>

<span data-ttu-id="66c15-154">ここに示す応答オブジェクトは、簡潔にするために切り詰められます。</span><span class="sxs-lookup"><span data-stu-id="66c15-154">The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="66c15-155">実際の呼び出しではすべてのプロパティが返されます。</span><span class="sxs-lookup"><span data-stu-id="66c15-155">All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 110

{
  "@odata.type": "#microsoft.graph.deviceAppManagement",
  "id": "bbb801a3-01a3-bbb8-a301-b8bba301b8bb"
}
```



