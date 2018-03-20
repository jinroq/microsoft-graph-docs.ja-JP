# <a name="update-organization"></a><span data-ttu-id="2d6f5-101">organization の更新</span><span class="sxs-lookup"><span data-stu-id="2d6f5-101">Update organization</span></span>

> <span data-ttu-id="2d6f5-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="2d6f5-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2d6f5-103">[organization](../resources/intune_onboarding_organization.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="2d6f5-103">Update the properties of a [calendar](../resources/intune_onboarding_organization.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2d6f5-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="2d6f5-104">Prerequisites</span></span>
<span data-ttu-id="2d6f5-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2d6f5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2d6f5-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2d6f5-107">Permission type</span></span>|<span data-ttu-id="2d6f5-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="2d6f5-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2d6f5-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2d6f5-109">Delegated (work or school account)</span></span>|<span data-ttu-id="2d6f5-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2d6f5-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="2d6f5-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2d6f5-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2d6f5-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2d6f5-112">Not supported.</span></span>|
|<span data-ttu-id="2d6f5-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2d6f5-113">Application</span></span>|<span data-ttu-id="2d6f5-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2d6f5-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2d6f5-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2d6f5-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /organization/{organizationId}
```

## <a name="request-headers"></a><span data-ttu-id="2d6f5-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2d6f5-116">Request headers</span></span>
|<span data-ttu-id="2d6f5-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2d6f5-117">Header</span></span>|<span data-ttu-id="2d6f5-118">値</span><span class="sxs-lookup"><span data-stu-id="2d6f5-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2d6f5-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="2d6f5-119">Authorization</span></span>|<span data-ttu-id="2d6f5-120">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="2d6f5-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="2d6f5-121">Accept</span><span class="sxs-lookup"><span data-stu-id="2d6f5-121">Accept</span></span>|<span data-ttu-id="2d6f5-122">application/json</span><span class="sxs-lookup"><span data-stu-id="2d6f5-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2d6f5-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="2d6f5-123">Request body</span></span>
<span data-ttu-id="2d6f5-124">要求本文で、[organization](../resources/intune_onboarding_organization.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="2d6f5-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_onboarding_organization.md) object.</span></span>

<span data-ttu-id="2d6f5-125">次の表に、[organization](../resources/intune_onboarding_organization.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="2d6f5-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="2d6f5-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2d6f5-126">Property</span></span>|<span data-ttu-id="2d6f5-127">型</span><span class="sxs-lookup"><span data-stu-id="2d6f5-127">Type</span></span>|<span data-ttu-id="2d6f5-128">説明</span><span class="sxs-lookup"><span data-stu-id="2d6f5-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2d6f5-129">id</span><span class="sxs-lookup"><span data-stu-id="2d6f5-129">id</span></span>|<span data-ttu-id="2d6f5-130">String</span><span class="sxs-lookup"><span data-stu-id="2d6f5-130">String</span></span>|<span data-ttu-id="2d6f5-131">オブジェクトの GUID。</span><span class="sxs-lookup"><span data-stu-id="2d6f5-131">The user GUID for the security object is not valid.</span></span>|
|<span data-ttu-id="2d6f5-132">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="2d6f5-132">mobileDeviceManagementAuthority</span></span>|<span data-ttu-id="2d6f5-133">String</span><span class="sxs-lookup"><span data-stu-id="2d6f5-133">String</span></span>|<span data-ttu-id="2d6f5-134">モバイル デバイス管理権限。</span><span class="sxs-lookup"><span data-stu-id="2d6f5-134">Mobile device management authority.</span></span> <span data-ttu-id="2d6f5-135">可能な値は、`unknown`、`intune`、`sccm`、`office365` です。</span><span class="sxs-lookup"><span data-stu-id="2d6f5-135">Possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|



## <a name="response"></a><span data-ttu-id="2d6f5-136">応答</span><span class="sxs-lookup"><span data-stu-id="2d6f5-136">Response</span></span>
<span data-ttu-id="2d6f5-137">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [organization](../resources/intune_onboarding_organization.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="2d6f5-137">If successful, this method returns a `200 OK` response code and updated [organization](../resources/intune_onboarding_organization.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2d6f5-138">例</span><span class="sxs-lookup"><span data-stu-id="2d6f5-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="2d6f5-139">要求</span><span class="sxs-lookup"><span data-stu-id="2d6f5-139">Request</span></span>
<span data-ttu-id="2d6f5-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2d6f5-140">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/organization/{organizationId}
Content-type: application/json
Content-length: 51

{
  "mobileDeviceManagementAuthority": "intune"
}
```

### <a name="response"></a><span data-ttu-id="2d6f5-141">応答</span><span class="sxs-lookup"><span data-stu-id="2d6f5-141">Response</span></span>
<span data-ttu-id="2d6f5-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2d6f5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 151

{
  "@odata.type": "#microsoft.graph.organization",
  "id": "9efe224a-224a-9efe-4a22-fe9e4a22fe9e",
  "mobileDeviceManagementAuthority": "intune"
}
```



