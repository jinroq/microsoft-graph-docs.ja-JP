# <a name="create-telecomexpensemanagementpartner"></a><span data-ttu-id="bbf9c-101">telecomExpenseManagementPartner の作成</span><span class="sxs-lookup"><span data-stu-id="bbf9c-101">Create telecomExpenseManagementPartner</span></span>

> <span data-ttu-id="bbf9c-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="bbf9c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="bbf9c-103">新しい [telecomExpenseManagementPartner](../resources/intune_tem_telecomexpensemanagementpartner.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="bbf9c-103">Create a new [telecomExpenseManagementPartner](../resources/intune_tem_telecomexpensemanagementpartner.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="bbf9c-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="bbf9c-104">Prerequisites</span></span>
<span data-ttu-id="bbf9c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bbf9c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="bbf9c-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="bbf9c-107">Permission type</span></span>|<span data-ttu-id="bbf9c-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="bbf9c-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bbf9c-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="bbf9c-109">Delegated (work or school account)</span></span>|<span data-ttu-id="bbf9c-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bbf9c-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="bbf9c-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="bbf9c-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bbf9c-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bbf9c-112">Not supported.</span></span>|
|<span data-ttu-id="bbf9c-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="bbf9c-113">Application</span></span>|<span data-ttu-id="bbf9c-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="bbf9c-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="bbf9c-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="bbf9c-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/telecomExpenseManagementPartners
```

## <a name="request-headers"></a><span data-ttu-id="bbf9c-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bbf9c-116">Request headers</span></span>
|<span data-ttu-id="bbf9c-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="bbf9c-117">Header</span></span>|<span data-ttu-id="bbf9c-118">値</span><span class="sxs-lookup"><span data-stu-id="bbf9c-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bbf9c-119">承認</span><span class="sxs-lookup"><span data-stu-id="bbf9c-119">Authorization</span></span>|<span data-ttu-id="bbf9c-120">ベアラー &lt;トークン&gt;が必須。</span><span class="sxs-lookup"><span data-stu-id="bbf9c-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bbf9c-121">承諾</span><span class="sxs-lookup"><span data-stu-id="bbf9c-121">Accept</span></span>|<span data-ttu-id="bbf9c-122">application/json</span><span class="sxs-lookup"><span data-stu-id="bbf9c-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bbf9c-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="bbf9c-123">Request body</span></span>
<span data-ttu-id="bbf9c-124">要求本文で、telecomExpenseManagementPartner オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="bbf9c-124">In the request body, supply a JSON representation for the telecomExpenseManagementPartner object.</span></span>

<span data-ttu-id="bbf9c-125">次の表に、telecomExpenseManagementPartner の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="bbf9c-125">The following table shows the properties that are required when you create the telecomExpenseManagementPartner.</span></span>

|<span data-ttu-id="bbf9c-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="bbf9c-126">Property</span></span>|<span data-ttu-id="bbf9c-127">型</span><span class="sxs-lookup"><span data-stu-id="bbf9c-127">Type</span></span>|<span data-ttu-id="bbf9c-128">説明</span><span class="sxs-lookup"><span data-stu-id="bbf9c-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bbf9c-129">id</span><span class="sxs-lookup"><span data-stu-id="bbf9c-129">id</span></span>|<span data-ttu-id="bbf9c-130">String</span><span class="sxs-lookup"><span data-stu-id="bbf9c-130">String</span></span>|<span data-ttu-id="bbf9c-131">TEM パートナーの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="bbf9c-131">Unique identifier of the TEM partner.</span></span>|
|<span data-ttu-id="bbf9c-132">displayName</span><span class="sxs-lookup"><span data-stu-id="bbf9c-132">displayName</span></span>|<span data-ttu-id="bbf9c-133">String</span><span class="sxs-lookup"><span data-stu-id="bbf9c-133">String</span></span>|<span data-ttu-id="bbf9c-134">TEM パートナーの表示名。</span><span class="sxs-lookup"><span data-stu-id="bbf9c-134">Display name of the TEM partner.</span></span>|
|<span data-ttu-id="bbf9c-135">url</span><span class="sxs-lookup"><span data-stu-id="bbf9c-135">url</span></span>|<span data-ttu-id="bbf9c-136">String</span><span class="sxs-lookup"><span data-stu-id="bbf9c-136">String</span></span>|<span data-ttu-id="bbf9c-137">TEM パートナーの管理用コントロール パネルの URL。管理者はここで TEM サービスを構成できます。</span><span class="sxs-lookup"><span data-stu-id="bbf9c-137">URL of the TEM partner's administrative control panel, where an administrator can configure their TEM service.</span></span>|
|<span data-ttu-id="bbf9c-138">appAuthorized</span><span class="sxs-lookup"><span data-stu-id="bbf9c-138">appAuthorized</span></span>|<span data-ttu-id="bbf9c-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="bbf9c-139">Boolean</span></span>|<span data-ttu-id="bbf9c-140">パートナーの AAD アプリに Intune へのアクセスが承認されているかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="bbf9c-140">Whether the partner's AAD app has been authorized to access Intune.</span></span>|
|<span data-ttu-id="bbf9c-141">enabled</span><span class="sxs-lookup"><span data-stu-id="bbf9c-141">enabled</span></span>|<span data-ttu-id="bbf9c-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="bbf9c-142">Boolean</span></span>|<span data-ttu-id="bbf9c-143">TEM サービスへの Intune の接続が現在有効であるか、無効であるかを指定します。</span><span class="sxs-lookup"><span data-stu-id="bbf9c-143">Whether Intune's connection to the TEM service is currently enabled or disabled.</span></span>|
|<span data-ttu-id="bbf9c-144">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="bbf9c-144">lastConnectionDateTime</span></span>|<span data-ttu-id="bbf9c-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bbf9c-145">DateTimeOffset</span></span>|<span data-ttu-id="bbf9c-146">TEM パートナーによって Intune に最後に送信された要求のタイムスタンプ。</span><span class="sxs-lookup"><span data-stu-id="bbf9c-146">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|



## <a name="response"></a><span data-ttu-id="bbf9c-147">応答</span><span class="sxs-lookup"><span data-stu-id="bbf9c-147">Response</span></span>
<span data-ttu-id="bbf9c-148">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [telecomExpenseManagementPartner](../resources/intune_tem_telecomexpensemanagementpartner.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="bbf9c-148">If successful, this method returns a `201 Created` response code and a [telecomExpenseManagementPartner](../resources/intune_tem_telecomexpensemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bbf9c-149">例</span><span class="sxs-lookup"><span data-stu-id="bbf9c-149">Example</span></span>
### <a name="request"></a><span data-ttu-id="bbf9c-150">要求</span><span class="sxs-lookup"><span data-stu-id="bbf9c-150">Request</span></span>
<span data-ttu-id="bbf9c-151">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="bbf9c-151">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/telecomExpenseManagementPartners
Content-type: application/json
Content-length: 248

{
  "@odata.type": "#microsoft.graph.telecomExpenseManagementPartner",
  "displayName": "Display Name value",
  "url": "Url value",
  "appAuthorized": true,
  "enabled": true,
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00"
}
```

### <a name="response"></a><span data-ttu-id="bbf9c-152">応答</span><span class="sxs-lookup"><span data-stu-id="bbf9c-152">Response</span></span>
<span data-ttu-id="bbf9c-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="bbf9c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 297

{
  "@odata.type": "#microsoft.graph.telecomExpenseManagementPartner",
  "id": "47a3b399-b399-47a3-99b3-a34799b3a347",
  "displayName": "Display Name value",
  "url": "Url value",
  "appAuthorized": true,
  "enabled": true,
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00"
}
```



