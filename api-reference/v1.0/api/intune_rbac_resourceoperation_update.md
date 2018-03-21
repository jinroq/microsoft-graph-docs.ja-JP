# <a name="update-resourceoperation"></a><span data-ttu-id="e63c4-101">resourceOperation の更新</span><span class="sxs-lookup"><span data-stu-id="e63c4-101">Update resourceOperation</span></span>

> <span data-ttu-id="e63c4-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e63c4-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e63c4-103">[resourceOperation](../resources/intune_rbac_resourceoperation.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="e63c4-103">Update the properties of a [calendar](../resources/intune_rbac_resourceoperation.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e63c4-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="e63c4-104">Prerequisites</span></span>
<span data-ttu-id="e63c4-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e63c4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e63c4-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e63c4-107">Permission type</span></span>|<span data-ttu-id="e63c4-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="e63c4-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e63c4-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e63c4-109">Delegated (work or school account)</span></span>|<span data-ttu-id="e63c4-110">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e63c4-110">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="e63c4-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e63c4-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e63c4-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e63c4-112">Not supported.</span></span>|
|<span data-ttu-id="e63c4-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e63c4-113">Application</span></span>|<span data-ttu-id="e63c4-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e63c4-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e63c4-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e63c4-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/resourceOperations/{resourceOperationId}
```

## <a name="request-headers"></a><span data-ttu-id="e63c4-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e63c4-116">Request headers</span></span>
|<span data-ttu-id="e63c4-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e63c4-117">Header</span></span>|<span data-ttu-id="e63c4-118">値</span><span class="sxs-lookup"><span data-stu-id="e63c4-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e63c4-119">承認</span><span class="sxs-lookup"><span data-stu-id="e63c4-119">Authorization</span></span>|<span data-ttu-id="e63c4-120">ベアラー &lt;トークン&gt;が必須。</span><span class="sxs-lookup"><span data-stu-id="e63c4-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="e63c4-121">承諾</span><span class="sxs-lookup"><span data-stu-id="e63c4-121">Accept</span></span>|<span data-ttu-id="e63c4-122">application/json</span><span class="sxs-lookup"><span data-stu-id="e63c4-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e63c4-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="e63c4-123">Request body</span></span>
<span data-ttu-id="e63c4-124">要求本文で、[resourceOperation](../resources/intune_rbac_resourceoperation.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="e63c4-124">In the request body, supply a JSON representation of [Message](../resources/intune_rbac_resourceoperation.md) object.</span></span>

<span data-ttu-id="e63c4-125">次の表に、[resourceOperation](../resources/intune_rbac_resourceoperation.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="e63c4-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="e63c4-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e63c4-126">Property</span></span>|<span data-ttu-id="e63c4-127">型</span><span class="sxs-lookup"><span data-stu-id="e63c4-127">Type</span></span>|<span data-ttu-id="e63c4-128">説明</span><span class="sxs-lookup"><span data-stu-id="e63c4-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e63c4-129">id</span><span class="sxs-lookup"><span data-stu-id="e63c4-129">id</span></span>|<span data-ttu-id="e63c4-130">String</span><span class="sxs-lookup"><span data-stu-id="e63c4-130">String</span></span>|<span data-ttu-id="e63c4-131">リソース操作のキー。</span><span class="sxs-lookup"><span data-stu-id="e63c4-131">Key of the Resource Operation.</span></span> <span data-ttu-id="e63c4-132">読み取り専用で、自動生成されます。</span><span class="sxs-lookup"><span data-stu-id="e63c4-132">Read-only, automatically generated.</span></span>|
|<span data-ttu-id="e63c4-133">resourceName</span><span class="sxs-lookup"><span data-stu-id="e63c4-133">resourceName</span></span>|<span data-ttu-id="e63c4-134">String</span><span class="sxs-lookup"><span data-stu-id="e63c4-134">String</span></span>|<span data-ttu-id="e63c4-135">この操作が実行されるリソースの名前。</span><span class="sxs-lookup"><span data-stu-id="e63c4-135">Name of the Resource this operation is performed on.</span></span>|
|<span data-ttu-id="e63c4-136">actionName</span><span class="sxs-lookup"><span data-stu-id="e63c4-136">ActionName</span></span>|<span data-ttu-id="e63c4-137">String</span><span class="sxs-lookup"><span data-stu-id="e63c4-137">String</span></span>|<span data-ttu-id="e63c4-138">この操作が実行するアクションの種類。</span><span class="sxs-lookup"><span data-stu-id="e63c4-138">Type of action this operation is going to perform.</span></span> <span data-ttu-id="e63c4-139">actionName は簡潔で、できるだけ少ない単語にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="e63c4-139">The actionName should be concise and limited to as few words as possible.</span></span>|
|<span data-ttu-id="e63c4-140">description</span><span class="sxs-lookup"><span data-stu-id="e63c4-140">description</span></span>|<span data-ttu-id="e63c4-141">String</span><span class="sxs-lookup"><span data-stu-id="e63c4-141">String</span></span>|<span data-ttu-id="e63c4-142">リソース操作の説明。</span><span class="sxs-lookup"><span data-stu-id="e63c4-142">Description of the resource operation.</span></span> <span data-ttu-id="e63c4-143">Azure Portal で操作にマウス ポインターを合わせると、その操作の説明がテキストで表示されます。</span><span class="sxs-lookup"><span data-stu-id="e63c4-143">The description is used in mouse-over text for the operation when shown in the Azure Portal.</span></span>|



## <a name="response"></a><span data-ttu-id="e63c4-144">応答</span><span class="sxs-lookup"><span data-stu-id="e63c4-144">Response</span></span>
<span data-ttu-id="e63c4-145">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [resourceOperation](../resources/intune_rbac_resourceoperation.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="e63c4-145">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_rbac_resourceoperation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e63c4-146">例</span><span class="sxs-lookup"><span data-stu-id="e63c4-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="e63c4-147">要求</span><span class="sxs-lookup"><span data-stu-id="e63c4-147">Request</span></span>
<span data-ttu-id="e63c4-148">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e63c4-148">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/resourceOperations/{resourceOperationId}
Content-type: application/json
Content-length: 122

{
  "resourceName": "Resource Name value",
  "actionName": "Action Name value",
  "description": "Description value"
}
```

### <a name="response"></a><span data-ttu-id="e63c4-149">応答</span><span class="sxs-lookup"><span data-stu-id="e63c4-149">Response</span></span>
<span data-ttu-id="e63c4-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e63c4-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



