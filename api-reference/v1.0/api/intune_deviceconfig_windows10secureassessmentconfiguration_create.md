# <a name="create-windows10secureassessmentconfiguration"></a><span data-ttu-id="325aa-101">Create windows10SecureAssessmentConfiguration</span><span class="sxs-lookup"><span data-stu-id="325aa-101">Create windows10SecureAssessmentConfiguration</span></span>

> <span data-ttu-id="325aa-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="325aa-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="325aa-103">新しい [windows10SecureAssessmentConfiguration](../resources/intune_deviceconfig_windows10secureassessmentconfiguration.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="325aa-103">Create a new [windows10SecureAssessmentConfiguration](../resources/intune_deviceconfig_windows10secureassessmentconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="325aa-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="325aa-104">Prerequisites</span></span>
<span data-ttu-id="325aa-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="325aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="325aa-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="325aa-107">Permission type</span></span>|<span data-ttu-id="325aa-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="325aa-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="325aa-109">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="325aa-109">Delegated (work or school account)</span></span>|<span data-ttu-id="325aa-110">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="325aa-110">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="325aa-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="325aa-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="325aa-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="325aa-112">Not supported.</span></span>|
|<span data-ttu-id="325aa-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="325aa-113">Application</span></span>|<span data-ttu-id="325aa-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="325aa-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="325aa-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="325aa-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="325aa-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="325aa-116">Request headers</span></span>
|<span data-ttu-id="325aa-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="325aa-117">Header</span></span>|<span data-ttu-id="325aa-118">値</span><span class="sxs-lookup"><span data-stu-id="325aa-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="325aa-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="325aa-119">Authorization</span></span>|<span data-ttu-id="325aa-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="325aa-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="325aa-121">Accept</span><span class="sxs-lookup"><span data-stu-id="325aa-121">Accept</span></span>|<span data-ttu-id="325aa-122">application/json</span><span class="sxs-lookup"><span data-stu-id="325aa-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="325aa-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="325aa-123">Request body</span></span>
<span data-ttu-id="325aa-124">要求本文で、windows10SecureAssessmentConfiguration オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="325aa-124">In the request body, supply a JSON representation for the windows10SecureAssessmentConfiguration object.</span></span>

<span data-ttu-id="325aa-125">次の表に、windows10SecureAssessmentConfiguration の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="325aa-125">The following table shows the properties that are required when you create the windows10SecureAssessmentConfiguration.</span></span>

|<span data-ttu-id="325aa-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="325aa-126">Property</span></span>|<span data-ttu-id="325aa-127">型</span><span class="sxs-lookup"><span data-stu-id="325aa-127">Type</span></span>|<span data-ttu-id="325aa-128">説明</span><span class="sxs-lookup"><span data-stu-id="325aa-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="325aa-129">id</span><span class="sxs-lookup"><span data-stu-id="325aa-129">id</span></span>|<span data-ttu-id="325aa-130">String</span><span class="sxs-lookup"><span data-stu-id="325aa-130">String</span></span>|<span data-ttu-id="325aa-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="325aa-131">Key of the entity.</span></span> <span data-ttu-id="325aa-132">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="325aa-132">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="325aa-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="325aa-133">lastModifiedDateTime</span></span>|<span data-ttu-id="325aa-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="325aa-134">DateTimeOffset</span></span>|<span data-ttu-id="325aa-135">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="325aa-135">DateTime the object was last modified.</span></span> <span data-ttu-id="325aa-136">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="325aa-136">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="325aa-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="325aa-137">createdDateTime</span></span>|<span data-ttu-id="325aa-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="325aa-138">DateTimeOffset</span></span>|<span data-ttu-id="325aa-139">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="325aa-139">DateTime the object was created.</span></span> <span data-ttu-id="325aa-140">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="325aa-140">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="325aa-141">description</span><span class="sxs-lookup"><span data-stu-id="325aa-141">description</span></span>|<span data-ttu-id="325aa-142">String</span><span class="sxs-lookup"><span data-stu-id="325aa-142">String</span></span>|<span data-ttu-id="325aa-143">デバイス構成について管理者が提供した説明。</span><span class="sxs-lookup"><span data-stu-id="325aa-143">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="325aa-144">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="325aa-144">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="325aa-145">displayName</span><span class="sxs-lookup"><span data-stu-id="325aa-145">displayName</span></span>|<span data-ttu-id="325aa-146">String</span><span class="sxs-lookup"><span data-stu-id="325aa-146">String</span></span>|<span data-ttu-id="325aa-147">デバイス構成について管理者が指定した名前。</span><span class="sxs-lookup"><span data-stu-id="325aa-147">Admin provided name of the device configuration.</span></span> <span data-ttu-id="325aa-148">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="325aa-148">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="325aa-149">version</span><span class="sxs-lookup"><span data-stu-id="325aa-149">version</span></span>|<span data-ttu-id="325aa-150">Int32</span><span class="sxs-lookup"><span data-stu-id="325aa-150">Int32</span></span>|<span data-ttu-id="325aa-151">デバイス構成のバージョン。</span><span class="sxs-lookup"><span data-stu-id="325aa-151">Version of the device configuration.</span></span> <span data-ttu-id="325aa-152">[deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="325aa-152">Inherited from [deviceConfiguration](../resources/intune_deviceconfig_deviceconfiguration.md)</span></span>|
|<span data-ttu-id="325aa-153">launchUri</span><span class="sxs-lookup"><span data-stu-id="325aa-153">launchUri</span></span>|<span data-ttu-id="325aa-154">String</span><span class="sxs-lookup"><span data-stu-id="325aa-154">String</span></span>|<span data-ttu-id="325aa-155">安全性評価ブラウザーを起動すると自動的に読み込まれる評価への URL リンク。</span><span class="sxs-lookup"><span data-stu-id="325aa-155">Url link to an assessment that's automatically loaded when the secure assessment browser is launched.</span></span> <span data-ttu-id="325aa-156">有効な URL である必要があります (http\[s\]://msdn.microsoft.com/)。</span><span class="sxs-lookup"><span data-stu-id="325aa-156">It has to be a valid Url (http\[s\]://msdn.microsoft.com/).</span></span>|
|<span data-ttu-id="325aa-157">configurationAccount</span><span class="sxs-lookup"><span data-stu-id="325aa-157">configurationAccount</span></span>|<span data-ttu-id="325aa-158">String</span><span class="sxs-lookup"><span data-stu-id="325aa-158">String</span></span>|<span data-ttu-id="325aa-159">Windows デバイスにテストを受けさせる際に、それを構成するために使用するアカウント。</span><span class="sxs-lookup"><span data-stu-id="325aa-159">The account used to configure the Windows device for taking the test.</span></span> <span data-ttu-id="325aa-160">ユーザーは、ドメイン アカウント (domain\user)、AAD アカウント (username@tenant.com)、ローカル アカウント (username) のいずれでも可能です。</span><span class="sxs-lookup"><span data-stu-id="325aa-160">The user can be a domain account (domain\user), an AAD account (username@tenant.com) or a local account (username).</span></span>|
|<span data-ttu-id="325aa-161">allowPrinting</span><span class="sxs-lookup"><span data-stu-id="325aa-161">allowPrinting</span></span>|<span data-ttu-id="325aa-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="325aa-162">Boolean</span></span>|<span data-ttu-id="325aa-163">テスト中にアプリが印刷することを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="325aa-163">Indicates whether or not to allow the app from printing during the test.</span></span>|
|<span data-ttu-id="325aa-164">allowScreenCapture</span><span class="sxs-lookup"><span data-stu-id="325aa-164">allowScreenCapture</span></span>|<span data-ttu-id="325aa-165">Boolean</span><span class="sxs-lookup"><span data-stu-id="325aa-165">Boolean</span></span>|<span data-ttu-id="325aa-166">テスト中に画面キャプチャ機能を許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="325aa-166">Indicates whether or not to allow screen capture capability during a test.</span></span>|
|<span data-ttu-id="325aa-167">allowTextSuggestion</span><span class="sxs-lookup"><span data-stu-id="325aa-167">allowTextSuggestion</span></span>|<span data-ttu-id="325aa-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="325aa-168">Boolean</span></span>|<span data-ttu-id="325aa-169">テスト中に入力ヒントを許可するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="325aa-169">Indicates whether or not to allow text suggestions during the test.</span></span>|



## <a name="response"></a><span data-ttu-id="325aa-170">応答</span><span class="sxs-lookup"><span data-stu-id="325aa-170">Response</span></span>
<span data-ttu-id="325aa-171">このメソッドが成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [windows10SecureAssessmentConfiguration](../resources/intune_deviceconfig_windows10secureassessmentconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="325aa-171">If successful, this method returns a `201 Created` response code and a [windows10SecureAssessmentConfiguration](../resources/intune_deviceconfig_windows10secureassessmentconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="325aa-172">例</span><span class="sxs-lookup"><span data-stu-id="325aa-172">Example</span></span>
### <a name="request"></a><span data-ttu-id="325aa-173">要求</span><span class="sxs-lookup"><span data-stu-id="325aa-173">Request</span></span>
<span data-ttu-id="325aa-174">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="325aa-174">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
Content-type: application/json
Content-length: 359

{
  "@odata.type": "#microsoft.graph.windows10SecureAssessmentConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "launchUri": "Launch Uri value",
  "configurationAccount": "Configuration Account value",
  "allowPrinting": true,
  "allowScreenCapture": true,
  "allowTextSuggestion": true
}
```

### <a name="response"></a><span data-ttu-id="325aa-175">応答</span><span class="sxs-lookup"><span data-stu-id="325aa-175">Response</span></span>
<span data-ttu-id="325aa-p110">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="325aa-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 531

{
  "@odata.type": "#microsoft.graph.windows10SecureAssessmentConfiguration",
  "id": "f60d71be-71be-f60d-be71-0df6be710df6",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "launchUri": "Launch Uri value",
  "configurationAccount": "Configuration Account value",
  "allowPrinting": true,
  "allowScreenCapture": true,
  "allowTextSuggestion": true
}
```



