# <a name="update-mobileappcontent"></a><span data-ttu-id="5f076-101">mobileAppContent の更新</span><span class="sxs-lookup"><span data-stu-id="5f076-101">Update mobileAppContent</span></span>

> <span data-ttu-id="5f076-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="5f076-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5f076-103">[mobileAppContent](../resources/intune_apps_mobileappcontent.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="5f076-103">Update the properties of a [calendar](../resources/intune_apps_mobileappcontent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5f076-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="5f076-104">Prerequisites</span></span>
<span data-ttu-id="5f076-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5f076-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5f076-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5f076-107">Permission type</span></span>|<span data-ttu-id="5f076-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="5f076-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5f076-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5f076-109">Delegated (work or school account)</span></span>|<span data-ttu-id="5f076-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5f076-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5f076-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5f076-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5f076-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5f076-112">Not supported.</span></span>|
|<span data-ttu-id="5f076-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5f076-113">Application</span></span>|<span data-ttu-id="5f076-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5f076-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5f076-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5f076-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.mobileLobApp/contentVersions/{mobileAppContentId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.managedMobileLobApp/contentVersions/{mobileAppContentId}
```

## <a name="request-headers"></a><span data-ttu-id="5f076-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5f076-116">Request headers</span></span>
|<span data-ttu-id="5f076-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5f076-117">Header</span></span>|<span data-ttu-id="5f076-118">値</span><span class="sxs-lookup"><span data-stu-id="5f076-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5f076-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="5f076-119">Authorization</span></span>|<span data-ttu-id="5f076-120">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="5f076-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="5f076-121">Accept</span><span class="sxs-lookup"><span data-stu-id="5f076-121">Accept</span></span>|<span data-ttu-id="5f076-122">application/json</span><span class="sxs-lookup"><span data-stu-id="5f076-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5f076-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="5f076-123">Request body</span></span>
<span data-ttu-id="5f076-124">要求本文で、[mobileAppContent](../resources/intune_apps_mobileappcontent.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="5f076-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_apps_mobileappcontent.md) object.</span></span>

<span data-ttu-id="5f076-125">次の表に、[mobileAppContent](../resources/intune_apps_mobileappcontent.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="5f076-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="5f076-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5f076-126">Property</span></span>|<span data-ttu-id="5f076-127">型</span><span class="sxs-lookup"><span data-stu-id="5f076-127">Type</span></span>|<span data-ttu-id="5f076-128">説明</span><span class="sxs-lookup"><span data-stu-id="5f076-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5f076-129">id</span><span class="sxs-lookup"><span data-stu-id="5f076-129">id</span></span>|<span data-ttu-id="5f076-130">String</span><span class="sxs-lookup"><span data-stu-id="5f076-130">String</span></span>|<span data-ttu-id="5f076-131">アプリのコンテンツのバージョン。</span><span class="sxs-lookup"><span data-stu-id="5f076-131">The app content version.</span></span>|



## <a name="response"></a><span data-ttu-id="5f076-132">応答</span><span class="sxs-lookup"><span data-stu-id="5f076-132">Response</span></span>
<span data-ttu-id="5f076-133">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [mobileAppContent](../resources/intune_apps_mobileappcontent.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="5f076-133">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_apps_mobileappcontent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5f076-134">例</span><span class="sxs-lookup"><span data-stu-id="5f076-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="5f076-135">要求</span><span class="sxs-lookup"><span data-stu-id="5f076-135">Request</span></span>
<span data-ttu-id="5f076-136">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5f076-136">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="5f076-137">応答</span><span class="sxs-lookup"><span data-stu-id="5f076-137">Response</span></span>
<span data-ttu-id="5f076-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="5f076-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 107

{
  "@odata.type": "#microsoft.graph.mobileAppContent",
  "id": "fe0bb9a9-b9a9-fe0b-a9b9-0bfea9b90bfe"
}
```



