# <a name="update-targetedmanagedappconfiguration"></a><span data-ttu-id="ae977-101">targetedManagedAppConfiguration の更新</span><span class="sxs-lookup"><span data-stu-id="ae977-101">Update targetedManagedAppConfiguration</span></span>

> <span data-ttu-id="ae977-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ae977-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ae977-103">[targetedManagedAppConfiguration](../resources/intune_mam_targetedmanagedappconfiguration.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="ae977-103">Update the properties of a [targetedManagedAppConfiguration](../resources/intune_mam_targetedmanagedappconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ae977-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="ae977-104">Prerequisites</span></span>
<span data-ttu-id="ae977-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ae977-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ae977-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ae977-107">Permission type</span></span>|<span data-ttu-id="ae977-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ae977-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ae977-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ae977-109">Delegated (work or school account)</span></span>|<span data-ttu-id="ae977-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae977-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ae977-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ae977-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ae977-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ae977-112">Not supported.</span></span>|
|<span data-ttu-id="ae977-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ae977-113">Application</span></span>|<span data-ttu-id="ae977-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ae977-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ae977-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ae977-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="ae977-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ae977-116">Request headers</span></span>
|<span data-ttu-id="ae977-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ae977-117">Header</span></span>|<span data-ttu-id="ae977-118">値</span><span class="sxs-lookup"><span data-stu-id="ae977-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ae977-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="ae977-119">Authorization</span></span>|<span data-ttu-id="ae977-120">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="ae977-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ae977-121">Accept</span><span class="sxs-lookup"><span data-stu-id="ae977-121">Accept</span></span>|<span data-ttu-id="ae977-122">application/json</span><span class="sxs-lookup"><span data-stu-id="ae977-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ae977-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="ae977-123">Request body</span></span>
<span data-ttu-id="ae977-124">要求本文で、[targetedManagedAppConfiguration](../resources/intune_mam_targetedmanagedappconfiguration.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="ae977-124">In the request body, supply a JSON representation for the [targetedManagedAppConfiguration](../resources/intune_mam_targetedmanagedappconfiguration.md) object.</span></span>

<span data-ttu-id="ae977-125">次の表に、[targetedManagedAppConfiguration](../resources/intune_mam_targetedmanagedappconfiguration.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="ae977-125">The following table shows the properties that are required when you create the [targetedManagedAppConfiguration](../resources/intune_mam_targetedmanagedappconfiguration.md).</span></span>

|<span data-ttu-id="ae977-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ae977-126">Property</span></span>|<span data-ttu-id="ae977-127">型</span><span class="sxs-lookup"><span data-stu-id="ae977-127">Type</span></span>|<span data-ttu-id="ae977-128">説明</span><span class="sxs-lookup"><span data-stu-id="ae977-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ae977-129">displayName</span><span class="sxs-lookup"><span data-stu-id="ae977-129">displayName</span></span>|<span data-ttu-id="ae977-130">String</span><span class="sxs-lookup"><span data-stu-id="ae977-130">String</span></span>|<span data-ttu-id="ae977-131">ポリシーの表示名。</span><span class="sxs-lookup"><span data-stu-id="ae977-131">Policy display name.</span></span> <span data-ttu-id="ae977-132">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ae977-132">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="ae977-133">description</span><span class="sxs-lookup"><span data-stu-id="ae977-133">description</span></span>|<span data-ttu-id="ae977-134">String</span><span class="sxs-lookup"><span data-stu-id="ae977-134">String</span></span>|<span data-ttu-id="ae977-135">ポリシーの説明。</span><span class="sxs-lookup"><span data-stu-id="ae977-135">The policy's description.</span></span> <span data-ttu-id="ae977-136">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ae977-136">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="ae977-137">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ae977-137">createdDateTime</span></span>|<span data-ttu-id="ae977-138">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ae977-138">DateTimeOffset</span></span>|<span data-ttu-id="ae977-139">ポリシーが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="ae977-139">The date and time the policy was created.</span></span> <span data-ttu-id="ae977-140">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ae977-140">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="ae977-141">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ae977-141">lastModifiedDateTime</span></span>|<span data-ttu-id="ae977-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ae977-142">DateTimeOffset</span></span>|<span data-ttu-id="ae977-143">ポリシーが変更された最終日時。</span><span class="sxs-lookup"><span data-stu-id="ae977-143">Last time the policy was modified.</span></span> <span data-ttu-id="ae977-144">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ae977-144">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="ae977-145">id</span><span class="sxs-lookup"><span data-stu-id="ae977-145">id</span></span>|<span data-ttu-id="ae977-146">String</span><span class="sxs-lookup"><span data-stu-id="ae977-146">String</span></span>|<span data-ttu-id="ae977-147">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="ae977-147">Key of the entity.</span></span> <span data-ttu-id="ae977-148">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ae977-148">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="ae977-149">version</span><span class="sxs-lookup"><span data-stu-id="ae977-149">version</span></span>|<span data-ttu-id="ae977-150">String</span><span class="sxs-lookup"><span data-stu-id="ae977-150">String</span></span>|<span data-ttu-id="ae977-151">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="ae977-151">Version of the entity.</span></span> <span data-ttu-id="ae977-152">[managedAppPolicy](../resources/intune_mam_managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ae977-152">Inherited from [managedAppPolicy](../resources/intune_mam_managedapppolicy.md)</span></span>|
|<span data-ttu-id="ae977-153">customSettings</span><span class="sxs-lookup"><span data-stu-id="ae977-153">customSettings</span></span>|<span data-ttu-id="ae977-154">[keyValuePair](../resources/intune_mam_keyvaluepair.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ae977-154">[keyValuePair](../resources/intune_mam_keyvaluepair.md) collection</span></span>|<span data-ttu-id="ae977-155">構成の対象であるユーザーに対して、このサービスで変更せずにアプリに送信される文字列キーと文字列値の一連のペア。[managedAppConfiguration](../resources/intune_mam_managedappconfiguration.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ae977-155">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service Inherited from [managedAppConfiguration](../resources/intune_mam_managedappconfiguration.md)</span></span>|
|<span data-ttu-id="ae977-156">deployedAppCount</span><span class="sxs-lookup"><span data-stu-id="ae977-156">deployedAppCount</span></span>|<span data-ttu-id="ae977-157">Int32</span><span class="sxs-lookup"><span data-stu-id="ae977-157">Int32</span></span>|<span data-ttu-id="ae977-158">現在のポリシーが配置されたアプリの数。</span><span class="sxs-lookup"><span data-stu-id="ae977-158">Count of apps to which the current policy is deployed.</span></span>|
|<span data-ttu-id="ae977-159">isAssigned</span><span class="sxs-lookup"><span data-stu-id="ae977-159">isAssigned</span></span>|<span data-ttu-id="ae977-160">Boolean</span><span class="sxs-lookup"><span data-stu-id="ae977-160">Boolean</span></span>|<span data-ttu-id="ae977-161">包含グループにポリシーを配置するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="ae977-161">Indicates if the policy is deployed to any inclusion groups or not.</span></span>|



## <a name="response"></a><span data-ttu-id="ae977-162">応答</span><span class="sxs-lookup"><span data-stu-id="ae977-162">Response</span></span>
<span data-ttu-id="ae977-163">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [targetedManagedAppConfiguration](../resources/intune_mam_targetedmanagedappconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ae977-163">If successful, this method returns a `200 OK` response code and an updated [targetedManagedAppConfiguration](../resources/intune_mam_targetedmanagedappconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae977-164">例</span><span class="sxs-lookup"><span data-stu-id="ae977-164">Example</span></span>
### <a name="request"></a><span data-ttu-id="ae977-165">要求</span><span class="sxs-lookup"><span data-stu-id="ae977-165">Request</span></span>
<span data-ttu-id="ae977-166">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ae977-166">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
Content-type: application/json
Content-length: 388

{
  "@odata.type": "#microsoft.graph.targetedManagedAppConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "version": "Version value",
  "customSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "deployedAppCount": 0,
  "isAssigned": true
}
```

### <a name="response"></a><span data-ttu-id="ae977-167">応答</span><span class="sxs-lookup"><span data-stu-id="ae977-167">Response</span></span>
<span data-ttu-id="ae977-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ae977-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 560

{
  "@odata.type": "#microsoft.graph.targetedManagedAppConfiguration",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "id": "2444e029-e029-2444-29e0-442429e04424",
  "version": "Version value",
  "customSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "Name value",
      "value": "Value value"
    }
  ],
  "deployedAppCount": 0,
  "isAssigned": true
}
```



