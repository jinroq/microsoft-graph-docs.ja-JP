# <a name="update-managedappoperation"></a><span data-ttu-id="ebda1-101">managedAppOperation の更新</span><span class="sxs-lookup"><span data-stu-id="ebda1-101">Update managedAppOperation</span></span>

> <span data-ttu-id="ebda1-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ebda1-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ebda1-103">[managedAppOperation](../resources/intune_mam_managedappoperation.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="ebda1-103">Update the properties of a [managedAppOperation](../resources/intune_mam_managedappoperation.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ebda1-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="ebda1-104">Prerequisites</span></span>
<span data-ttu-id="ebda1-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ebda1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ebda1-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ebda1-107">Permission type</span></span>|<span data-ttu-id="ebda1-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ebda1-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ebda1-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ebda1-109">Delegated (work or school account)</span></span>|<span data-ttu-id="ebda1-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ebda1-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ebda1-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ebda1-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ebda1-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ebda1-112">Not supported.</span></span>|
|<span data-ttu-id="ebda1-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ebda1-113">Application</span></span>|<span data-ttu-id="ebda1-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ebda1-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ebda1-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ebda1-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations/{managedAppOperationId}
```

## <a name="request-headers"></a><span data-ttu-id="ebda1-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ebda1-116">Request headers</span></span>
|<span data-ttu-id="ebda1-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ebda1-117">Header</span></span>|<span data-ttu-id="ebda1-118">値</span><span class="sxs-lookup"><span data-stu-id="ebda1-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ebda1-119">承認</span><span class="sxs-lookup"><span data-stu-id="ebda1-119">Authorization</span></span>|<span data-ttu-id="ebda1-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="ebda1-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ebda1-121">承諾</span><span class="sxs-lookup"><span data-stu-id="ebda1-121">Accept</span></span>|<span data-ttu-id="ebda1-122">アプリケーションまたは json</span><span class="sxs-lookup"><span data-stu-id="ebda1-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ebda1-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="ebda1-123">Request body</span></span>
<span data-ttu-id="ebda1-124">要求本文で、[managedAppOperation](../resources/intune_mam_managedappoperation.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="ebda1-124">In the request body, supply a JSON representation for the [managedAppOperation](../resources/intune_mam_managedappoperation.md) object.</span></span>

<span data-ttu-id="ebda1-125">次の表に、[managedAppOperation](../resources/intune_mam_managedappoperation.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="ebda1-125">The following table shows the properties that are required when you create the [managedAppOperation](../resources/intune_mam_managedappoperation.md).</span></span>

|<span data-ttu-id="ebda1-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ebda1-126">Property</span></span>|<span data-ttu-id="ebda1-127">型</span><span class="sxs-lookup"><span data-stu-id="ebda1-127">Type</span></span>|<span data-ttu-id="ebda1-128">説明</span><span class="sxs-lookup"><span data-stu-id="ebda1-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ebda1-129">displayName</span><span class="sxs-lookup"><span data-stu-id="ebda1-129">displayName</span></span>|<span data-ttu-id="ebda1-130">文字列</span><span class="sxs-lookup"><span data-stu-id="ebda1-130">String</span></span>|<span data-ttu-id="ebda1-131">操作名。</span><span class="sxs-lookup"><span data-stu-id="ebda1-131">The operation name.</span></span>|
|<span data-ttu-id="ebda1-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ebda1-132">lastModifiedDateTime</span></span>|<span data-ttu-id="ebda1-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ebda1-133">DateTimeOffset</span></span>|<span data-ttu-id="ebda1-134">アプリ操作が変更された最終時刻。</span><span class="sxs-lookup"><span data-stu-id="ebda1-134">The last time the app operation was modified.</span></span>|
|<span data-ttu-id="ebda1-135">状態</span><span class="sxs-lookup"><span data-stu-id="ebda1-135">state</span></span>|<span data-ttu-id="ebda1-136">文字列</span><span class="sxs-lookup"><span data-stu-id="ebda1-136">String</span></span>|<span data-ttu-id="ebda1-137">操作の現在の状態。</span><span class="sxs-lookup"><span data-stu-id="ebda1-137">The current state of the operation</span></span>|
|<span data-ttu-id="ebda1-138">id</span><span class="sxs-lookup"><span data-stu-id="ebda1-138">id</span></span>|<span data-ttu-id="ebda1-139">文字列</span><span class="sxs-lookup"><span data-stu-id="ebda1-139">String</span></span>|<span data-ttu-id="ebda1-140">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="ebda1-140">Key of the entity.</span></span>|
|<span data-ttu-id="ebda1-141">バージョン</span><span class="sxs-lookup"><span data-stu-id="ebda1-141">version</span></span>|<span data-ttu-id="ebda1-142">文字列</span><span class="sxs-lookup"><span data-stu-id="ebda1-142">String</span></span>|<span data-ttu-id="ebda1-143">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="ebda1-143">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="ebda1-144">応答</span><span class="sxs-lookup"><span data-stu-id="ebda1-144">Response</span></span>
<span data-ttu-id="ebda1-145">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [managedAppOperation](../resources/intune_mam_managedappoperation.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ebda1-145">If successful, this method returns a `200 OK` response code and an updated [managedAppOperation](../resources/intune_mam_managedappoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ebda1-146">例</span><span class="sxs-lookup"><span data-stu-id="ebda1-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="ebda1-147">要求</span><span class="sxs-lookup"><span data-stu-id="ebda1-147">Request</span></span>
<span data-ttu-id="ebda1-148">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ebda1-148">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations/{managedAppOperationId}
Content-type: application/json
Content-length: 165

{
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "state": "State value",
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="ebda1-149">応答</span><span class="sxs-lookup"><span data-stu-id="ebda1-149">Response</span></span>
<span data-ttu-id="ebda1-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ebda1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 272

{
  "@odata.type": "#microsoft.graph.managedAppOperation",
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "state": "State value",
  "id": "f2867b06-7b06-f286-067b-86f2067b86f2",
  "version": "Version value"
}
```








