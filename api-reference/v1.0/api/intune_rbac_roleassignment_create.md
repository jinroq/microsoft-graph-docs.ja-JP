# <a name="create-roleassignment"></a><span data-ttu-id="263fa-101">roleAssignment の作成</span><span class="sxs-lookup"><span data-stu-id="263fa-101">Create roleAssignment</span></span>

> <span data-ttu-id="263fa-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="263fa-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="263fa-103">新しい [roleAssignment](../resources/intune_rbac_roleassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="263fa-103">Create a new [plannerBucket](../resources/intune_rbac_roleassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="263fa-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="263fa-104">Prerequisites</span></span>
<span data-ttu-id="263fa-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="263fa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="263fa-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="263fa-107">Permission type</span></span>|<span data-ttu-id="263fa-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="263fa-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="263fa-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="263fa-109">Delegated (work or school account)</span></span>|<span data-ttu-id="263fa-110">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="263fa-110">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="263fa-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="263fa-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="263fa-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="263fa-112">Not supported.</span></span>|
|<span data-ttu-id="263fa-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="263fa-113">Application</span></span>|<span data-ttu-id="263fa-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="263fa-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="263fa-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="263fa-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="263fa-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="263fa-116">Request headers</span></span>
|<span data-ttu-id="263fa-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="263fa-117">Header</span></span>|<span data-ttu-id="263fa-118">値</span><span class="sxs-lookup"><span data-stu-id="263fa-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="263fa-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="263fa-119">Authorization</span></span>|<span data-ttu-id="263fa-120">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="263fa-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="263fa-121">Accept</span><span class="sxs-lookup"><span data-stu-id="263fa-121">Accept</span></span>|<span data-ttu-id="263fa-122">application/json</span><span class="sxs-lookup"><span data-stu-id="263fa-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="263fa-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="263fa-123">Request body</span></span>
<span data-ttu-id="263fa-124">要求本文で、roleAssignment オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="263fa-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="263fa-125">次の表に、roleAssignment の作成時に必要になるプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="263fa-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="263fa-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="263fa-126">Property</span></span>|<span data-ttu-id="263fa-127">型</span><span class="sxs-lookup"><span data-stu-id="263fa-127">Type</span></span>|<span data-ttu-id="263fa-128">説明</span><span class="sxs-lookup"><span data-stu-id="263fa-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="263fa-129">id</span><span class="sxs-lookup"><span data-stu-id="263fa-129">id</span></span>|<span data-ttu-id="263fa-130">String</span><span class="sxs-lookup"><span data-stu-id="263fa-130">String</span></span>|<span data-ttu-id="263fa-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="263fa-131">Name of the entity.</span></span> <span data-ttu-id="263fa-132">これは読み取り専用で、自動生成されます。</span><span class="sxs-lookup"><span data-stu-id="263fa-132">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="263fa-133">displayName</span><span class="sxs-lookup"><span data-stu-id="263fa-133">displayName</span></span>|<span data-ttu-id="263fa-134">String</span><span class="sxs-lookup"><span data-stu-id="263fa-134">String</span></span>|<span data-ttu-id="263fa-135">ロール割り当ての表示名またはフレンドリ名。</span><span class="sxs-lookup"><span data-stu-id="263fa-135">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="263fa-136">description</span><span class="sxs-lookup"><span data-stu-id="263fa-136">description</span></span>|<span data-ttu-id="263fa-137">String</span><span class="sxs-lookup"><span data-stu-id="263fa-137">String</span></span>|<span data-ttu-id="263fa-138">ロール割り当ての説明。</span><span class="sxs-lookup"><span data-stu-id="263fa-138">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="263fa-139">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="263fa-139">resourceScopes</span></span>|<span data-ttu-id="263fa-140">String コレクション</span><span class="sxs-lookup"><span data-stu-id="263fa-140">String collection</span></span>|<span data-ttu-id="263fa-141">役割のスコープ メンバーのセキュリティ グループの ID リスト。</span><span class="sxs-lookup"><span data-stu-id="263fa-141">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="263fa-142">Azure Active Directory の ID。</span><span class="sxs-lookup"><span data-stu-id="263fa-142">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="263fa-143">応答</span><span class="sxs-lookup"><span data-stu-id="263fa-143">Response</span></span>
<span data-ttu-id="263fa-144">成功した場合、このメソッドは `201 Created` 応答コードと応答本文で [roleAssignment](../resources/intune_rbac_roleassignment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="263fa-144">If successful, this method returns a `201 Created` response code and a [section](../resources/intune_rbac_roleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="263fa-145">例</span><span class="sxs-lookup"><span data-stu-id="263fa-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="263fa-146">要求</span><span class="sxs-lookup"><span data-stu-id="263fa-146">Request</span></span>
<span data-ttu-id="263fa-147">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="263fa-147">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments
Content-type: application/json
Content-length: 193

{
  "@odata.type": "#microsoft.graph.roleAssignment",
  "displayName": "Display Name value",
  "description": "Description value",
  "resourceScopes": [
    "Resource Scopes value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="263fa-148">応答</span><span class="sxs-lookup"><span data-stu-id="263fa-148">Response</span></span>
<span data-ttu-id="263fa-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="263fa-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 242

{
  "@odata.type": "#microsoft.graph.roleAssignment",
  "id": "b3234d24-4d24-b323-244d-23b3244d23b3",
  "displayName": "Display Name value",
  "description": "Description value",
  "resourceScopes": [
    "Resource Scopes value"
  ]
}
```



