# <a name="create-deviceandappmanagementroleassignment"></a><span data-ttu-id="01f7d-101">deviceAndAppManagementRoleAssignment の作成</span><span class="sxs-lookup"><span data-stu-id="01f7d-101">Create deviceAndAppManagementRoleAssignment</span></span>

> <span data-ttu-id="01f7d-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="01f7d-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="01f7d-103">新しい [deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="01f7d-103">Create a new [plannerBucket](../resources/intune_rbac_deviceandappmanagementroleassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="01f7d-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="01f7d-104">Prerequisites</span></span>
<span data-ttu-id="01f7d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="01f7d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="01f7d-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="01f7d-107">Permission type</span></span>|<span data-ttu-id="01f7d-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="01f7d-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="01f7d-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="01f7d-109">Delegated (work or school account)</span></span>|<span data-ttu-id="01f7d-110">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01f7d-110">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="01f7d-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="01f7d-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="01f7d-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="01f7d-112">Not supported.</span></span>|
|<span data-ttu-id="01f7d-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="01f7d-113">Application</span></span>|<span data-ttu-id="01f7d-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="01f7d-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="01f7d-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="01f7d-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="01f7d-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="01f7d-116">Request headers</span></span>
|<span data-ttu-id="01f7d-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="01f7d-117">Header</span></span>|<span data-ttu-id="01f7d-118">値</span><span class="sxs-lookup"><span data-stu-id="01f7d-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="01f7d-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="01f7d-119">Authorization</span></span>|<span data-ttu-id="01f7d-120">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="01f7d-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="01f7d-121">Accept</span><span class="sxs-lookup"><span data-stu-id="01f7d-121">Accept</span></span>|<span data-ttu-id="01f7d-122">application/json</span><span class="sxs-lookup"><span data-stu-id="01f7d-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="01f7d-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="01f7d-123">Request body</span></span>
<span data-ttu-id="01f7d-124">要求本文で、deviceAndAppManagementRoleAssignment オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="01f7d-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="01f7d-125">次の表に、deviceAndAppManagementRoleAssignment の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="01f7d-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="01f7d-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="01f7d-126">Property</span></span>|<span data-ttu-id="01f7d-127">型</span><span class="sxs-lookup"><span data-stu-id="01f7d-127">Type</span></span>|<span data-ttu-id="01f7d-128">説明</span><span class="sxs-lookup"><span data-stu-id="01f7d-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="01f7d-129">id</span><span class="sxs-lookup"><span data-stu-id="01f7d-129">id</span></span>|<span data-ttu-id="01f7d-130">String</span><span class="sxs-lookup"><span data-stu-id="01f7d-130">String</span></span>|<span data-ttu-id="01f7d-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="01f7d-131">Name of the entity.</span></span> <span data-ttu-id="01f7d-132">これは読み取り専用で、自動生成されます。</span><span class="sxs-lookup"><span data-stu-id="01f7d-132">This is read-only and automatically generated.</span></span> <span data-ttu-id="01f7d-133">[roleAssignment](../resources/intune_rbac_roleassignment.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="01f7d-133">Inherited from [roleAssignment](../resources/intune_rbac_roleassignment.md)</span></span>|
|<span data-ttu-id="01f7d-134">displayName</span><span class="sxs-lookup"><span data-stu-id="01f7d-134">displayName</span></span>|<span data-ttu-id="01f7d-135">String</span><span class="sxs-lookup"><span data-stu-id="01f7d-135">String</span></span>|<span data-ttu-id="01f7d-136">ロール割り当ての表示名またはフレンドリ名。</span><span class="sxs-lookup"><span data-stu-id="01f7d-136">The display or friendly name of the role Assignment.</span></span> <span data-ttu-id="01f7d-137">[roleAssignment](../resources/intune_rbac_roleassignment.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="01f7d-137">Inherited from [roleAssignment](../resources/intune_rbac_roleassignment.md)</span></span>|
|<span data-ttu-id="01f7d-138">description</span><span class="sxs-lookup"><span data-stu-id="01f7d-138">description</span></span>|<span data-ttu-id="01f7d-139">String</span><span class="sxs-lookup"><span data-stu-id="01f7d-139">String</span></span>|<span data-ttu-id="01f7d-140">ロール割り当ての説明。</span><span class="sxs-lookup"><span data-stu-id="01f7d-140">Description of the Role Assignment.</span></span> <span data-ttu-id="01f7d-141">[roleAssignment](../resources/intune_rbac_roleassignment.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="01f7d-141">Inherited from [roleAssignment](../resources/intune_rbac_roleassignment.md)</span></span>|
|<span data-ttu-id="01f7d-142">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="01f7d-142">resourceScopes</span></span>|<span data-ttu-id="01f7d-143">String コレクション</span><span class="sxs-lookup"><span data-stu-id="01f7d-143">String collection</span></span>|<span data-ttu-id="01f7d-144">役割のスコープ メンバーのセキュリティ グループの ID リスト。</span><span class="sxs-lookup"><span data-stu-id="01f7d-144">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="01f7d-145">Azure Active Directory の ID。</span><span class="sxs-lookup"><span data-stu-id="01f7d-145">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="01f7d-146">[roleAssignment](../resources/intune_rbac_roleassignment.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="01f7d-146">Inherited from [roleAssignment](../resources/intune_rbac_roleassignment.md)</span></span>|
|<span data-ttu-id="01f7d-147">members</span><span class="sxs-lookup"><span data-stu-id="01f7d-147">members</span></span>|<span data-ttu-id="01f7d-148">String コレクション</span><span class="sxs-lookup"><span data-stu-id="01f7d-148">String collection</span></span>|<span data-ttu-id="01f7d-149">ロール メンバーのセキュリティ グループの ID リスト。</span><span class="sxs-lookup"><span data-stu-id="01f7d-149">The list of ids of role member security groups.</span></span> <span data-ttu-id="01f7d-150">Azure Active Directory の ID。</span><span class="sxs-lookup"><span data-stu-id="01f7d-150">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="01f7d-151">応答</span><span class="sxs-lookup"><span data-stu-id="01f7d-151">Response</span></span>
<span data-ttu-id="01f7d-152">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="01f7d-152">If successful, this method returns a `201 Created` response code and a [DriveItemVersion](../resources/intune_rbac_deviceandappmanagementroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="01f7d-153">例</span><span class="sxs-lookup"><span data-stu-id="01f7d-153">Example</span></span>
### <a name="request"></a><span data-ttu-id="01f7d-154">要求</span><span class="sxs-lookup"><span data-stu-id="01f7d-154">Request</span></span>
<span data-ttu-id="01f7d-155">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="01f7d-155">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/roleAssignments
Content-type: application/json
Content-length: 258

{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleAssignment",
  "displayName": "Display Name value",
  "description": "Description value",
  "resourceScopes": [
    "Resource Scopes value"
  ],
  "members": [
    "Members value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="01f7d-156">応答</span><span class="sxs-lookup"><span data-stu-id="01f7d-156">Response</span></span>
<span data-ttu-id="01f7d-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="01f7d-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 307

{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleAssignment",
  "id": "a12e8ebb-8ebb-a12e-bb8e-2ea1bb8e2ea1",
  "displayName": "Display Name value",
  "description": "Description value",
  "resourceScopes": [
    "Resource Scopes value"
  ],
  "members": [
    "Members value"
  ]
}
```



