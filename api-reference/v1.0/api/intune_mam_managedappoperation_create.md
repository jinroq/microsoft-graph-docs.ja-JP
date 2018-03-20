# <a name="create-managedappoperation"></a><span data-ttu-id="de88f-101">managedAppOperation の作成</span><span class="sxs-lookup"><span data-stu-id="de88f-101">Create managedAppOperation</span></span>

> <span data-ttu-id="de88f-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="de88f-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="de88f-103">新しい [managedAppOperation](../resources/intune_mam_managedappoperation.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="de88f-103">Create a new [plannerBucket](../resources/intune_mam_managedappoperation.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="de88f-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="de88f-104">Prerequisites</span></span>
<span data-ttu-id="de88f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="de88f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="de88f-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="de88f-107">Permission type</span></span>|<span data-ttu-id="de88f-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="de88f-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="de88f-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="de88f-109">Delegated (work or school account)</span></span>|<span data-ttu-id="de88f-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de88f-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="de88f-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="de88f-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="de88f-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="de88f-112">Not supported.</span></span>|
|<span data-ttu-id="de88f-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="de88f-113">Application</span></span>|<span data-ttu-id="de88f-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="de88f-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="de88f-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="de88f-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations
```

## <a name="request-headers"></a><span data-ttu-id="de88f-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="de88f-116">Request headers</span></span>
|<span data-ttu-id="de88f-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="de88f-117">Header</span></span>|<span data-ttu-id="de88f-118">値</span><span class="sxs-lookup"><span data-stu-id="de88f-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="de88f-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="de88f-119">Authorization</span></span>|<span data-ttu-id="de88f-120">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="de88f-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="de88f-121">Accept</span><span class="sxs-lookup"><span data-stu-id="de88f-121">Accept</span></span>|<span data-ttu-id="de88f-122">application/json</span><span class="sxs-lookup"><span data-stu-id="de88f-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="de88f-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="de88f-123">Request body</span></span>
<span data-ttu-id="de88f-124">要求本文で、managedAppOperation オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="de88f-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="de88f-125">次の表に、managedAppOperation の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="de88f-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="de88f-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="de88f-126">Property</span></span>|<span data-ttu-id="de88f-127">型</span><span class="sxs-lookup"><span data-stu-id="de88f-127">Type</span></span>|<span data-ttu-id="de88f-128">説明</span><span class="sxs-lookup"><span data-stu-id="de88f-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="de88f-129">displayName</span><span class="sxs-lookup"><span data-stu-id="de88f-129">displayName</span></span>|<span data-ttu-id="de88f-130">String</span><span class="sxs-lookup"><span data-stu-id="de88f-130">String</span></span>|<span data-ttu-id="de88f-131">操作名。</span><span class="sxs-lookup"><span data-stu-id="de88f-131">The operation name.</span></span>|
|<span data-ttu-id="de88f-132">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="de88f-132">lastModifiedDateTime</span></span>|<span data-ttu-id="de88f-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="de88f-133">DateTimeOffset</span></span>|<span data-ttu-id="de88f-134">アプリ操作が変更された最終時刻。</span><span class="sxs-lookup"><span data-stu-id="de88f-134">The last time the app operation was modified.</span></span>|
|<span data-ttu-id="de88f-135">state</span><span class="sxs-lookup"><span data-stu-id="de88f-135">state</span></span>|<span data-ttu-id="de88f-136">String</span><span class="sxs-lookup"><span data-stu-id="de88f-136">String</span></span>|<span data-ttu-id="de88f-137">操作の現在の状態。</span><span class="sxs-lookup"><span data-stu-id="de88f-137">The current state of the operation</span></span>|
|<span data-ttu-id="de88f-138">id</span><span class="sxs-lookup"><span data-stu-id="de88f-138">id</span></span>|<span data-ttu-id="de88f-139">String</span><span class="sxs-lookup"><span data-stu-id="de88f-139">String</span></span>|<span data-ttu-id="de88f-140">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="de88f-140">Name of the entity.</span></span>|
|<span data-ttu-id="de88f-141">version</span><span class="sxs-lookup"><span data-stu-id="de88f-141">version</span></span>|<span data-ttu-id="de88f-142">String</span><span class="sxs-lookup"><span data-stu-id="de88f-142">String</span></span>|<span data-ttu-id="de88f-143">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="de88f-143">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="de88f-144">応答</span><span class="sxs-lookup"><span data-stu-id="de88f-144">Response</span></span>
<span data-ttu-id="de88f-145">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [managedAppOperation](../resources/intune_mam_managedappoperation.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="de88f-145">If successful, this method returns a `201 Created` response code and a [section](../resources/intune_mam_managedappoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="de88f-146">例</span><span class="sxs-lookup"><span data-stu-id="de88f-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="de88f-147">要求</span><span class="sxs-lookup"><span data-stu-id="de88f-147">Request</span></span>
<span data-ttu-id="de88f-148">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="de88f-148">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedAppRegistrations/{managedAppRegistrationId}/operations
Content-type: application/json
Content-length: 223

{
  "@odata.type": "#microsoft.graph.managedAppOperation",
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "state": "State value",
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="de88f-149">応答</span><span class="sxs-lookup"><span data-stu-id="de88f-149">Response</span></span>
<span data-ttu-id="de88f-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="de88f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



