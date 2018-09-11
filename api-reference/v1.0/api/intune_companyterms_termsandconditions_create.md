# <a name="create-termsandconditions"></a><span data-ttu-id="5a9cc-101">termsAndConditions の作成</span><span class="sxs-lookup"><span data-stu-id="5a9cc-101">Create termsAndConditions</span></span>

> <span data-ttu-id="5a9cc-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="5a9cc-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5a9cc-103">新しい [termsAndConditions](../resources/intune_companyterms_termsandconditions.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="5a9cc-103">Create a new [termsAndConditions](../resources/intune_companyterms_termsandconditions.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5a9cc-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="5a9cc-104">Prerequisites</span></span>
<span data-ttu-id="5a9cc-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5a9cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="5a9cc-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5a9cc-107">Permission type</span></span>|<span data-ttu-id="5a9cc-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="5a9cc-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5a9cc-109">委任 (職場または学校アカウント)</span><span class="sxs-lookup"><span data-stu-id="5a9cc-109">Delegated (work or school account)</span></span>|<span data-ttu-id="5a9cc-110">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5a9cc-110">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="5a9cc-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5a9cc-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5a9cc-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5a9cc-112">Not supported.</span></span>|
|<span data-ttu-id="5a9cc-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5a9cc-113">Application</span></span>|<span data-ttu-id="5a9cc-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5a9cc-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5a9cc-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5a9cc-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/termsAndConditions
```

## <a name="request-headers"></a><span data-ttu-id="5a9cc-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5a9cc-116">Request headers</span></span>
|<span data-ttu-id="5a9cc-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5a9cc-117">Header</span></span>|<span data-ttu-id="5a9cc-118">値</span><span class="sxs-lookup"><span data-stu-id="5a9cc-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5a9cc-119">承認</span><span class="sxs-lookup"><span data-stu-id="5a9cc-119">Authorization</span></span>|<span data-ttu-id="5a9cc-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="5a9cc-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5a9cc-121">承諾</span><span class="sxs-lookup"><span data-stu-id="5a9cc-121">Accept</span></span>|<span data-ttu-id="5a9cc-122">アプリケーションまたは json</span><span class="sxs-lookup"><span data-stu-id="5a9cc-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5a9cc-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="5a9cc-123">Request body</span></span>
<span data-ttu-id="5a9cc-124">要求本文において、termsAndConditions オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="5a9cc-124">In the request body, supply a JSON representation for the termsAndConditions object.</span></span>

<span data-ttu-id="5a9cc-125">次の表に、termsAndConditions の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="5a9cc-125">The following table shows the properties that are required when you create the termsAndConditions.</span></span>

|<span data-ttu-id="5a9cc-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5a9cc-126">Property</span></span>|<span data-ttu-id="5a9cc-127">型</span><span class="sxs-lookup"><span data-stu-id="5a9cc-127">Type</span></span>|<span data-ttu-id="5a9cc-128">説明</span><span class="sxs-lookup"><span data-stu-id="5a9cc-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5a9cc-129">ID</span><span class="sxs-lookup"><span data-stu-id="5a9cc-129">id</span></span>|<span data-ttu-id="5a9cc-130">文字列</span><span class="sxs-lookup"><span data-stu-id="5a9cc-130">String</span></span>|<span data-ttu-id="5a9cc-131">T&C ポリシーの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="5a9cc-131">Unique identifier of the T&C policy.</span></span>|
|<span data-ttu-id="5a9cc-132">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="5a9cc-132">createdDateTime</span></span>|<span data-ttu-id="5a9cc-133">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5a9cc-133">DateTimeOffset</span></span>|<span data-ttu-id="5a9cc-134">オブジェクトが作成された DateTime。</span><span class="sxs-lookup"><span data-stu-id="5a9cc-134">DateTime the object was created.</span></span>|
|<span data-ttu-id="5a9cc-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="5a9cc-135">lastModifiedDateTime</span></span>|<span data-ttu-id="5a9cc-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5a9cc-136">DateTimeOffset</span></span>|<span data-ttu-id="5a9cc-137">オブジェクトが最後に変更された DateTime。</span><span class="sxs-lookup"><span data-stu-id="5a9cc-137">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="5a9cc-138">displayName</span><span class="sxs-lookup"><span data-stu-id="5a9cc-138">displayName</span></span>|<span data-ttu-id="5a9cc-139">文字列</span><span class="sxs-lookup"><span data-stu-id="5a9cc-139">String</span></span>|<span data-ttu-id="5a9cc-140">T&C ポリシー用に管理者が提供した名前。</span><span class="sxs-lookup"><span data-stu-id="5a9cc-140">Administrator-supplied name for the T&C policy.</span></span> |
|<span data-ttu-id="5a9cc-141">説明</span><span class="sxs-lookup"><span data-stu-id="5a9cc-141">description</span></span>|<span data-ttu-id="5a9cc-142">文字列</span><span class="sxs-lookup"><span data-stu-id="5a9cc-142">String</span></span>|<span data-ttu-id="5a9cc-143">管理者が提供した T&C ポリシーの説明。</span><span class="sxs-lookup"><span data-stu-id="5a9cc-143">Administrator-supplied description of the T&C policy.</span></span>|
|<span data-ttu-id="5a9cc-144">タイトル</span><span class="sxs-lookup"><span data-stu-id="5a9cc-144">title</span></span>|<span data-ttu-id="5a9cc-145">文字列</span><span class="sxs-lookup"><span data-stu-id="5a9cc-145">String</span></span>|<span data-ttu-id="5a9cc-146">管理者が提供した契約条件のタイトル。</span><span class="sxs-lookup"><span data-stu-id="5a9cc-146">Administrator-supplied title of the terms and conditions.</span></span> <span data-ttu-id="5a9cc-147">ユーザーが T&C ポリシーを承諾する際のプロンプトに表示されます。</span><span class="sxs-lookup"><span data-stu-id="5a9cc-147">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="5a9cc-148">bodyText</span><span class="sxs-lookup"><span data-stu-id="5a9cc-148">bodyText</span></span>|<span data-ttu-id="5a9cc-149">文字列</span><span class="sxs-lookup"><span data-stu-id="5a9cc-149">String</span></span>|<span data-ttu-id="5a9cc-150">管理者が提供する契約条件の本文で、通常は条件そのものです。</span><span class="sxs-lookup"><span data-stu-id="5a9cc-150">Administrator-supplied body text of the terms and conditions, typically the terms themselves.</span></span> <span data-ttu-id="5a9cc-151">ユーザーが T&C ポリシーを承諾する際のプロンプトに表示されます。</span><span class="sxs-lookup"><span data-stu-id="5a9cc-151">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="5a9cc-152">acceptanceStatement</span><span class="sxs-lookup"><span data-stu-id="5a9cc-152">acceptanceStatement</span></span>|<span data-ttu-id="5a9cc-153">文字列</span><span class="sxs-lookup"><span data-stu-id="5a9cc-153">String</span></span>|<span data-ttu-id="5a9cc-154">使用条件に関する、管理者指定の説明内容です。通常は、T&C ポリシーに定められた使用条件を受け入れることの意味を記載します。</span><span class="sxs-lookup"><span data-stu-id="5a9cc-154">Administrator-supplied explanation of the terms and conditions, typically describing what it means to accept the terms and conditions set out in the T&C policy.</span></span> <span data-ttu-id="5a9cc-155">ユーザーが T&C ポリシーを承諾する際のプロンプトに表示されます。</span><span class="sxs-lookup"><span data-stu-id="5a9cc-155">This is shown to the user on prompts to accept the T&C policy.</span></span>|
|<span data-ttu-id="5a9cc-156">バージョン</span><span class="sxs-lookup"><span data-stu-id="5a9cc-156">version</span></span>|<span data-ttu-id="5a9cc-157">Int32</span><span class="sxs-lookup"><span data-stu-id="5a9cc-157">Int32</span></span>|<span data-ttu-id="5a9cc-158">条件の現行バージョンを示す整数。</span><span class="sxs-lookup"><span data-stu-id="5a9cc-158">Integer indicating the current version of the terms.</span></span> <span data-ttu-id="5a9cc-159">管理者が条件を変更し、修正された T&C ポリシーをユーザーが再承諾するように求める場合に増分されます。</span><span class="sxs-lookup"><span data-stu-id="5a9cc-159">Incremented when an administrator makes a change to the terms and wishes to require users to re-accept the modified T&C policy.</span></span>|



## <a name="response"></a><span data-ttu-id="5a9cc-160">応答</span><span class="sxs-lookup"><span data-stu-id="5a9cc-160">Response</span></span>
<span data-ttu-id="5a9cc-161">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [termsAndConditions](../resources/intune_companyterms_termsandconditions.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="5a9cc-161">If successful, this method returns a `201 Created` response code and a [termsAndConditions](../resources/intune_companyterms_termsandconditions.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5a9cc-162">例</span><span class="sxs-lookup"><span data-stu-id="5a9cc-162">Example</span></span>
### <a name="request"></a><span data-ttu-id="5a9cc-163">要求</span><span class="sxs-lookup"><span data-stu-id="5a9cc-163">Request</span></span>
<span data-ttu-id="5a9cc-164">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5a9cc-164">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5a9cc-165">応答</span><span class="sxs-lookup"><span data-stu-id="5a9cc-165">Response</span></span>
<span data-ttu-id="5a9cc-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="5a9cc-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








