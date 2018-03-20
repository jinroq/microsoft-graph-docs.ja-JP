# <a name="create-termsandconditionsacceptancestatus"></a><span data-ttu-id="4fa1c-101">termsAndConditionsAcceptanceStatus の作成</span><span class="sxs-lookup"><span data-stu-id="4fa1c-101">Create termsAndConditionsAcceptanceStatus</span></span>

> <span data-ttu-id="4fa1c-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="4fa1c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4fa1c-103">新しい [termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="4fa1c-103">Create a new [plannerBucket](../resources/intune_companyterms_termsandconditionsacceptancestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4fa1c-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="4fa1c-104">Prerequisites</span></span>
<span data-ttu-id="4fa1c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4fa1c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="4fa1c-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4fa1c-107">Permission type</span></span>|<span data-ttu-id="4fa1c-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="4fa1c-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4fa1c-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4fa1c-109">Delegated (work or school account)</span></span>|<span data-ttu-id="4fa1c-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4fa1c-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="4fa1c-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4fa1c-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4fa1c-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4fa1c-112">Not supported.</span></span>|
|<span data-ttu-id="4fa1c-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4fa1c-113">Application</span></span>|<span data-ttu-id="4fa1c-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4fa1c-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4fa1c-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4fa1c-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="4fa1c-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4fa1c-116">Request headers</span></span>
|<span data-ttu-id="4fa1c-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4fa1c-117">Header</span></span>|<span data-ttu-id="4fa1c-118">値</span><span class="sxs-lookup"><span data-stu-id="4fa1c-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4fa1c-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="4fa1c-119">Authorization</span></span>|<span data-ttu-id="4fa1c-120">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="4fa1c-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="4fa1c-121">Accept</span><span class="sxs-lookup"><span data-stu-id="4fa1c-121">Accept</span></span>|<span data-ttu-id="4fa1c-122">application/json</span><span class="sxs-lookup"><span data-stu-id="4fa1c-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4fa1c-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="4fa1c-123">Request body</span></span>
<span data-ttu-id="4fa1c-124">要求本文で、termsAndConditionsAcceptanceStatus オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="4fa1c-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="4fa1c-125">次の表に、termsAndConditionsAcceptanceStatus の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="4fa1c-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="4fa1c-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4fa1c-126">Property</span></span>|<span data-ttu-id="4fa1c-127">型</span><span class="sxs-lookup"><span data-stu-id="4fa1c-127">Type</span></span>|<span data-ttu-id="4fa1c-128">説明</span><span class="sxs-lookup"><span data-stu-id="4fa1c-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4fa1c-129">id</span><span class="sxs-lookup"><span data-stu-id="4fa1c-129">id</span></span>|<span data-ttu-id="4fa1c-130">String</span><span class="sxs-lookup"><span data-stu-id="4fa1c-130">String</span></span>|<span data-ttu-id="4fa1c-131">エンティティの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="4fa1c-131">Unique identifier of the folder.</span></span>|
|<span data-ttu-id="4fa1c-132">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="4fa1c-132">userDisplayName</span></span>|<span data-ttu-id="4fa1c-133">String</span><span class="sxs-lookup"><span data-stu-id="4fa1c-133">String</span></span>|<span data-ttu-id="4fa1c-134">エンティティによって承諾が示されているユーザーの表示名。</span><span class="sxs-lookup"><span data-stu-id="4fa1c-134">Display name of the user whose acceptance the entity represents.</span></span>|
|<span data-ttu-id="4fa1c-135">acceptedVersion</span><span class="sxs-lookup"><span data-stu-id="4fa1c-135">acceptedVersion</span></span>|<span data-ttu-id="4fa1c-136">Int32</span><span class="sxs-lookup"><span data-stu-id="4fa1c-136">Int32</span></span>|<span data-ttu-id="4fa1c-137">ユーザーによって承諾された使用条件の最新バージョン番号。</span><span class="sxs-lookup"><span data-stu-id="4fa1c-137">Most recent version number of the T&C accepted by the user.</span></span>|
|<span data-ttu-id="4fa1c-138">acceptedDateTime</span><span class="sxs-lookup"><span data-stu-id="4fa1c-138">acceptedDateTime</span></span>|<span data-ttu-id="4fa1c-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4fa1c-139">DateTimeOffset</span></span>|<span data-ttu-id="4fa1c-140">最後にユーザーによって使用条件が承諾された DateTime。</span><span class="sxs-lookup"><span data-stu-id="4fa1c-140">DateTime when the terms were last accepted by the user.</span></span>|



## <a name="response"></a><span data-ttu-id="4fa1c-141">応答</span><span class="sxs-lookup"><span data-stu-id="4fa1c-141">Response</span></span>
<span data-ttu-id="4fa1c-142">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="4fa1c-142">If successful, this method returns a `201 Created` response code and a [section](../resources/intune_companyterms_termsandconditionsacceptancestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4fa1c-143">例</span><span class="sxs-lookup"><span data-stu-id="4fa1c-143">Example</span></span>
### <a name="request"></a><span data-ttu-id="4fa1c-144">要求</span><span class="sxs-lookup"><span data-stu-id="4fa1c-144">Request</span></span>
<span data-ttu-id="4fa1c-145">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4fa1c-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses
Content-type: application/json
Content-length: 211

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
  "userDisplayName": "User Display Name value",
  "acceptedVersion": 15,
  "acceptedDateTime": "2016-12-31T23:57:43.6165506-08:00"
}
```

### <a name="response"></a><span data-ttu-id="4fa1c-146">応答</span><span class="sxs-lookup"><span data-stu-id="4fa1c-146">Response</span></span>
<span data-ttu-id="4fa1c-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4fa1c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 260

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
  "id": "a045ce1a-ce1a-a045-1ace-45a01ace45a0",
  "userDisplayName": "User Display Name value",
  "acceptedVersion": 15,
  "acceptedDateTime": "2016-12-31T23:57:43.6165506-08:00"
}
```



