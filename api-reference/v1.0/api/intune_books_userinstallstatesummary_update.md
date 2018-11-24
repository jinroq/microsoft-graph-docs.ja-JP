# <a name="update-userinstallstatesummary"></a><span data-ttu-id="45149-101">userInstallStateSummary の更新</span><span class="sxs-lookup"><span data-stu-id="45149-101">Update userInstallStateSummary</span></span>

> <span data-ttu-id="45149-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="45149-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="45149-103">[userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="45149-103">Update the properties of a [userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="45149-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="45149-104">Prerequisites</span></span>
<span data-ttu-id="45149-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="45149-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="45149-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="45149-107">Permission type</span></span>|<span data-ttu-id="45149-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="45149-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="45149-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="45149-109">Delegated (work or school account)</span></span>|<span data-ttu-id="45149-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45149-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="45149-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="45149-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="45149-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="45149-112">Not supported.</span></span>|
|<span data-ttu-id="45149-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="45149-113">Application</span></span>|<span data-ttu-id="45149-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="45149-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="45149-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="45149-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="45149-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="45149-116">Request headers</span></span>
|<span data-ttu-id="45149-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="45149-117">Header</span></span>|<span data-ttu-id="45149-118">値</span><span class="sxs-lookup"><span data-stu-id="45149-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="45149-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="45149-119">Authorization</span></span>|<span data-ttu-id="45149-120">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="45149-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="45149-121">Accept</span><span class="sxs-lookup"><span data-stu-id="45149-121">Accept</span></span>|<span data-ttu-id="45149-122">application/json</span><span class="sxs-lookup"><span data-stu-id="45149-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="45149-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="45149-123">Request body</span></span>
<span data-ttu-id="45149-124">要求本文で、[userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="45149-124">In the request body, supply a JSON representation for the [userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md) object.</span></span>

<span data-ttu-id="45149-125">次の表に、[userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="45149-125">The following table shows the properties that are required when you create the [userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md).</span></span>

|<span data-ttu-id="45149-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="45149-126">Property</span></span>|<span data-ttu-id="45149-127">型</span><span class="sxs-lookup"><span data-stu-id="45149-127">Type</span></span>|<span data-ttu-id="45149-128">説明</span><span class="sxs-lookup"><span data-stu-id="45149-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45149-129">id</span><span class="sxs-lookup"><span data-stu-id="45149-129">id</span></span>|<span data-ttu-id="45149-130">String</span><span class="sxs-lookup"><span data-stu-id="45149-130">String</span></span>|<span data-ttu-id="45149-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="45149-131">Key of the entity.</span></span>|
|<span data-ttu-id="45149-132">userName</span><span class="sxs-lookup"><span data-stu-id="45149-132">userName</span></span>|<span data-ttu-id="45149-133">String</span><span class="sxs-lookup"><span data-stu-id="45149-133">String</span></span>|<span data-ttu-id="45149-134">ユーザー名です。</span><span class="sxs-lookup"><span data-stu-id="45149-134">User name.</span></span>|
|<span data-ttu-id="45149-135">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="45149-135">installedDeviceCount</span></span>|<span data-ttu-id="45149-136">Int32</span><span class="sxs-lookup"><span data-stu-id="45149-136">Int32</span></span>|<span data-ttu-id="45149-137">インストールされたデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="45149-137">Installed Device Count.</span></span>|
|<span data-ttu-id="45149-138">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="45149-138">failedDeviceCount</span></span>|<span data-ttu-id="45149-139">Int32</span><span class="sxs-lookup"><span data-stu-id="45149-139">Int32</span></span>|<span data-ttu-id="45149-140">失敗したデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="45149-140">Failed Device Count.</span></span>|
|<span data-ttu-id="45149-141">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="45149-141">notInstalledDeviceCount</span></span>|<span data-ttu-id="45149-142">Int32</span><span class="sxs-lookup"><span data-stu-id="45149-142">Int32</span></span>|<span data-ttu-id="45149-143">インストールされていないデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="45149-143">Not installed device count.</span></span>|



## <a name="response"></a><span data-ttu-id="45149-144">応答</span><span class="sxs-lookup"><span data-stu-id="45149-144">Response</span></span>
<span data-ttu-id="45149-145">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="45149-145">If successful, this method returns a `200 OK` response code and an updated [userInstallStateSummary](../resources/intune_books_userinstallstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="45149-146">例</span><span class="sxs-lookup"><span data-stu-id="45149-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="45149-147">要求</span><span class="sxs-lookup"><span data-stu-id="45149-147">Request</span></span>
<span data-ttu-id="45149-148">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="45149-148">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}
Content-type: application/json
Content-length: 189

{
  "@odata.type": "#microsoft.graph.userInstallStateSummary",
  "userName": "User Name value",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notInstalledDeviceCount": 7
}
```

### <a name="response"></a><span data-ttu-id="45149-149">応答</span><span class="sxs-lookup"><span data-stu-id="45149-149">Response</span></span>
<span data-ttu-id="45149-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="45149-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 238

{
  "@odata.type": "#microsoft.graph.userInstallStateSummary",
  "id": "1e5b41ba-41ba-1e5b-ba41-5b1eba415b1e",
  "userName": "User Name value",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notInstalledDeviceCount": 7
}
```



