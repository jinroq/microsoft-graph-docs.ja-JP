# <a name="update-organization"></a><span data-ttu-id="9f102-101">organization の更新</span><span class="sxs-lookup"><span data-stu-id="9f102-101">Update organization</span></span>

> <span data-ttu-id="9f102-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="9f102-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9f102-103">[organization](../resources/intune_onboarding_organization.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="9f102-103">Update the properties of a [organization](../resources/intune_onboarding_organization.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9f102-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="9f102-104">Prerequisites</span></span>
<span data-ttu-id="9f102-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9f102-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="9f102-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9f102-107">Permission type</span></span>|<span data-ttu-id="9f102-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="9f102-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9f102-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9f102-109">Delegated (work or school account)</span></span>|<span data-ttu-id="9f102-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f102-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="9f102-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9f102-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9f102-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9f102-112">Not supported.</span></span>|
|<span data-ttu-id="9f102-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9f102-113">Application</span></span>|<span data-ttu-id="9f102-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9f102-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9f102-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9f102-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /organization/{organizationId}
```

## <a name="request-headers"></a><span data-ttu-id="9f102-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9f102-116">Request headers</span></span>
|<span data-ttu-id="9f102-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9f102-117">Header</span></span>|<span data-ttu-id="9f102-118">値</span><span class="sxs-lookup"><span data-stu-id="9f102-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9f102-119">承認</span><span class="sxs-lookup"><span data-stu-id="9f102-119">Authorization</span></span>|<span data-ttu-id="9f102-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="9f102-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9f102-121">承諾</span><span class="sxs-lookup"><span data-stu-id="9f102-121">Accept</span></span>|<span data-ttu-id="9f102-122">アプリケーションまたは json</span><span class="sxs-lookup"><span data-stu-id="9f102-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9f102-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="9f102-123">Request body</span></span>
<span data-ttu-id="9f102-124">要求本文で、[organization](../resources/intune_onboarding_organization.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="9f102-124">In the request body, supply a JSON representation for the [organization](../resources/intune_onboarding_organization.md) object.</span></span>

<span data-ttu-id="9f102-125">次の表に、[organization](../resources/intune_onboarding_organization.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="9f102-125">The following table shows the properties that are required when you create the [organization](../resources/intune_onboarding_organization.md).</span></span>

|<span data-ttu-id="9f102-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9f102-126">Property</span></span>|<span data-ttu-id="9f102-127">タイプ</span><span class="sxs-lookup"><span data-stu-id="9f102-127">Type</span></span>|<span data-ttu-id="9f102-128">説明</span><span class="sxs-lookup"><span data-stu-id="9f102-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9f102-129">ID</span><span class="sxs-lookup"><span data-stu-id="9f102-129">id</span></span>|<span data-ttu-id="9f102-130">文字列</span><span class="sxs-lookup"><span data-stu-id="9f102-130">String</span></span>|<span data-ttu-id="9f102-131">オブジェクトの GUID。</span><span class="sxs-lookup"><span data-stu-id="9f102-131">The GUID for the object.</span></span>|
|<span data-ttu-id="9f102-132">mobileDeviceManagementAuthority</span><span class="sxs-lookup"><span data-stu-id="9f102-132">mobileDeviceManagementAuthority</span></span>|[<span data-ttu-id="9f102-133">mdmAuthority</span><span class="sxs-lookup"><span data-stu-id="9f102-133">mdmAuthority</span></span>](../resources/intune_onboarding_mdmauthority.md)|<span data-ttu-id="9f102-p102">モバイル デバイス管理権限。指定できる値は、`unknown` 、`intune`、`sccm`、`office365` です。</span><span class="sxs-lookup"><span data-stu-id="9f102-p102">Mobile device management authority. The possible values are: `unknown`, `intune`, `sccm`, `office365`.</span></span>|



## <a name="response"></a><span data-ttu-id="9f102-136">応答</span><span class="sxs-lookup"><span data-stu-id="9f102-136">Response</span></span>
<span data-ttu-id="9f102-137">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [organization](../resources/intune_onboarding_organization.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="9f102-137">If successful, this method returns a `200 OK` response code and an updated [organization](../resources/intune_onboarding_organization.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9f102-138">例</span><span class="sxs-lookup"><span data-stu-id="9f102-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="9f102-139">要求</span><span class="sxs-lookup"><span data-stu-id="9f102-139">Request</span></span>
<span data-ttu-id="9f102-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9f102-140">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/organization/{organizationId}
Content-type: application/json
Content-length: 51

{
  "mobileDeviceManagementAuthority": "intune"
}
```

### <a name="response"></a><span data-ttu-id="9f102-141">応答</span><span class="sxs-lookup"><span data-stu-id="9f102-141">Response</span></span>
<span data-ttu-id="9f102-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="9f102-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








