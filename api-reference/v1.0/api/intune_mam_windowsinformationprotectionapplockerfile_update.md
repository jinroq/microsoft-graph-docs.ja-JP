# <a name="update-windowsinformationprotectionapplockerfile"></a><span data-ttu-id="dc071-101">windowsInformationProtectionAppLockerFile の更新</span><span class="sxs-lookup"><span data-stu-id="dc071-101">Update windowsInformationProtectionAppLockerFile</span></span>

> <span data-ttu-id="dc071-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="dc071-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dc071-103">[windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="dc071-103">Update the properties of a [windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="dc071-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="dc071-104">Prerequisites</span></span>
<span data-ttu-id="dc071-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dc071-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="dc071-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="dc071-107">Permission type</span></span>|<span data-ttu-id="dc071-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="dc071-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dc071-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="dc071-109">Delegated (work or school account)</span></span>|<span data-ttu-id="dc071-110">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dc071-110">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="dc071-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="dc071-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dc071-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dc071-112">Not supported.</span></span>|
|<span data-ttu-id="dc071-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="dc071-113">Application</span></span>|<span data-ttu-id="dc071-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dc071-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dc071-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="dc071-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
PATCH /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/protectedAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
PATCH /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/exemptAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
PATCH /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/protectedAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
```

## <a name="request-headers"></a><span data-ttu-id="dc071-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="dc071-116">Request headers</span></span>
|<span data-ttu-id="dc071-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="dc071-117">Header</span></span>|<span data-ttu-id="dc071-118">値</span><span class="sxs-lookup"><span data-stu-id="dc071-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dc071-119">承認</span><span class="sxs-lookup"><span data-stu-id="dc071-119">Authorization</span></span>|<span data-ttu-id="dc071-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="dc071-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dc071-121">承諾</span><span class="sxs-lookup"><span data-stu-id="dc071-121">Accept</span></span>|<span data-ttu-id="dc071-122">アプリケーションまたは json</span><span class="sxs-lookup"><span data-stu-id="dc071-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dc071-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="dc071-123">Request body</span></span>
<span data-ttu-id="dc071-124">要求本文で、[windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="dc071-124">In the request body, supply a JSON representation for the [windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md) object.</span></span>

<span data-ttu-id="dc071-125">次の表に、[windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="dc071-125">The following table shows the properties that are required when you create the [windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md).</span></span>

|<span data-ttu-id="dc071-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="dc071-126">Property</span></span>|<span data-ttu-id="dc071-127">型</span><span class="sxs-lookup"><span data-stu-id="dc071-127">Type</span></span>|<span data-ttu-id="dc071-128">説明</span><span class="sxs-lookup"><span data-stu-id="dc071-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dc071-129">displayName</span><span class="sxs-lookup"><span data-stu-id="dc071-129">displayName</span></span>|<span data-ttu-id="dc071-130">文字列</span><span class="sxs-lookup"><span data-stu-id="dc071-130">String</span></span>|<span data-ttu-id="dc071-131">フレンドリ名</span><span class="sxs-lookup"><span data-stu-id="dc071-131">The friendly name</span></span>|
|<span data-ttu-id="dc071-132">fileHash</span><span class="sxs-lookup"><span data-stu-id="dc071-132">fileHash</span></span>|<span data-ttu-id="dc071-133">文字列</span><span class="sxs-lookup"><span data-stu-id="dc071-133">String</span></span>|<span data-ttu-id="dc071-134">ファイルの SHA256 ハッシュ</span><span class="sxs-lookup"><span data-stu-id="dc071-134">SHA256 hash of the file</span></span>|
|<span data-ttu-id="dc071-135">ファイル</span><span class="sxs-lookup"><span data-stu-id="dc071-135">file</span></span>|<span data-ttu-id="dc071-136">バイナリ型 (Binary)</span><span class="sxs-lookup"><span data-stu-id="dc071-136">Binary</span></span>|<span data-ttu-id="dc071-137">バイト配列のファイル</span><span class="sxs-lookup"><span data-stu-id="dc071-137">File as a byte array</span></span>|
|<span data-ttu-id="dc071-138">ID</span><span class="sxs-lookup"><span data-stu-id="dc071-138">id</span></span>|<span data-ttu-id="dc071-139">文字列</span><span class="sxs-lookup"><span data-stu-id="dc071-139">String</span></span>|<span data-ttu-id="dc071-140">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="dc071-140">Key of the entity.</span></span>|
|<span data-ttu-id="dc071-141">バージョン</span><span class="sxs-lookup"><span data-stu-id="dc071-141">version</span></span>|<span data-ttu-id="dc071-142">文字列</span><span class="sxs-lookup"><span data-stu-id="dc071-142">String</span></span>|<span data-ttu-id="dc071-143">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="dc071-143">Version of the entity.</span></span>|



## <a name="response"></a><span data-ttu-id="dc071-144">応答</span><span class="sxs-lookup"><span data-stu-id="dc071-144">Response</span></span>
<span data-ttu-id="dc071-145">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="dc071-145">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionAppLockerFile](../resources/intune_mam_windowsinformationprotectionapplockerfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dc071-146">例</span><span class="sxs-lookup"><span data-stu-id="dc071-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="dc071-147">要求</span><span class="sxs-lookup"><span data-stu-id="dc071-147">Request</span></span>
<span data-ttu-id="dc071-148">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="dc071-148">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
Content-type: application/json
Content-length: 131

{
  "displayName": "Display Name value",
  "fileHash": "File Hash value",
  "file": "ZmlsZQ==",
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="dc071-149">応答</span><span class="sxs-lookup"><span data-stu-id="dc071-149">Response</span></span>
<span data-ttu-id="dc071-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="dc071-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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








