# <a name="update-ebookinstallsummary"></a><span data-ttu-id="4c276-101">eBookInstallSummary の更新</span><span class="sxs-lookup"><span data-stu-id="4c276-101">Update eBookInstallSummary</span></span>

> <span data-ttu-id="4c276-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="4c276-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4c276-103">[eBookInstallSummary](../resources/intune_books_ebookinstallsummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="4c276-103">Update the properties of a [eBookInstallSummary](../resources/intune_books_ebookinstallsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4c276-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="4c276-104">Prerequisites</span></span>
<span data-ttu-id="4c276-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4c276-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4c276-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4c276-107">Permission type</span></span>|<span data-ttu-id="4c276-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="4c276-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4c276-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4c276-109">Delegated (work or school account)</span></span>|<span data-ttu-id="4c276-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c276-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4c276-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4c276-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4c276-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4c276-112">Not supported.</span></span>|
|<span data-ttu-id="4c276-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4c276-113">Application</span></span>|<span data-ttu-id="4c276-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4c276-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4c276-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4c276-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/installSummary
```

## <a name="request-headers"></a><span data-ttu-id="4c276-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4c276-116">Request headers</span></span>
|<span data-ttu-id="4c276-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4c276-117">Header</span></span>|<span data-ttu-id="4c276-118">値</span><span class="sxs-lookup"><span data-stu-id="4c276-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4c276-119">承認</span><span class="sxs-lookup"><span data-stu-id="4c276-119">Authorization</span></span>|<span data-ttu-id="4c276-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="4c276-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4c276-121">承諾</span><span class="sxs-lookup"><span data-stu-id="4c276-121">Accept</span></span>|<span data-ttu-id="4c276-122">アプリケーションまたは json</span><span class="sxs-lookup"><span data-stu-id="4c276-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4c276-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="4c276-123">Request body</span></span>
<span data-ttu-id="4c276-124">要求本文で、[eBookInstallSummary](../resources/intune_books_ebookinstallsummary.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="4c276-124">In the request body, supply a JSON representation for the [eBookInstallSummary](../resources/intune_books_ebookinstallsummary.md) object.</span></span>

<span data-ttu-id="4c276-125">次の表に、[eBookInstallSummary](../resources/intune_books_ebookinstallsummary.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="4c276-125">The following table shows the properties that are required when you create the [eBookInstallSummary](../resources/intune_books_ebookinstallsummary.md).</span></span>

|<span data-ttu-id="4c276-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4c276-126">Property</span></span>|<span data-ttu-id="4c276-127">型</span><span class="sxs-lookup"><span data-stu-id="4c276-127">Type</span></span>|<span data-ttu-id="4c276-128">説明</span><span class="sxs-lookup"><span data-stu-id="4c276-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4c276-129">id</span><span class="sxs-lookup"><span data-stu-id="4c276-129">id</span></span>|<span data-ttu-id="4c276-130">文字列</span><span class="sxs-lookup"><span data-stu-id="4c276-130">String</span></span>|<span data-ttu-id="4c276-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="4c276-131">Key of the entity.</span></span>|
|<span data-ttu-id="4c276-132">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="4c276-132">installedDeviceCount</span></span>|<span data-ttu-id="4c276-133">Int32</span><span class="sxs-lookup"><span data-stu-id="4c276-133">Int32</span></span>|<span data-ttu-id="4c276-134">このブックが正常にインストールされたデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="4c276-134">Number of Devices that have successfully installed this book.</span></span>|
|<span data-ttu-id="4c276-135">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="4c276-135">failedDeviceCount</span></span>|<span data-ttu-id="4c276-136">Int32</span><span class="sxs-lookup"><span data-stu-id="4c276-136">Int32</span></span>|<span data-ttu-id="4c276-137">このブックのインストールが失敗したデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="4c276-137">Number of Devices that have failed to install this book.</span></span>|
|<span data-ttu-id="4c276-138">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="4c276-138">notInstalledDeviceCount</span></span>|<span data-ttu-id="4c276-139">Int32</span><span class="sxs-lookup"><span data-stu-id="4c276-139">Int32</span></span>|<span data-ttu-id="4c276-140">このブックがインストールされていないデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="4c276-140">Number of Devices that does not have this book installed.</span></span>|
|<span data-ttu-id="4c276-141">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="4c276-141">installedUserCount</span></span>|<span data-ttu-id="4c276-142">Int32</span><span class="sxs-lookup"><span data-stu-id="4c276-142">Int32</span></span>|<span data-ttu-id="4c276-143">このブックがすべて正常にインストールされたデバイスを所有しているユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="4c276-143">Number of Users whose devices have all succeeded to install this book.</span></span>|
|<span data-ttu-id="4c276-144">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="4c276-144">failedUserCount</span></span>|<span data-ttu-id="4c276-145">Int32</span><span class="sxs-lookup"><span data-stu-id="4c276-145">Int32</span></span>|<span data-ttu-id="4c276-146">このブックのインストールが失敗したデバイスを 1 台以上所有しているユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="4c276-146">Number of Users that have 1 or more device that failed to install this book.</span></span>|
|<span data-ttu-id="4c276-147">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="4c276-147">notInstalledUserCount</span></span>|<span data-ttu-id="4c276-148">Int32</span><span class="sxs-lookup"><span data-stu-id="4c276-148">Int32</span></span>|<span data-ttu-id="4c276-149">このブックをインストールしていないユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="4c276-149">Number of Users that did not install this book.</span></span>|



## <a name="response"></a><span data-ttu-id="4c276-150">応答</span><span class="sxs-lookup"><span data-stu-id="4c276-150">Response</span></span>
<span data-ttu-id="4c276-151">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [eBookInstallSummary](../resources/intune_books_ebookinstallsummary.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="4c276-151">If successful, this method returns a `200 OK` response code and an updated [eBookInstallSummary](../resources/intune_books_ebookinstallsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4c276-152">例</span><span class="sxs-lookup"><span data-stu-id="4c276-152">Example</span></span>
### <a name="request"></a><span data-ttu-id="4c276-153">要求</span><span class="sxs-lookup"><span data-stu-id="4c276-153">Request</span></span>
<span data-ttu-id="4c276-154">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4c276-154">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/installSummary
Content-type: application/json
Content-length: 178

{
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notInstalledDeviceCount": 7,
  "installedUserCount": 2,
  "failedUserCount": 15,
  "notInstalledUserCount": 5
}
```

### <a name="response"></a><span data-ttu-id="4c276-155">応答</span><span class="sxs-lookup"><span data-stu-id="4c276-155">Response</span></span>
<span data-ttu-id="4c276-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4c276-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 285

{
  "@odata.type": "#microsoft.graph.eBookInstallSummary",
  "id": "9708ad78-ad78-9708-78ad-089778ad0897",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notInstalledDeviceCount": 7,
  "installedUserCount": 2,
  "failedUserCount": 15,
  "notInstalledUserCount": 5
}
```








