# <a name="create-mobileappcontentfile"></a><span data-ttu-id="2e7d5-101">mobileAppContentFile の作成</span><span class="sxs-lookup"><span data-stu-id="2e7d5-101">Create mobileAppContentFile</span></span>

> <span data-ttu-id="2e7d5-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="2e7d5-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2e7d5-103">新しい [mobileAppContentFile](../resources/intune_apps_mobileappcontentfile.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="2e7d5-103">Create a new [mobileAppContentFile](../resources/intune_apps_mobileappcontentfile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2e7d5-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="2e7d5-104">Prerequisites</span></span>
<span data-ttu-id="2e7d5-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2e7d5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2e7d5-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2e7d5-107">Permission type</span></span>|<span data-ttu-id="2e7d5-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="2e7d5-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2e7d5-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2e7d5-109">Delegated (work or school account)</span></span>|<span data-ttu-id="2e7d5-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2e7d5-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2e7d5-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2e7d5-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2e7d5-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2e7d5-112">Not supported.</span></span>|
|<span data-ttu-id="2e7d5-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2e7d5-113">Application</span></span>|<span data-ttu-id="2e7d5-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2e7d5-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2e7d5-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2e7d5-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files
```

## <a name="request-headers"></a><span data-ttu-id="2e7d5-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2e7d5-116">Request headers</span></span>
|<span data-ttu-id="2e7d5-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2e7d5-117">Header</span></span>|<span data-ttu-id="2e7d5-118">値</span><span class="sxs-lookup"><span data-stu-id="2e7d5-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2e7d5-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="2e7d5-119">Authorization</span></span>|<span data-ttu-id="2e7d5-120">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="2e7d5-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2e7d5-121">Accept</span><span class="sxs-lookup"><span data-stu-id="2e7d5-121">Accept</span></span>|<span data-ttu-id="2e7d5-122">application/json</span><span class="sxs-lookup"><span data-stu-id="2e7d5-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2e7d5-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="2e7d5-123">Request body</span></span>
<span data-ttu-id="2e7d5-124">要求本文で、mobileAppContentFile オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="2e7d5-124">In the request body, supply a JSON representation for the mobileAppContentFile object.</span></span>

<span data-ttu-id="2e7d5-125">次の表に、mobileAppContentFile の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="2e7d5-125">The following table shows the properties that are required when you create the mobileAppContentFile.</span></span>

|<span data-ttu-id="2e7d5-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2e7d5-126">Property</span></span>|<span data-ttu-id="2e7d5-127">型</span><span class="sxs-lookup"><span data-stu-id="2e7d5-127">Type</span></span>|<span data-ttu-id="2e7d5-128">説明</span><span class="sxs-lookup"><span data-stu-id="2e7d5-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2e7d5-129">azureStorageUri</span><span class="sxs-lookup"><span data-stu-id="2e7d5-129">azureStorageUri</span></span>|<span data-ttu-id="2e7d5-130">String</span><span class="sxs-lookup"><span data-stu-id="2e7d5-130">String</span></span>|<span data-ttu-id="2e7d5-131">Azure Storage の URI。</span><span class="sxs-lookup"><span data-stu-id="2e7d5-131">The Azure Storage URI.</span></span>|
|<span data-ttu-id="2e7d5-132">isCommitted</span><span class="sxs-lookup"><span data-stu-id="2e7d5-132">isCommitted</span></span>|<span data-ttu-id="2e7d5-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="2e7d5-133">Boolean</span></span>|<span data-ttu-id="2e7d5-134">ファイルがコミットされたかどうかを示す値。</span><span class="sxs-lookup"><span data-stu-id="2e7d5-134">A value indicating whether the file is committed.</span></span>|
|<span data-ttu-id="2e7d5-135">id</span><span class="sxs-lookup"><span data-stu-id="2e7d5-135">id</span></span>|<span data-ttu-id="2e7d5-136">String</span><span class="sxs-lookup"><span data-stu-id="2e7d5-136">String</span></span>|<span data-ttu-id="2e7d5-137">ファイル ID。</span><span class="sxs-lookup"><span data-stu-id="2e7d5-137">The File Id.</span></span>|
|<span data-ttu-id="2e7d5-138">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2e7d5-138">createdDateTime</span></span>|<span data-ttu-id="2e7d5-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2e7d5-139">DateTimeOffset</span></span>|<span data-ttu-id="2e7d5-140">ファイルが作成された時刻。</span><span class="sxs-lookup"><span data-stu-id="2e7d5-140">The time the file was created.</span></span>|
|<span data-ttu-id="2e7d5-141">name</span><span class="sxs-lookup"><span data-stu-id="2e7d5-141">name</span></span>|<span data-ttu-id="2e7d5-142">String</span><span class="sxs-lookup"><span data-stu-id="2e7d5-142">String</span></span>|<span data-ttu-id="2e7d5-143">ファイル名。</span><span class="sxs-lookup"><span data-stu-id="2e7d5-143">the file name.</span></span>|
|<span data-ttu-id="2e7d5-144">size</span><span class="sxs-lookup"><span data-stu-id="2e7d5-144">size</span></span>|<span data-ttu-id="2e7d5-145">Int64</span><span class="sxs-lookup"><span data-stu-id="2e7d5-145">Int64</span></span>|<span data-ttu-id="2e7d5-146">暗号化前のファイルのサイズ。</span><span class="sxs-lookup"><span data-stu-id="2e7d5-146">The size of the file prior to encryption.</span></span>|
|<span data-ttu-id="2e7d5-147">sizeEncrypted</span><span class="sxs-lookup"><span data-stu-id="2e7d5-147">sizeEncrypted</span></span>|<span data-ttu-id="2e7d5-148">Int64</span><span class="sxs-lookup"><span data-stu-id="2e7d5-148">Int64</span></span>|<span data-ttu-id="2e7d5-149">暗号化後のファイルのサイズ。</span><span class="sxs-lookup"><span data-stu-id="2e7d5-149">The size of the file after encryption.</span></span>|
|<span data-ttu-id="2e7d5-150">azureStorageUriExpirationDateTime</span><span class="sxs-lookup"><span data-stu-id="2e7d5-150">azureStorageUriExpirationDateTime</span></span>|<span data-ttu-id="2e7d5-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2e7d5-151">DateTimeOffset</span></span>|<span data-ttu-id="2e7d5-152">Azure Storage の URI が有効期限切れになる時刻。</span><span class="sxs-lookup"><span data-stu-id="2e7d5-152">The time the Azure storage Uri expires.</span></span>|
|<span data-ttu-id="2e7d5-153">manifest</span><span class="sxs-lookup"><span data-stu-id="2e7d5-153">manifest</span></span>|<span data-ttu-id="2e7d5-154">Binary</span><span class="sxs-lookup"><span data-stu-id="2e7d5-154">Binary</span></span>|<span data-ttu-id="2e7d5-155">マニフェスト情報。</span><span class="sxs-lookup"><span data-stu-id="2e7d5-155">The manifest information.</span></span>|
|<span data-ttu-id="2e7d5-156">uploadState</span><span class="sxs-lookup"><span data-stu-id="2e7d5-156">uploadState</span></span>|[<span data-ttu-id="2e7d5-157">mobileAppContentFileUploadState</span><span class="sxs-lookup"><span data-stu-id="2e7d5-157">mobileAppContentFileUploadState</span></span>](../resources/intune_apps_mobileappcontentfileuploadstate.md)|<span data-ttu-id="2e7d5-158">現在のアップロード要求の状態。</span><span class="sxs-lookup"><span data-stu-id="2e7d5-158">The state of the current upload request.</span></span> <span data-ttu-id="2e7d5-159">可能な値は、`success`、`transientError`、`error`、`unknown`、`azureStorageUriRequestSuccess`、`azureStorageUriRequestPending`、`azureStorageUriRequestFailed`、`azureStorageUriRequestTimedOut`、`azureStorageUriRenewalSuccess`、`azureStorageUriRenewalPending`、`azureStorageUriRenewalFailed`、`azureStorageUriRenewalTimedOut`、`commitFileSuccess`、`commitFilePending`、`commitFileFailed`、`commitFileTimedOut` です。</span><span class="sxs-lookup"><span data-stu-id="2e7d5-159">Possible values are: `success`, `transientError`, `error`, `unknown`, `azureStorageUriRequestSuccess`, `azureStorageUriRequestPending`, `azureStorageUriRequestFailed`, `azureStorageUriRequestTimedOut`, `azureStorageUriRenewalSuccess`, `azureStorageUriRenewalPending`, `azureStorageUriRenewalFailed`, `azureStorageUriRenewalTimedOut`, `commitFileSuccess`, `commitFilePending`, `commitFileFailed`, `commitFileTimedOut`.</span></span>|



## <a name="response"></a><span data-ttu-id="2e7d5-160">応答</span><span class="sxs-lookup"><span data-stu-id="2e7d5-160">Response</span></span>
<span data-ttu-id="2e7d5-161">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [mobileAppContentFile](../resources/intune_apps_mobileappcontentfile.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="2e7d5-161">If successful, this method returns a `201 Created` response code and a [mobileAppContentFile](../resources/intune_apps_mobileappcontentfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2e7d5-162">例</span><span class="sxs-lookup"><span data-stu-id="2e7d5-162">Example</span></span>
### <a name="request"></a><span data-ttu-id="2e7d5-163">要求</span><span class="sxs-lookup"><span data-stu-id="2e7d5-163">Request</span></span>
<span data-ttu-id="2e7d5-164">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2e7d5-164">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/files
Content-type: application/json
Content-length: 342

{
  "@odata.type": "#microsoft.graph.mobileAppContentFile",
  "azureStorageUri": "Azure Storage Uri value",
  "isCommitted": true,
  "name": "Name value",
  "size": 4,
  "sizeEncrypted": 13,
  "azureStorageUriExpirationDateTime": "2017-01-01T00:00:08.4940464-08:00",
  "manifest": "bWFuaWZlc3Q=",
  "uploadState": "transientError"
}
```

### <a name="response"></a><span data-ttu-id="2e7d5-165">応答</span><span class="sxs-lookup"><span data-stu-id="2e7d5-165">Response</span></span>
<span data-ttu-id="2e7d5-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2e7d5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 450

{
  "@odata.type": "#microsoft.graph.mobileAppContentFile",
  "azureStorageUri": "Azure Storage Uri value",
  "isCommitted": true,
  "id": "eab2e29b-e29b-eab2-9be2-b2ea9be2b2ea",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "name": "Name value",
  "size": 4,
  "sizeEncrypted": 13,
  "azureStorageUriExpirationDateTime": "2017-01-01T00:00:08.4940464-08:00",
  "manifest": "bWFuaWZlc3Q=",
  "uploadState": "transientError"
}
```



