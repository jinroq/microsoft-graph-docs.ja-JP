# <a name="update-roleassignment"></a><span data-ttu-id="35262-101">roleAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="35262-101">Update roleAssignment</span></span>

> <span data-ttu-id="35262-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="35262-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="35262-103">[roleAssignment](../resources/intune_rbac_roleassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="35262-103">Update the properties of a [calendar](../resources/intune_rbac_roleassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="35262-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="35262-104">Prerequisites</span></span>
<span data-ttu-id="35262-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="35262-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="35262-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="35262-107">Permission type</span></span>|<span data-ttu-id="35262-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="35262-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="35262-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="35262-109">Delegated (work or school account)</span></span>|<span data-ttu-id="35262-110">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="35262-110">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="35262-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="35262-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="35262-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="35262-112">Not supported.</span></span>|
|<span data-ttu-id="35262-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="35262-113">Application</span></span>|<span data-ttu-id="35262-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="35262-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="35262-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="35262-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="35262-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="35262-116">Request headers</span></span>
|<span data-ttu-id="35262-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="35262-117">Header</span></span>|<span data-ttu-id="35262-118">値</span><span class="sxs-lookup"><span data-stu-id="35262-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="35262-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="35262-119">Authorization</span></span>|<span data-ttu-id="35262-120">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="35262-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="35262-121">Accept</span><span class="sxs-lookup"><span data-stu-id="35262-121">Accept</span></span>|<span data-ttu-id="35262-122">application/json</span><span class="sxs-lookup"><span data-stu-id="35262-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="35262-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="35262-123">Request body</span></span>
<span data-ttu-id="35262-124">要求本文で、[roleAssignment](../resources/intune_rbac_roleassignment.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="35262-124">In the request body, supply a JSON representation of the [Contact](../resources/intune_rbac_roleassignment.md) object.</span></span>

<span data-ttu-id="35262-125">次の表に、[roleAssignment](../resources/intune_rbac_roleassignment.md) の作成時に必要になるプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="35262-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="35262-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="35262-126">Property</span></span>|<span data-ttu-id="35262-127">型</span><span class="sxs-lookup"><span data-stu-id="35262-127">Type</span></span>|<span data-ttu-id="35262-128">説明</span><span class="sxs-lookup"><span data-stu-id="35262-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="35262-129">id</span><span class="sxs-lookup"><span data-stu-id="35262-129">id</span></span>|<span data-ttu-id="35262-130">String</span><span class="sxs-lookup"><span data-stu-id="35262-130">String</span></span>|<span data-ttu-id="35262-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="35262-131">Name of the entity.</span></span> <span data-ttu-id="35262-132">これは読み取り専用で、自動生成されます。</span><span class="sxs-lookup"><span data-stu-id="35262-132">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="35262-133">displayName</span><span class="sxs-lookup"><span data-stu-id="35262-133">displayName</span></span>|<span data-ttu-id="35262-134">String</span><span class="sxs-lookup"><span data-stu-id="35262-134">String</span></span>|<span data-ttu-id="35262-135">ロール割り当ての表示名またはフレンドリ名。</span><span class="sxs-lookup"><span data-stu-id="35262-135">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="35262-136">description</span><span class="sxs-lookup"><span data-stu-id="35262-136">description</span></span>|<span data-ttu-id="35262-137">String</span><span class="sxs-lookup"><span data-stu-id="35262-137">String</span></span>|<span data-ttu-id="35262-138">ロール割り当ての説明。</span><span class="sxs-lookup"><span data-stu-id="35262-138">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="35262-139">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="35262-139">resourceScopes</span></span>|<span data-ttu-id="35262-140">String コレクション</span><span class="sxs-lookup"><span data-stu-id="35262-140">String collection</span></span>|<span data-ttu-id="35262-141">役割のスコープ メンバーのセキュリティ グループの ID リスト。</span><span class="sxs-lookup"><span data-stu-id="35262-141">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="35262-142">Azure Active Directory の ID。</span><span class="sxs-lookup"><span data-stu-id="35262-142">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="35262-143">応答</span><span class="sxs-lookup"><span data-stu-id="35262-143">Response</span></span>
<span data-ttu-id="35262-144">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [roleAssignment](../resources/intune_rbac_roleassignment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="35262-144">If successful, this method returns a `200 OK` response code and an updated [contact](../resources/intune_rbac_roleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="35262-145">例</span><span class="sxs-lookup"><span data-stu-id="35262-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="35262-146">要求</span><span class="sxs-lookup"><span data-stu-id="35262-146">Request</span></span>
<span data-ttu-id="35262-147">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="35262-147">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}
Content-type: application/json
Content-length: 140

{
  "displayName": "Display Name value",
  "description": "Description value",
  "resourceScopes": [
    "Resource Scopes value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="35262-148">応答</span><span class="sxs-lookup"><span data-stu-id="35262-148">Response</span></span>
<span data-ttu-id="35262-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="35262-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



