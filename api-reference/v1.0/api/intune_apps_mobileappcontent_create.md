# <a name="create-mobileappcontent"></a><span data-ttu-id="f9fd3-101">mobileAppContent の作成</span><span class="sxs-lookup"><span data-stu-id="f9fd3-101">Create mobileAppContent</span></span>

> <span data-ttu-id="f9fd3-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f9fd3-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f9fd3-103">新しい [mobileAppContent](../resources/intune_apps_mobileappcontent.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="f9fd3-103">Create a new [mobileAppContent](../resources/intune_apps_mobileappcontent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f9fd3-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="f9fd3-104">Prerequisites</span></span>
<span data-ttu-id="f9fd3-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f9fd3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="f9fd3-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f9fd3-107">Permission type</span></span>|<span data-ttu-id="f9fd3-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f9fd3-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f9fd3-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f9fd3-109">Delegated (work or school account)</span></span>|<span data-ttu-id="f9fd3-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9fd3-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f9fd3-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f9fd3-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f9fd3-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f9fd3-112">Not supported.</span></span>|
|<span data-ttu-id="f9fd3-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f9fd3-113">Application</span></span>|<span data-ttu-id="f9fd3-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f9fd3-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f9fd3-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f9fd3-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.mobileLobApp/contentVersions
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.managedMobileLobApp/contentVersions
```

## <a name="request-headers"></a><span data-ttu-id="f9fd3-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f9fd3-116">Request headers</span></span>
|<span data-ttu-id="f9fd3-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f9fd3-117">Header</span></span>|<span data-ttu-id="f9fd3-118">値</span><span class="sxs-lookup"><span data-stu-id="f9fd3-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f9fd3-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="f9fd3-119">Authorization</span></span>|<span data-ttu-id="f9fd3-120">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="f9fd3-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f9fd3-121">Accept</span><span class="sxs-lookup"><span data-stu-id="f9fd3-121">Accept</span></span>|<span data-ttu-id="f9fd3-122">application/json</span><span class="sxs-lookup"><span data-stu-id="f9fd3-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f9fd3-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="f9fd3-123">Request body</span></span>
<span data-ttu-id="f9fd3-124">要求本文で、mobileAppContent オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="f9fd3-124">In the request body, supply a JSON representation for the mobileAppContent object.</span></span>

<span data-ttu-id="f9fd3-125">次の表に、mobileAppContent の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="f9fd3-125">The following table shows the properties that are required when you create the mobileAppContent.</span></span>

|<span data-ttu-id="f9fd3-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f9fd3-126">Property</span></span>|<span data-ttu-id="f9fd3-127">型</span><span class="sxs-lookup"><span data-stu-id="f9fd3-127">Type</span></span>|<span data-ttu-id="f9fd3-128">説明</span><span class="sxs-lookup"><span data-stu-id="f9fd3-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f9fd3-129">id</span><span class="sxs-lookup"><span data-stu-id="f9fd3-129">id</span></span>|<span data-ttu-id="f9fd3-130">String</span><span class="sxs-lookup"><span data-stu-id="f9fd3-130">String</span></span>|<span data-ttu-id="f9fd3-131">アプリのコンテンツのバージョン。</span><span class="sxs-lookup"><span data-stu-id="f9fd3-131">The app content version.</span></span>|



## <a name="response"></a><span data-ttu-id="f9fd3-132">応答</span><span class="sxs-lookup"><span data-stu-id="f9fd3-132">Response</span></span>
<span data-ttu-id="f9fd3-133">成功した場合、このメソッドは `201 Created` 応答コードと応答本文で [mobileAppContent](../resources/intune_apps_mobileappcontent.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f9fd3-133">If successful, this method returns a `201 Created` response code and a [mobileAppContent](../resources/intune_apps_mobileappcontent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f9fd3-134">例</span><span class="sxs-lookup"><span data-stu-id="f9fd3-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="f9fd3-135">要求</span><span class="sxs-lookup"><span data-stu-id="f9fd3-135">Request</span></span>
<span data-ttu-id="f9fd3-136">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f9fd3-136">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions
Content-type: application/json
Content-length: 58

{
  "@odata.type": "#microsoft.graph.mobileAppContent"
}
```

### <a name="response"></a><span data-ttu-id="f9fd3-137">応答</span><span class="sxs-lookup"><span data-stu-id="f9fd3-137">Response</span></span>
<span data-ttu-id="f9fd3-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f9fd3-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 107

{
  "@odata.type": "#microsoft.graph.mobileAppContent",
  "id": "fe0bb9a9-b9a9-fe0b-a9b9-0bfea9b90bfe"
}
```



