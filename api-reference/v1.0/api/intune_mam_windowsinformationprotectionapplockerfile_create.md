# <a name="create-windowsinformationprotectionapplockerfile"></a><span data-ttu-id="97ef7-101">windowsInformationProtectionAppLockerFile の作成</span><span class="sxs-lookup"><span data-stu-id="97ef7-101">Create windowsInformationProtectionAppLockerFile</span></span>

> <span data-ttu-id="97ef7-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="97ef7-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="97ef7-103">新しい [windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="97ef7-103">Create a new [windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="97ef7-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="97ef7-104">Prerequisites</span></span>
<span data-ttu-id="97ef7-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="97ef7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="97ef7-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="97ef7-107">Permission type</span></span>|<span data-ttu-id="97ef7-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="97ef7-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="97ef7-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="97ef7-109">Delegated (work or school account)</span></span>|<span data-ttu-id="97ef7-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="97ef7-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="97ef7-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="97ef7-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="97ef7-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="97ef7-112">Not supported.</span></span>|
|<span data-ttu-id="97ef7-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="97ef7-113">Application</span></span>|<span data-ttu-id="97ef7-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="97ef7-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="97ef7-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="97ef7-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles
POST /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/protectedAppLockerFiles
POST /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/exemptAppLockerFiles
POST /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/protectedAppLockerFiles
```

## <a name="request-headers"></a><span data-ttu-id="97ef7-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="97ef7-116">Request headers</span></span>
|<span data-ttu-id="97ef7-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="97ef7-117">Header</span></span>|<span data-ttu-id="97ef7-118">値</span><span class="sxs-lookup"><span data-stu-id="97ef7-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="97ef7-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="97ef7-119">Authorization</span></span>|<span data-ttu-id="97ef7-120">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="97ef7-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="97ef7-121">Accept</span><span class="sxs-lookup"><span data-stu-id="97ef7-121">Accept</span></span>|<span data-ttu-id="97ef7-122">application/json</span><span class="sxs-lookup"><span data-stu-id="97ef7-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="97ef7-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="97ef7-123">Request body</span></span>
<span data-ttu-id="97ef7-124">要求本文で、windowsInformationProtectionAppLockerFile オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="97ef7-124">In the request body, supply a JSON representation for the windowsInformationProtectionAppLockerFile object.</span></span>

<span data-ttu-id="97ef7-125">次の表に、windowsInformationProtectionAppLockerFile の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="97ef7-125">The following table shows the properties that are required when you create the windowsInformationProtectionAppLockerFile.</span></span>

|<span data-ttu-id="97ef7-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="97ef7-126">Property</span></span>|<span data-ttu-id="97ef7-127">型</span><span class="sxs-lookup"><span data-stu-id="97ef7-127">Type</span></span>|<span data-ttu-id="97ef7-128">説明</span><span class="sxs-lookup"><span data-stu-id="97ef7-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="97ef7-129">displayName</span><span class="sxs-lookup"><span data-stu-id="97ef7-129">displayName</span></span>|<span data-ttu-id="97ef7-130">String</span><span class="sxs-lookup"><span data-stu-id="97ef7-130">String</span></span>|<span data-ttu-id="97ef7-131">フレンドリ名</span><span class="sxs-lookup"><span data-stu-id="97ef7-131">The friendly name</span></span>|
|<span data-ttu-id="97ef7-132">fileHash</span><span class="sxs-lookup"><span data-stu-id="97ef7-132">fileHash</span></span>|<span data-ttu-id="97ef7-133">String</span><span class="sxs-lookup"><span data-stu-id="97ef7-133">String</span></span>|<span data-ttu-id="97ef7-134">ファイルの SHA256 ハッシュ</span><span class="sxs-lookup"><span data-stu-id="97ef7-134">SHA256 hash of the file</span></span>|
|<span data-ttu-id="97ef7-135">file</span><span class="sxs-lookup"><span data-stu-id="97ef7-135">file</span></span>|<span data-ttu-id="97ef7-136">Binary</span><span class="sxs-lookup"><span data-stu-id="97ef7-136">Binary</span></span>|<span data-ttu-id="97ef7-137">バイト配列のファイル</span><span class="sxs-lookup"><span data-stu-id="97ef7-137">File as a byte array</span></span>|
|<span data-ttu-id="97ef7-138">id</span><span class="sxs-lookup"><span data-stu-id="97ef7-138">id</span></span>|<span data-ttu-id="97ef7-139">String</span><span class="sxs-lookup"><span data-stu-id="97ef7-139">String</span></span>|<span data-ttu-id="97ef7-140">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="97ef7-140">Key of the entity.</span></span>|
|<span data-ttu-id="97ef7-141">version</span><span class="sxs-lookup"><span data-stu-id="97ef7-141">version</span></span>|<span data-ttu-id="97ef7-142">String</span><span class="sxs-lookup"><span data-stu-id="97ef7-142">String</span></span>|<span data-ttu-id="97ef7-143">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="97ef7-143">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="97ef7-144">応答</span><span class="sxs-lookup"><span data-stu-id="97ef7-144">Response</span></span>
<span data-ttu-id="97ef7-145">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="97ef7-145">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="97ef7-146">例</span><span class="sxs-lookup"><span data-stu-id="97ef7-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="97ef7-147">要求</span><span class="sxs-lookup"><span data-stu-id="97ef7-147">Request</span></span>
<span data-ttu-id="97ef7-148">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="97ef7-148">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles
Content-type: application/json
Content-length: 211

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLockerFile",
  "displayName": "Display Name value",
  "fileHash": "File Hash value",
  "file": "ZmlsZQ==",
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="97ef7-149">応答</span><span class="sxs-lookup"><span data-stu-id="97ef7-149">Response</span></span>
<span data-ttu-id="97ef7-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="97ef7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 260

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLockerFile",
  "displayName": "Display Name value",
  "fileHash": "File Hash value",
  "file": "ZmlsZQ==",
  "id": "d81f0e40-0e40-d81f-400e-1fd8400e1fd8",
  "version": "Version value"
}
```



