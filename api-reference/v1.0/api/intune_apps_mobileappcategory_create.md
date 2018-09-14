# <a name="create-mobileappcategory"></a><span data-ttu-id="0c6f5-101">mobileAppCategory の作成</span><span class="sxs-lookup"><span data-stu-id="0c6f5-101">Create mobileAppCategory</span></span>

> <span data-ttu-id="0c6f5-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="0c6f5-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0c6f5-103">新しい [mobileAppCategory](../resources/intune_apps_mobileappcategory.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="0c6f5-103">Create a new [mobileAppCategory](../resources/intune_apps_mobileappcategory.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0c6f5-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="0c6f5-104">Prerequisites</span></span>
<span data-ttu-id="0c6f5-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0c6f5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="0c6f5-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0c6f5-107">Permission type</span></span>|<span data-ttu-id="0c6f5-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="0c6f5-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0c6f5-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0c6f5-109">Delegated (work or school account)</span></span>|<span data-ttu-id="0c6f5-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c6f5-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0c6f5-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0c6f5-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0c6f5-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0c6f5-112">Not supported.</span></span>|
|<span data-ttu-id="0c6f5-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0c6f5-113">Application</span></span>|<span data-ttu-id="0c6f5-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0c6f5-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0c6f5-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0c6f5-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileAppCategories
POST /deviceAppManagement/mobileApps/{mobileAppId}/categories
```

## <a name="request-headers"></a><span data-ttu-id="0c6f5-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0c6f5-116">Request headers</span></span>
|<span data-ttu-id="0c6f5-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0c6f5-117">Header</span></span>|<span data-ttu-id="0c6f5-118">値</span><span class="sxs-lookup"><span data-stu-id="0c6f5-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0c6f5-119">承認</span><span class="sxs-lookup"><span data-stu-id="0c6f5-119">Authorization</span></span>|<span data-ttu-id="0c6f5-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="0c6f5-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0c6f5-121">受け入れる</span><span class="sxs-lookup"><span data-stu-id="0c6f5-121">Accept</span></span>|<span data-ttu-id="0c6f5-122">アプリケーションまたは json</span><span class="sxs-lookup"><span data-stu-id="0c6f5-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0c6f5-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="0c6f5-123">Request body</span></span>
<span data-ttu-id="0c6f5-124">要求本文で、mobileAppCategory オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="0c6f5-124">In the request body, supply a JSON representation for the mobileAppCategory object.</span></span>

<span data-ttu-id="0c6f5-125">次の表に、mobileAppCategory の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="0c6f5-125">The following table shows the properties that are required when you create the mobileAppCategory.</span></span>

|<span data-ttu-id="0c6f5-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0c6f5-126">Property</span></span>|<span data-ttu-id="0c6f5-127">型</span><span class="sxs-lookup"><span data-stu-id="0c6f5-127">Type</span></span>|<span data-ttu-id="0c6f5-128">説明</span><span class="sxs-lookup"><span data-stu-id="0c6f5-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c6f5-129">ID</span><span class="sxs-lookup"><span data-stu-id="0c6f5-129">id</span></span>|<span data-ttu-id="0c6f5-130">文字列</span><span class="sxs-lookup"><span data-stu-id="0c6f5-130">String</span></span>|<span data-ttu-id="0c6f5-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="0c6f5-131">The key of the entity.</span></span>|
|<span data-ttu-id="0c6f5-132">displayName</span><span class="sxs-lookup"><span data-stu-id="0c6f5-132">displayName</span></span>|<span data-ttu-id="0c6f5-133">文字列</span><span class="sxs-lookup"><span data-stu-id="0c6f5-133">String</span></span>|<span data-ttu-id="0c6f5-134">アプリのカテゴリの名前。</span><span class="sxs-lookup"><span data-stu-id="0c6f5-134">The name of the app category.</span></span>|
|<span data-ttu-id="0c6f5-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0c6f5-135">lastModifiedDateTime</span></span>|<span data-ttu-id="0c6f5-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0c6f5-136">DateTimeOffset</span></span>|<span data-ttu-id="0c6f5-137">mobileAppCategory が最後に変更された日時。</span><span class="sxs-lookup"><span data-stu-id="0c6f5-137">The date and time the mobileAppCategory was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="0c6f5-138">応答</span><span class="sxs-lookup"><span data-stu-id="0c6f5-138">Response</span></span>
<span data-ttu-id="0c6f5-139">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [mobileAppCategory](../resources/intune_apps_mobileappcategory.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="0c6f5-139">If successful, this method returns a `201 Created` response code and a [mobileAppCategory](../resources/intune_apps_mobileappcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0c6f5-140">例</span><span class="sxs-lookup"><span data-stu-id="0c6f5-140">Example</span></span>
### <a name="request"></a><span data-ttu-id="0c6f5-141">要求</span><span class="sxs-lookup"><span data-stu-id="0c6f5-141">Request</span></span>
<span data-ttu-id="0c6f5-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0c6f5-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppCategories
Content-type: application/json
Content-length: 163

{
  "@odata.type": "#microsoft.graph.mobileAppCategory",
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```

### <a name="response"></a><span data-ttu-id="0c6f5-143">応答</span><span class="sxs-lookup"><span data-stu-id="0c6f5-143">Response</span></span>
<span data-ttu-id="0c6f5-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0c6f5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 212

{
  "@odata.type": "#microsoft.graph.mobileAppCategory",
  "id": "d85d9cee-9cee-d85d-ee9c-5dd8ee9c5dd8",
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```








