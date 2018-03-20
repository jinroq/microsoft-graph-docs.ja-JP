# <a name="create-termsandconditions"></a><span data-ttu-id="87a4c-101">termsAndConditions の作成</span><span class="sxs-lookup"><span data-stu-id="87a4c-101">Create termsAndConditions</span></span>

> <span data-ttu-id="87a4c-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="87a4c-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="87a4c-103">新しい [termsAndConditions](../resources/intune_companyterms_termsandconditions.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="87a4c-103">Create a new [plannerBucket](../resources/intune_companyterms_termsandconditions.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="87a4c-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="87a4c-104">Prerequisites</span></span>
<span data-ttu-id="87a4c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="87a4c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="87a4c-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="87a4c-107">Permission type</span></span>|<span data-ttu-id="87a4c-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="87a4c-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="87a4c-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="87a4c-109">Delegated (work or school account)</span></span>|<span data-ttu-id="87a4c-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="87a4c-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="87a4c-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="87a4c-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="87a4c-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="87a4c-112">Not supported.</span></span>|
|<span data-ttu-id="87a4c-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="87a4c-113">Application</span></span>|<span data-ttu-id="87a4c-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="87a4c-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="87a4c-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="87a4c-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/termsAndConditions
```

## <a name="request-headers"></a><span data-ttu-id="87a4c-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="87a4c-116">Request headers</span></span>
|<span data-ttu-id="87a4c-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="87a4c-117">Header</span></span>|<span data-ttu-id="87a4c-118">値</span><span class="sxs-lookup"><span data-stu-id="87a4c-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="87a4c-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="87a4c-119">Authorization</span></span>|<span data-ttu-id="87a4c-120">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="87a4c-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="87a4c-121">Accept</span><span class="sxs-lookup"><span data-stu-id="87a4c-121">Accept</span></span>|<span data-ttu-id="87a4c-122">application/json</span><span class="sxs-lookup"><span data-stu-id="87a4c-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="87a4c-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="87a4c-123">Request body</span></span>
<span data-ttu-id="87a4c-124">要求本文において、termsAndConditions オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="87a4c-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="87a4c-125">次の表に、termsAndConditions の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="87a4c-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="87a4c-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="87a4c-126">Property</span></span>|<span data-ttu-id="87a4c-127">型</span><span class="sxs-lookup"><span data-stu-id="87a4c-127">Type</span></span>|<span data-ttu-id="87a4c-128">説明</span><span class="sxs-lookup"><span data-stu-id="87a4c-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="87a4c-129">id</span><span class="sxs-lookup"><span data-stu-id="87a4c-129">id</span></span>|<span data-ttu-id="87a4c-130">String</span><span class="sxs-lookup"><span data-stu-id="87a4c-130">String</span></span>|<span data-ttu-id="87a4c-131">T&C ポリシーの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="87a4c-131">Unique identifier of the T&C policy.</span></span>|
|<span data-ttu-id="87a4c-132">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="87a4c-132">createdDateTime</span></span>|<span data-ttu-id="87a4c-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="87a4c-133">DateTimeOffset</span></span>|<span data-ttu-id="87a4c-134">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="87a4c-134">DateTime the object was created.</span></span>|
|<span data-ttu-id="87a4c-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="87a4c-135">lastModifiedDateTime</span></span>|<span data-ttu-id="87a4c-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="87a4c-136">DateTimeOffset</span></span>|<span data-ttu-id="87a4c-137">オブジェクトの最終更新の DateTime。</span><span class="sxs-lookup"><span data-stu-id="87a4c-137">Gets or sets a DateTime value specifying when the node object was last modified.</span></span>|
|<span data-ttu-id="87a4c-138">displayName</span><span class="sxs-lookup"><span data-stu-id="87a4c-138">displayName</span></span>|<span data-ttu-id="87a4c-139">String</span><span class="sxs-lookup"><span data-stu-id="87a4c-139">String</span></span>|<span data-ttu-id="87a4c-140">管理者が指定した T&C ポリシーの名前。</span><span class="sxs-lookup"><span data-stu-id="87a4c-140">Administrator-supplied name for the T&C policy.</span></span> |
|<span data-ttu-id="87a4c-141">description</span><span class="sxs-lookup"><span data-stu-id="87a4c-141">description</span></span>|<span data-ttu-id="87a4c-142">String</span><span class="sxs-lookup"><span data-stu-id="87a4c-142">String</span></span>|<span data-ttu-id="87a4c-143">管理者が指定した T&C ポリシーの説明。</span><span class="sxs-lookup"><span data-stu-id="87a4c-143">Administrator-supplied description of the T&C policy.</span></span>|
|<span data-ttu-id="87a4c-144">title</span><span class="sxs-lookup"><span data-stu-id="87a4c-144">title</span></span>|<span data-ttu-id="87a4c-145">String</span><span class="sxs-lookup"><span data-stu-id="87a4c-145">String</span></span>|<span data-ttu-id="87a4c-146">管理者が指定した使用条件のタイトル。</span><span class="sxs-lookup"><span data-stu-id="87a4c-146">Administrator-supplied title of the terms and conditions.</span></span> <span data-ttu-id="87a4c-147">ユーザーが T&C ポリシーを承諾する際のプロンプトに表示されます。</span><span class="sxs-lookup"><span data-stu-id="87a4c-147">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="87a4c-148">bodyText</span><span class="sxs-lookup"><span data-stu-id="87a4c-148">BodyText</span></span>|<span data-ttu-id="87a4c-149">String</span><span class="sxs-lookup"><span data-stu-id="87a4c-149">String</span></span>|<span data-ttu-id="87a4c-150">管理者が指定した使用条件の本文で、通常は使用条件そのものです。</span><span class="sxs-lookup"><span data-stu-id="87a4c-150">Administrator-supplied body text of the terms and conditions, typically the terms themselves.</span></span> <span data-ttu-id="87a4c-151">ユーザーが T&C ポリシーを承諾する際のプロンプトに表示されます。</span><span class="sxs-lookup"><span data-stu-id="87a4c-151">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="87a4c-152">acceptanceStatement</span><span class="sxs-lookup"><span data-stu-id="87a4c-152">acceptanceStatement</span></span>|<span data-ttu-id="87a4c-153">String</span><span class="sxs-lookup"><span data-stu-id="87a4c-153">String</span></span>|<span data-ttu-id="87a4c-154">管理者が指定した使用条件に関する説明内容です。通常は、T&C ポリシーに定められた使用条件を受け入れることの意味が記載されます。</span><span class="sxs-lookup"><span data-stu-id="87a4c-154">Administrator-supplied explanation of the terms and conditions, typically describing what it means to accept the terms and conditions set out in the T&C policy.</span></span> <span data-ttu-id="87a4c-155">ユーザーが T&C ポリシーを承諾する際のプロンプトに表示されます。</span><span class="sxs-lookup"><span data-stu-id="87a4c-155">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="87a4c-156">version</span><span class="sxs-lookup"><span data-stu-id="87a4c-156">version</span></span>|<span data-ttu-id="87a4c-157">Int32</span><span class="sxs-lookup"><span data-stu-id="87a4c-157">Int32</span></span>|<span data-ttu-id="87a4c-158">使用条件の現在のバージョンを示す整数。</span><span class="sxs-lookup"><span data-stu-id="87a4c-158">Integer indicating the current version of the terms.</span></span> <span data-ttu-id="87a4c-159">管理者が条件を変更し、修正された T&C ポリシーをユーザーが再承諾するように求める場合に増分されます。</span><span class="sxs-lookup"><span data-stu-id="87a4c-159">Incremented when an administrator makes a change to the terms and wishes to require users to re-accept the modified T&C policy.</span></span>|



## <a name="response"></a><span data-ttu-id="87a4c-160">応答</span><span class="sxs-lookup"><span data-stu-id="87a4c-160">Response</span></span>
<span data-ttu-id="87a4c-161">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [termsAndConditions](../resources/intune_companyterms_termsandconditions.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="87a4c-161">If successful, this method returns a `201 Created` response code and a [section](../resources/intune_companyterms_termsandconditions.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="87a4c-162">例</span><span class="sxs-lookup"><span data-stu-id="87a4c-162">Example</span></span>
### <a name="request"></a><span data-ttu-id="87a4c-163">要求</span><span class="sxs-lookup"><span data-stu-id="87a4c-163">Request</span></span>
<span data-ttu-id="87a4c-164">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="87a4c-164">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions
Content-type: application/json
Content-length: 337

{
  "@odata.type": "#microsoft.graph.termsAndConditions",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "description": "Description value",
  "title": "Title value",
  "bodyText": "Body Text value",
  "acceptanceStatement": "Acceptance Statement value",
  "version": 7
}
```

### <a name="response"></a><span data-ttu-id="87a4c-165">応答</span><span class="sxs-lookup"><span data-stu-id="87a4c-165">Response</span></span>
<span data-ttu-id="87a4c-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="87a4c-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 445

{
  "@odata.type": "#microsoft.graph.termsAndConditions",
  "id": "eefc80cf-80cf-eefc-cf80-fceecf80fcee",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "displayName": "Display Name value",
  "description": "Description value",
  "title": "Title value",
  "bodyText": "Body Text value",
  "acceptanceStatement": "Acceptance Statement value",
  "version": 7
}
```



