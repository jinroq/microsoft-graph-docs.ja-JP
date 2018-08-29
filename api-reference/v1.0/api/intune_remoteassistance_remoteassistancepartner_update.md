# <a name="update-remoteassistancepartner"></a><span data-ttu-id="baeed-101">remoteAssistancePartner の更新</span><span class="sxs-lookup"><span data-stu-id="baeed-101">Update remoteAssistancePartner</span></span>

> <span data-ttu-id="baeed-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="baeed-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="baeed-103">[remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="baeed-103">Update the properties of a [remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="baeed-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="baeed-104">Prerequisites</span></span>
<span data-ttu-id="baeed-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="baeed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="baeed-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="baeed-107">Permission type</span></span>|<span data-ttu-id="baeed-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="baeed-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="baeed-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="baeed-109">Delegated (work or school account)</span></span>|<span data-ttu-id="baeed-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="baeed-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="baeed-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="baeed-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="baeed-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="baeed-112">Not supported.</span></span>|
|<span data-ttu-id="baeed-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="baeed-113">Application</span></span>|<span data-ttu-id="baeed-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="baeed-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="baeed-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="baeed-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}
```

## <a name="request-headers"></a><span data-ttu-id="baeed-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="baeed-116">Request headers</span></span>
|<span data-ttu-id="baeed-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="baeed-117">Header</span></span>|<span data-ttu-id="baeed-118">値</span><span class="sxs-lookup"><span data-stu-id="baeed-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="baeed-119">承認</span><span class="sxs-lookup"><span data-stu-id="baeed-119">Authorization</span></span>|<span data-ttu-id="baeed-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="baeed-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="baeed-121">承諾</span><span class="sxs-lookup"><span data-stu-id="baeed-121">Accept</span></span>|<span data-ttu-id="baeed-122">application/json</span><span class="sxs-lookup"><span data-stu-id="baeed-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="baeed-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="baeed-123">Request body</span></span>
<span data-ttu-id="baeed-124">要求本文で、[remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="baeed-124">In the request body, supply a JSON representation for the [remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md) object.</span></span>

<span data-ttu-id="baeed-125">次の表に、[remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="baeed-125">The following table shows the properties that are required when you create the [remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md).</span></span>

|<span data-ttu-id="baeed-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="baeed-126">Property</span></span>|<span data-ttu-id="baeed-127">タイプ</span><span class="sxs-lookup"><span data-stu-id="baeed-127">Type</span></span>|<span data-ttu-id="baeed-128">説明</span><span class="sxs-lookup"><span data-stu-id="baeed-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="baeed-129">ID</span><span class="sxs-lookup"><span data-stu-id="baeed-129">id</span></span>|<span data-ttu-id="baeed-130">文字列</span><span class="sxs-lookup"><span data-stu-id="baeed-130">String</span></span>|<span data-ttu-id="baeed-131">パートナーの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="baeed-131">Unique identifier of the partner.</span></span>|
|<span data-ttu-id="baeed-132">displayName</span><span class="sxs-lookup"><span data-stu-id="baeed-132">displayName</span></span>|<span data-ttu-id="baeed-133">文字列</span><span class="sxs-lookup"><span data-stu-id="baeed-133">String</span></span>|<span data-ttu-id="baeed-134">パートナーの表示名。</span><span class="sxs-lookup"><span data-stu-id="baeed-134">Display name of the partner.</span></span>|
|<span data-ttu-id="baeed-135">onboardingUrl</span><span class="sxs-lookup"><span data-stu-id="baeed-135">onboardingUrl</span></span>|<span data-ttu-id="baeed-136">文字列</span><span class="sxs-lookup"><span data-stu-id="baeed-136">String</span></span>|<span data-ttu-id="baeed-137">パートナーのオンボーディング ポータルの URL。このポータルでは、管理者がパートナーのリモート アシスタンス サービスを構成できます。</span><span class="sxs-lookup"><span data-stu-id="baeed-137">URL of the partner's onboarding portal, where an administrator can configure their Remote Assistance service.</span></span>|
|<span data-ttu-id="baeed-138">onboardingStatus</span><span class="sxs-lookup"><span data-stu-id="baeed-138">onboardingStatus</span></span>|[<span data-ttu-id="baeed-139">remoteAssistanceOnboardingStatus</span><span class="sxs-lookup"><span data-stu-id="baeed-139">remoteAssistanceOnboardingStatus</span></span>](../resources/intune_remoteassistance_remoteassistanceonboardingstatus.md)|<span data-ttu-id="baeed-140">未定</span><span class="sxs-lookup"><span data-stu-id="baeed-140">TBD</span></span> <span data-ttu-id="baeed-141">可能な値は、 `notOnboarded`、`onboarding`、`onboarded` です。</span><span class="sxs-lookup"><span data-stu-id="baeed-141">The possible values are `notOnboarded`, `onboarding`, or `onboarded`.</span></span>|
|<span data-ttu-id="baeed-142">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="baeed-142">lastConnectionDateTime</span></span>|<span data-ttu-id="baeed-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="baeed-143">DateTimeOffset</span></span>|<span data-ttu-id="baeed-144">TEM パートナーによって Intune に最後に送信された要求のタイムスタンプ。</span><span class="sxs-lookup"><span data-stu-id="baeed-144">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|



## <a name="response"></a><span data-ttu-id="baeed-145">応答</span><span class="sxs-lookup"><span data-stu-id="baeed-145">Response</span></span>
<span data-ttu-id="baeed-146">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="baeed-146">If successful, this method returns a `200 OK` response code and an updated [remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="baeed-147">例</span><span class="sxs-lookup"><span data-stu-id="baeed-147">Example</span></span>
### <a name="request"></a><span data-ttu-id="baeed-148">要求</span><span class="sxs-lookup"><span data-stu-id="baeed-148">Request</span></span>
<span data-ttu-id="baeed-149">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="baeed-149">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/remoteAssistancePartners/{remoteAssistancePartnerId}
Content-type: application/json
Content-length: 204

{
  "displayName": "Display Name value",
  "onboardingUrl": "https://example.com/onboardingUrl/",
  "onboardingStatus": "onboarding",
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00"
}
```

### <a name="response"></a><span data-ttu-id="baeed-150">応答</span><span class="sxs-lookup"><span data-stu-id="baeed-150">Response</span></span>
<span data-ttu-id="baeed-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="baeed-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 315

{
  "@odata.type": "#microsoft.graph.remoteAssistancePartner",
  "id": "7443c8b9-c8b9-7443-b9c8-4374b9c84374",
  "displayName": "Display Name value",
  "onboardingUrl": "https://example.com/onboardingUrl/",
  "onboardingStatus": "onboarding",
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00"
}
```



