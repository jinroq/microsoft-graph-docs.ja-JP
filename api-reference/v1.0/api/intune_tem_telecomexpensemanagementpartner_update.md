# <a name="update-telecomexpensemanagementpartner"></a><span data-ttu-id="8064b-101">telecomExpenseManagementPartner の更新</span><span class="sxs-lookup"><span data-stu-id="8064b-101">Update telecomExpenseManagementPartner</span></span>

> <span data-ttu-id="8064b-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="8064b-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8064b-103">[telecomExpenseManagementPartner](../resources/intune_tem_telecomexpensemanagementpartner.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="8064b-103">Update the properties of a [calendar](../resources/intune_tem_telecomexpensemanagementpartner.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8064b-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="8064b-104">Prerequisites</span></span>
<span data-ttu-id="8064b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8064b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="8064b-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8064b-107">Permission type</span></span>|<span data-ttu-id="8064b-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="8064b-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8064b-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8064b-109">Delegated (work or school account)</span></span>|<span data-ttu-id="8064b-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8064b-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="8064b-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8064b-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8064b-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8064b-112">Not supported.</span></span>|
|<span data-ttu-id="8064b-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8064b-113">Application</span></span>|<span data-ttu-id="8064b-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8064b-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8064b-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8064b-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/telecomExpenseManagementPartners/{telecomExpenseManagementPartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="8064b-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8064b-116">Request headers</span></span>
|<span data-ttu-id="8064b-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8064b-117">Header</span></span>|<span data-ttu-id="8064b-118">値</span><span class="sxs-lookup"><span data-stu-id="8064b-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8064b-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="8064b-119">Authorization</span></span>|<span data-ttu-id="8064b-120">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="8064b-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="8064b-121">Accept</span><span class="sxs-lookup"><span data-stu-id="8064b-121">Accept</span></span>|<span data-ttu-id="8064b-122">application/json</span><span class="sxs-lookup"><span data-stu-id="8064b-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8064b-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="8064b-123">Request body</span></span>
<span data-ttu-id="8064b-124">要求本文で、[telecomExpenseManagementPartner](../resources/intune_tem_telecomexpensemanagementpartner.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="8064b-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_tem_telecomexpensemanagementpartner.md) object.</span></span>

<span data-ttu-id="8064b-125">次の表に、[telecomExpenseManagementPartner](../resources/intune_tem_telecomexpensemanagementpartner.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="8064b-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="8064b-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8064b-126">Property</span></span>|<span data-ttu-id="8064b-127">型</span><span class="sxs-lookup"><span data-stu-id="8064b-127">Type</span></span>|<span data-ttu-id="8064b-128">説明</span><span class="sxs-lookup"><span data-stu-id="8064b-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8064b-129">id</span><span class="sxs-lookup"><span data-stu-id="8064b-129">id</span></span>|<span data-ttu-id="8064b-130">String</span><span class="sxs-lookup"><span data-stu-id="8064b-130">String</span></span>|<span data-ttu-id="8064b-131">TEM パートナーの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="8064b-131">Unique identifier of the TEM partner.</span></span>|
|<span data-ttu-id="8064b-132">displayName</span><span class="sxs-lookup"><span data-stu-id="8064b-132">displayName</span></span>|<span data-ttu-id="8064b-133">String</span><span class="sxs-lookup"><span data-stu-id="8064b-133">String</span></span>|<span data-ttu-id="8064b-134">TEM パートナーの表示名。</span><span class="sxs-lookup"><span data-stu-id="8064b-134">Display name of the TEM partner.</span></span>|
|<span data-ttu-id="8064b-135">url</span><span class="sxs-lookup"><span data-stu-id="8064b-135">url</span></span>|<span data-ttu-id="8064b-136">String</span><span class="sxs-lookup"><span data-stu-id="8064b-136">String</span></span>|<span data-ttu-id="8064b-137">TEM パートナーの管理用コントロール パネルの URL。管理者は、このパネルで TEM サービスを構成できます。</span><span class="sxs-lookup"><span data-stu-id="8064b-137">URL of the TEM partner's administrative control panel, where an administrator can configure their TEM service.</span></span>|
|<span data-ttu-id="8064b-138">appAuthorized</span><span class="sxs-lookup"><span data-stu-id="8064b-138">appAuthorized</span></span>|<span data-ttu-id="8064b-139">Boolean</span><span class="sxs-lookup"><span data-stu-id="8064b-139">Boolean</span></span>|<span data-ttu-id="8064b-140">パートナーの AAD アプリに Intune へのアクセスが承認されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="8064b-140">Whether the partner's AAD app has been authorized to access Intune.</span></span>|
|<span data-ttu-id="8064b-141">enabled</span><span class="sxs-lookup"><span data-stu-id="8064b-141">enabled</span></span>|<span data-ttu-id="8064b-142">Boolean</span><span class="sxs-lookup"><span data-stu-id="8064b-142">Boolean</span></span>|<span data-ttu-id="8064b-143">TEM サービスへの Intune の接続が現在有効であるか、無効であるかを示します。</span><span class="sxs-lookup"><span data-stu-id="8064b-143">Whether Intune's connection to the TEM service is currently enabled or disabled.</span></span>|
|<span data-ttu-id="8064b-144">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="8064b-144">lastConnectionDateTime</span></span>|<span data-ttu-id="8064b-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="8064b-145">DateTimeOffset</span></span>|<span data-ttu-id="8064b-146">TEM パートナーによって Intune に最後に送信された要求のタイムスタンプ。</span><span class="sxs-lookup"><span data-stu-id="8064b-146">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|



## <a name="response"></a><span data-ttu-id="8064b-147">応答</span><span class="sxs-lookup"><span data-stu-id="8064b-147">Response</span></span>
<span data-ttu-id="8064b-148">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [telecomExpenseManagementPartner](../resources/intune_tem_telecomexpensemanagementpartner.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="8064b-148">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_tem_telecomexpensemanagementpartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8064b-149">例</span><span class="sxs-lookup"><span data-stu-id="8064b-149">Example</span></span>
### <a name="request"></a><span data-ttu-id="8064b-150">要求</span><span class="sxs-lookup"><span data-stu-id="8064b-150">Request</span></span>
<span data-ttu-id="8064b-151">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8064b-151">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/telecomExpenseManagementPartners/{telecomExpenseManagementPartnerId}
Content-type: application/json
Content-length: 178

{
  "displayName": "Display Name value",
  "url": "Url value",
  "appAuthorized": true,
  "enabled": true,
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00"
}
```

### <a name="response"></a><span data-ttu-id="8064b-152">応答</span><span class="sxs-lookup"><span data-stu-id="8064b-152">Response</span></span>
<span data-ttu-id="8064b-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8064b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



