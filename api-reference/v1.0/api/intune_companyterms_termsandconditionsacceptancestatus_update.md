# <a name="update-termsandconditionsacceptancestatus"></a><span data-ttu-id="e86d5-101">termsAndConditionsAcceptanceStatus の更新</span><span class="sxs-lookup"><span data-stu-id="e86d5-101">Update termsAndConditionsAcceptanceStatus</span></span>

> <span data-ttu-id="e86d5-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e86d5-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e86d5-103">[termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="e86d5-103">Update the properties of a [termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e86d5-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="e86d5-104">Prerequisites</span></span>
<span data-ttu-id="e86d5-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e86d5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e86d5-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e86d5-107">Permission type</span></span>|<span data-ttu-id="e86d5-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="e86d5-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e86d5-109">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="e86d5-109">Delegated (work or school account)</span></span>|<span data-ttu-id="e86d5-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e86d5-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e86d5-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e86d5-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e86d5-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e86d5-112">Not supported.</span></span>|
|<span data-ttu-id="e86d5-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e86d5-113">Application</span></span>|<span data-ttu-id="e86d5-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e86d5-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e86d5-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e86d5-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="e86d5-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e86d5-116">Request headers</span></span>
|<span data-ttu-id="e86d5-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e86d5-117">Header</span></span>|<span data-ttu-id="e86d5-118">値</span><span class="sxs-lookup"><span data-stu-id="e86d5-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e86d5-119">承認</span><span class="sxs-lookup"><span data-stu-id="e86d5-119">Authorization</span></span>|<span data-ttu-id="e86d5-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="e86d5-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e86d5-121">承諾する</span><span class="sxs-lookup"><span data-stu-id="e86d5-121">Accept</span></span>|<span data-ttu-id="e86d5-122">アプリケーションまたは json</span><span class="sxs-lookup"><span data-stu-id="e86d5-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e86d5-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="e86d5-123">Request body</span></span>
<span data-ttu-id="e86d5-124">要求本文で、[termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="e86d5-124">In the request body, supply a JSON representation for the [termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md) object.</span></span>

<span data-ttu-id="e86d5-125">次の表に、[termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="e86d5-125">The following table shows the properties that are required when you create the [termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md).</span></span>

|<span data-ttu-id="e86d5-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e86d5-126">Property</span></span>|<span data-ttu-id="e86d5-127">型</span><span class="sxs-lookup"><span data-stu-id="e86d5-127">Type</span></span>|<span data-ttu-id="e86d5-128">説明</span><span class="sxs-lookup"><span data-stu-id="e86d5-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e86d5-129">ID</span><span class="sxs-lookup"><span data-stu-id="e86d5-129">id</span></span>|<span data-ttu-id="e86d5-130">文字列</span><span class="sxs-lookup"><span data-stu-id="e86d5-130">String</span></span>|<span data-ttu-id="e86d5-131">エンティティの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="e86d5-131">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="e86d5-132">userDisplayName</span><span class="sxs-lookup"><span data-stu-id="e86d5-132">userDisplayName</span></span>|<span data-ttu-id="e86d5-133">文字列</span><span class="sxs-lookup"><span data-stu-id="e86d5-133">String</span></span>|<span data-ttu-id="e86d5-134">エンティティによって承諾が示されているユーザーの表示名。</span><span class="sxs-lookup"><span data-stu-id="e86d5-134">Display name of the user whose acceptance the entity represents.</span></span>|
|<span data-ttu-id="e86d5-135">acceptedVersion</span><span class="sxs-lookup"><span data-stu-id="e86d5-135">acceptedVersion</span></span>|<span data-ttu-id="e86d5-136">Int32</span><span class="sxs-lookup"><span data-stu-id="e86d5-136">Int32</span></span>|<span data-ttu-id="e86d5-137">ユーザーによって承諾された使用条件の最新バージョン番号。</span><span class="sxs-lookup"><span data-stu-id="e86d5-137">Most recent version number of the T&C accepted by the user.</span></span>|
|<span data-ttu-id="e86d5-138">acceptedDateTime</span><span class="sxs-lookup"><span data-stu-id="e86d5-138">acceptedDateTime</span></span>|<span data-ttu-id="e86d5-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e86d5-139">DateTimeOffset</span></span>|<span data-ttu-id="e86d5-140">最後にユーザーによって使用条件が承諾された DateTime。</span><span class="sxs-lookup"><span data-stu-id="e86d5-140">DateTime when the terms were last accepted by the user.</span></span>|



## <a name="response"></a><span data-ttu-id="e86d5-141">応答</span><span class="sxs-lookup"><span data-stu-id="e86d5-141">Response</span></span>
<span data-ttu-id="e86d5-142">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e86d5-142">If successful, this method returns a `200 OK` response code and an updated [termsAndConditionsAcceptanceStatus](../resources/intune_companyterms_termsandconditionsacceptancestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e86d5-143">例</span><span class="sxs-lookup"><span data-stu-id="e86d5-143">Example</span></span>
### <a name="request"></a><span data-ttu-id="e86d5-144">要求</span><span class="sxs-lookup"><span data-stu-id="e86d5-144">Request</span></span>
<span data-ttu-id="e86d5-145">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e86d5-145">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses/{termsAndConditionsAcceptanceStatusId}
Content-type: application/json
Content-length: 138

{
  "userDisplayName": "User Display Name value",
  "acceptedVersion": 15,
  "acceptedDateTime": "2016-12-31T23:57:43.6165506-08:00"
}
```

### <a name="response"></a><span data-ttu-id="e86d5-146">応答</span><span class="sxs-lookup"><span data-stu-id="e86d5-146">Response</span></span>
<span data-ttu-id="e86d5-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e86d5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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








