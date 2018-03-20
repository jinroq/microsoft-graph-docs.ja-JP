# <a name="create-remoteassistancepartner"></a><span data-ttu-id="ee9cb-101">remoteAssistancePartner の作成</span><span class="sxs-lookup"><span data-stu-id="ee9cb-101">Create remoteAssistancePartner</span></span>

> <span data-ttu-id="ee9cb-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ee9cb-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ee9cb-103">新しい [remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="ee9cb-103">Create a new [plannerBucket](../resources/intune_remoteassistance_remoteassistancepartner.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ee9cb-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="ee9cb-104">Prerequisites</span></span>
<span data-ttu-id="ee9cb-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ee9cb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ee9cb-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ee9cb-107">Permission type</span></span>|<span data-ttu-id="ee9cb-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ee9cb-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ee9cb-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ee9cb-109">Delegated (work or school account)</span></span>|<span data-ttu-id="ee9cb-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ee9cb-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="ee9cb-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ee9cb-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ee9cb-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ee9cb-112">Not supported.</span></span>|
|<span data-ttu-id="ee9cb-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ee9cb-113">Application</span></span>|<span data-ttu-id="ee9cb-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ee9cb-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ee9cb-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ee9cb-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/remoteAssistancePartners
```

## <a name="request-headers"></a><span data-ttu-id="ee9cb-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ee9cb-116">Request headers</span></span>
|<span data-ttu-id="ee9cb-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ee9cb-117">Header</span></span>|<span data-ttu-id="ee9cb-118">値</span><span class="sxs-lookup"><span data-stu-id="ee9cb-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ee9cb-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="ee9cb-119">Authorization</span></span>|<span data-ttu-id="ee9cb-120">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="ee9cb-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="ee9cb-121">Accept</span><span class="sxs-lookup"><span data-stu-id="ee9cb-121">Accept</span></span>|<span data-ttu-id="ee9cb-122">application/json</span><span class="sxs-lookup"><span data-stu-id="ee9cb-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ee9cb-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="ee9cb-123">Request body</span></span>
<span data-ttu-id="ee9cb-124">要求本文で、remoteAssistancePartner オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="ee9cb-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="ee9cb-125">次の表に、remoteAssistancePartner の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="ee9cb-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="ee9cb-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ee9cb-126">Property</span></span>|<span data-ttu-id="ee9cb-127">型</span><span class="sxs-lookup"><span data-stu-id="ee9cb-127">Type</span></span>|<span data-ttu-id="ee9cb-128">説明</span><span class="sxs-lookup"><span data-stu-id="ee9cb-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ee9cb-129">id</span><span class="sxs-lookup"><span data-stu-id="ee9cb-129">id</span></span>|<span data-ttu-id="ee9cb-130">String</span><span class="sxs-lookup"><span data-stu-id="ee9cb-130">String</span></span>|<span data-ttu-id="ee9cb-131">パートナーの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="ee9cb-131">Unique identifier of the area.</span></span>|
|<span data-ttu-id="ee9cb-132">displayName</span><span class="sxs-lookup"><span data-stu-id="ee9cb-132">displayName</span></span>|<span data-ttu-id="ee9cb-133">String</span><span class="sxs-lookup"><span data-stu-id="ee9cb-133">String</span></span>|<span data-ttu-id="ee9cb-134">パートナーの表示名。</span><span class="sxs-lookup"><span data-stu-id="ee9cb-134">Display name of the item</span></span>|
|<span data-ttu-id="ee9cb-135">onboardingUrl</span><span class="sxs-lookup"><span data-stu-id="ee9cb-135">onboardingUrl</span></span>|<span data-ttu-id="ee9cb-136">String</span><span class="sxs-lookup"><span data-stu-id="ee9cb-136">String</span></span>|<span data-ttu-id="ee9cb-137">パートナーのオンボーディング ポータルの URL。このポータルでは、管理者がパートナーのリモート アシスタンス サービスを構成できます。</span><span class="sxs-lookup"><span data-stu-id="ee9cb-137">URL of the partner's onboarding portal, where an administrator can configure their Remote Assistance service.</span></span>|
|<span data-ttu-id="ee9cb-138">onboardingStatus</span><span class="sxs-lookup"><span data-stu-id="ee9cb-138">onboardingStatus</span></span>|<span data-ttu-id="ee9cb-139">String</span><span class="sxs-lookup"><span data-stu-id="ee9cb-139">String</span></span>|<span data-ttu-id="ee9cb-140">TBD の可能な値は、`notOnboarded`、`onboarding`、`onboarded` です。</span><span class="sxs-lookup"><span data-stu-id="ee9cb-140">Possible values are: `notOnboarded`, `onboarding`, `onboarded`, .</span></span>|
|<span data-ttu-id="ee9cb-141">lastConnectionDateTime</span><span class="sxs-lookup"><span data-stu-id="ee9cb-141">lastConnectionDateTime</span></span>|<span data-ttu-id="ee9cb-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ee9cb-142">DateTimeOffset</span></span>|<span data-ttu-id="ee9cb-143">TEM パートナーによって Intune に最後に送信された要求のタイムスタンプ。</span><span class="sxs-lookup"><span data-stu-id="ee9cb-143">Timestamp of the last request sent to Intune by the TEM partner.</span></span>|



## <a name="response"></a><span data-ttu-id="ee9cb-144">応答</span><span class="sxs-lookup"><span data-stu-id="ee9cb-144">Response</span></span>
<span data-ttu-id="ee9cb-145">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [remoteAssistancePartner](../resources/intune_remoteassistance_remoteassistancepartner.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ee9cb-145">If successful, this method returns a `201 Created` response code and a [DriveItemVersion](../resources/intune_remoteassistance_remoteassistancepartner.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ee9cb-146">例</span><span class="sxs-lookup"><span data-stu-id="ee9cb-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="ee9cb-147">要求</span><span class="sxs-lookup"><span data-stu-id="ee9cb-147">Request</span></span>
<span data-ttu-id="ee9cb-148">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ee9cb-148">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/remoteAssistancePartners
Content-type: application/json
Content-length: 266

{
  "@odata.type": "#microsoft.graph.remoteAssistancePartner",
  "displayName": "Display Name value",
  "onboardingUrl": "https://example.com/onboardingUrl/",
  "onboardingStatus": "onboarding",
  "lastConnectionDateTime": "2016-12-31T23:58:36.6670033-08:00"
}
```

### <a name="response"></a><span data-ttu-id="ee9cb-149">応答</span><span class="sxs-lookup"><span data-stu-id="ee9cb-149">Response</span></span>
<span data-ttu-id="ee9cb-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ee9cb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



