# <a name="create-resourceoperation"></a><span data-ttu-id="2b292-101">resourceOperation の作成</span><span class="sxs-lookup"><span data-stu-id="2b292-101">Create resourceOperation</span></span>

> <span data-ttu-id="2b292-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="2b292-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2b292-103">新しい [resourceOperation](../resources/intune_rbac_resourceoperation.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="2b292-103">Create a new [resourceOperation](../resources/intune_rbac_resourceoperation.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2b292-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="2b292-104">Prerequisites</span></span>
<span data-ttu-id="2b292-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2b292-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="2b292-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2b292-107">Permission type</span></span>|<span data-ttu-id="2b292-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="2b292-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2b292-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2b292-109">Delegated (work or school account)</span></span>|<span data-ttu-id="2b292-110">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2b292-110">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="2b292-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2b292-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2b292-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2b292-112">Not supported.</span></span>|
|<span data-ttu-id="2b292-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2b292-113">Application</span></span>|<span data-ttu-id="2b292-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2b292-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2b292-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2b292-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/resourceOperations
```

## <a name="request-headers"></a><span data-ttu-id="2b292-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2b292-116">Request headers</span></span>
|<span data-ttu-id="2b292-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2b292-117">Header</span></span>|<span data-ttu-id="2b292-118">値</span><span class="sxs-lookup"><span data-stu-id="2b292-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2b292-119">承認</span><span class="sxs-lookup"><span data-stu-id="2b292-119">Authorization</span></span>|<span data-ttu-id="2b292-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="2b292-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2b292-121">承諾</span><span class="sxs-lookup"><span data-stu-id="2b292-121">Accept</span></span>|<span data-ttu-id="2b292-122">アプリケーションまたは json</span><span class="sxs-lookup"><span data-stu-id="2b292-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2b292-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="2b292-123">Request body</span></span>
<span data-ttu-id="2b292-124">要求本文で、resourceOperation オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="2b292-124">In the request body, supply a JSON representation for the resourceOperation object.</span></span>

<span data-ttu-id="2b292-125">次の表に、resourceOperation の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="2b292-125">The following table shows the properties that are required when you create the resourceOperation.</span></span>

|<span data-ttu-id="2b292-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2b292-126">Property</span></span>|<span data-ttu-id="2b292-127">型</span><span class="sxs-lookup"><span data-stu-id="2b292-127">Type</span></span>|<span data-ttu-id="2b292-128">説明</span><span class="sxs-lookup"><span data-stu-id="2b292-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2b292-129">ID</span><span class="sxs-lookup"><span data-stu-id="2b292-129">id</span></span>|<span data-ttu-id="2b292-130">文字列</span><span class="sxs-lookup"><span data-stu-id="2b292-130">String</span></span>|<span data-ttu-id="2b292-131">リソース操作のキー。</span><span class="sxs-lookup"><span data-stu-id="2b292-131">Key of the Resource Operation.</span></span> <span data-ttu-id="2b292-132">読み取り専用で、自動生成されます。</span><span class="sxs-lookup"><span data-stu-id="2b292-132">Read-only, automatically generated.</span></span>|
|<span data-ttu-id="2b292-133">resourceName</span><span class="sxs-lookup"><span data-stu-id="2b292-133">resourceName</span></span>|<span data-ttu-id="2b292-134">文字列</span><span class="sxs-lookup"><span data-stu-id="2b292-134">String</span></span>|<span data-ttu-id="2b292-135">この操作が実行されるリソースの名前。</span><span class="sxs-lookup"><span data-stu-id="2b292-135">Name of the Resource this operation is performed on.</span></span>|
|<span data-ttu-id="2b292-136">actionName</span><span class="sxs-lookup"><span data-stu-id="2b292-136">actionName</span></span>|<span data-ttu-id="2b292-137">文字列</span><span class="sxs-lookup"><span data-stu-id="2b292-137">String</span></span>|<span data-ttu-id="2b292-138">この操作が実行するアクションの種類。</span><span class="sxs-lookup"><span data-stu-id="2b292-138">Type of action this operation is going to perform.</span></span> <span data-ttu-id="2b292-139">actionName は簡潔で、できるだけ少ない単語にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="2b292-139">The actionName should be concise and limited to as few words as possible.</span></span>|
|<span data-ttu-id="2b292-140">説明</span><span class="sxs-lookup"><span data-stu-id="2b292-140">description</span></span>|<span data-ttu-id="2b292-141">文字列</span><span class="sxs-lookup"><span data-stu-id="2b292-141">String</span></span>|<span data-ttu-id="2b292-142">リソース操作の説明。</span><span class="sxs-lookup"><span data-stu-id="2b292-142">Description of the resource operation.</span></span> <span data-ttu-id="2b292-143">Azure Portal で操作にマウス ポインターを合わせると、その操作の説明がテキストで表示されます。</span><span class="sxs-lookup"><span data-stu-id="2b292-143">The description is used in mouse-over text for the operation when shown in the Azure Portal.</span></span>|



## <a name="response"></a><span data-ttu-id="2b292-144">応答</span><span class="sxs-lookup"><span data-stu-id="2b292-144">Response</span></span>
<span data-ttu-id="2b292-145">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [resourceOperation](../resources/intune_rbac_resourceoperation.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="2b292-145">If successful, this method returns a `201 Created` response code and a [resourceOperation](../resources/intune_rbac_resourceoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2b292-146">例</span><span class="sxs-lookup"><span data-stu-id="2b292-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="2b292-147">要求</span><span class="sxs-lookup"><span data-stu-id="2b292-147">Request</span></span>
<span data-ttu-id="2b292-148">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2b292-148">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/resourceOperations
Content-type: application/json
Content-length: 178

{
  "@odata.type": "#microsoft.graph.resourceOperation",
  "resourceName": "Resource Name value",
  "actionName": "Action Name value",
  "description": "Description value"
}
```

### <a name="response"></a><span data-ttu-id="2b292-149">応答</span><span class="sxs-lookup"><span data-stu-id="2b292-149">Response</span></span>
<span data-ttu-id="2b292-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2b292-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 227

{
  "@odata.type": "#microsoft.graph.resourceOperation",
  "id": "232b8fee-8fee-232b-ee8f-2b23ee8f2b23",
  "resourceName": "Resource Name value",
  "actionName": "Action Name value",
  "description": "Description value"
}
```








