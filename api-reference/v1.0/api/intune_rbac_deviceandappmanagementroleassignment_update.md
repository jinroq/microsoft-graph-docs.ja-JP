# <a name="update-deviceandappmanagementroleassignment"></a><span data-ttu-id="1be0a-101">deviceAndAppManagementRoleAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="1be0a-101">Update deviceAndAppManagementRoleAssignment</span></span>

> <span data-ttu-id="1be0a-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="1be0a-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1be0a-103">[deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="1be0a-103">Update the properties of a [deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1be0a-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="1be0a-104">Prerequisites</span></span>
<span data-ttu-id="1be0a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1be0a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="1be0a-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1be0a-107">Permission type</span></span>|<span data-ttu-id="1be0a-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="1be0a-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1be0a-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1be0a-109">Delegated (work or school account)</span></span>|<span data-ttu-id="1be0a-110">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1be0a-110">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="1be0a-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1be0a-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1be0a-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1be0a-112">Not supported.</span></span>|
|<span data-ttu-id="1be0a-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1be0a-113">Application</span></span>|<span data-ttu-id="1be0a-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1be0a-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1be0a-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1be0a-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleAssignments/{deviceAndAppManagementRoleAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="1be0a-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1be0a-116">Request headers</span></span>
|<span data-ttu-id="1be0a-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1be0a-117">Header</span></span>|<span data-ttu-id="1be0a-118">値</span><span class="sxs-lookup"><span data-stu-id="1be0a-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1be0a-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="1be0a-119">Authorization</span></span>|<span data-ttu-id="1be0a-120">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="1be0a-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1be0a-121">Accept</span><span class="sxs-lookup"><span data-stu-id="1be0a-121">Accept</span></span>|<span data-ttu-id="1be0a-122">application/json</span><span class="sxs-lookup"><span data-stu-id="1be0a-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1be0a-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="1be0a-123">Request body</span></span>
<span data-ttu-id="1be0a-124">要求本文で、[deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="1be0a-124">In the request body, supply a JSON representation for the [deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md) object.</span></span>

<span data-ttu-id="1be0a-125">次の表に、[deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="1be0a-125">The following table shows the properties that are required when you create the [deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md).</span></span>

|<span data-ttu-id="1be0a-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1be0a-126">Property</span></span>|<span data-ttu-id="1be0a-127">型</span><span class="sxs-lookup"><span data-stu-id="1be0a-127">Type</span></span>|<span data-ttu-id="1be0a-128">説明</span><span class="sxs-lookup"><span data-stu-id="1be0a-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1be0a-129">id</span><span class="sxs-lookup"><span data-stu-id="1be0a-129">id</span></span>|<span data-ttu-id="1be0a-130">String</span><span class="sxs-lookup"><span data-stu-id="1be0a-130">String</span></span>|<span data-ttu-id="1be0a-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="1be0a-131">Key of the entity.</span></span> <span data-ttu-id="1be0a-132">これは読み取り専用で、自動生成されます。</span><span class="sxs-lookup"><span data-stu-id="1be0a-132">This is read-only and automatically generated.</span></span> <span data-ttu-id="1be0a-133">[roleAssignment](../resources/intune_rbac_roleassignment.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1be0a-133">Inherited from [roleAssignment](../resources/intune_rbac_roleassignment.md)</span></span>|
|<span data-ttu-id="1be0a-134">displayName</span><span class="sxs-lookup"><span data-stu-id="1be0a-134">displayName</span></span>|<span data-ttu-id="1be0a-135">String</span><span class="sxs-lookup"><span data-stu-id="1be0a-135">String</span></span>|<span data-ttu-id="1be0a-136">ロール割り当ての表示名またはフレンドリ名。</span><span class="sxs-lookup"><span data-stu-id="1be0a-136">The display or friendly name of the role Assignment.</span></span> <span data-ttu-id="1be0a-137">[roleAssignment](../resources/intune_rbac_roleassignment.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1be0a-137">Inherited from [roleAssignment](../resources/intune_rbac_roleassignment.md)</span></span>|
|<span data-ttu-id="1be0a-138">description</span><span class="sxs-lookup"><span data-stu-id="1be0a-138">description</span></span>|<span data-ttu-id="1be0a-139">String</span><span class="sxs-lookup"><span data-stu-id="1be0a-139">String</span></span>|<span data-ttu-id="1be0a-140">ロール割り当ての説明。</span><span class="sxs-lookup"><span data-stu-id="1be0a-140">Description of the Role Assignment.</span></span> <span data-ttu-id="1be0a-141">[roleAssignment](../resources/intune_rbac_roleassignment.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1be0a-141">Inherited from [roleAssignment](../resources/intune_rbac_roleassignment.md)</span></span>|
|<span data-ttu-id="1be0a-142">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="1be0a-142">resourceScopes</span></span>|<span data-ttu-id="1be0a-143">String コレクション</span><span class="sxs-lookup"><span data-stu-id="1be0a-143">String collection</span></span>|<span data-ttu-id="1be0a-144">役割のスコープ メンバーのセキュリティ グループの ID リスト。</span><span class="sxs-lookup"><span data-stu-id="1be0a-144">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="1be0a-145">Azure Active Directory の ID。</span><span class="sxs-lookup"><span data-stu-id="1be0a-145">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="1be0a-146">[roleAssignment](../resources/intune_rbac_roleassignment.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="1be0a-146">Inherited from [roleAssignment](../resources/intune_rbac_roleassignment.md)</span></span>|
|<span data-ttu-id="1be0a-147">members</span><span class="sxs-lookup"><span data-stu-id="1be0a-147">members</span></span>|<span data-ttu-id="1be0a-148">String コレクション</span><span class="sxs-lookup"><span data-stu-id="1be0a-148">String collection</span></span>|<span data-ttu-id="1be0a-149">ロール メンバーのセキュリティ グループの ID リスト。</span><span class="sxs-lookup"><span data-stu-id="1be0a-149">The list of ids of role member security groups.</span></span> <span data-ttu-id="1be0a-150">Azure Active Directory の ID。</span><span class="sxs-lookup"><span data-stu-id="1be0a-150">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="1be0a-151">応答</span><span class="sxs-lookup"><span data-stu-id="1be0a-151">Response</span></span>
<span data-ttu-id="1be0a-152">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で、更新された [deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="1be0a-152">If successful, this method returns a `200 OK` response code and an updated [deviceAndAppManagementRoleAssignment](../resources/intune_rbac_deviceandappmanagementroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1be0a-153">例</span><span class="sxs-lookup"><span data-stu-id="1be0a-153">Example</span></span>
### <a name="request"></a><span data-ttu-id="1be0a-154">要求</span><span class="sxs-lookup"><span data-stu-id="1be0a-154">Request</span></span>
<span data-ttu-id="1be0a-155">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1be0a-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/roleAssignments/{deviceAndAppManagementRoleAssignmentId}
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

### <a name="response"></a><span data-ttu-id="1be0a-156">応答</span><span class="sxs-lookup"><span data-stu-id="1be0a-156">Response</span></span>
<span data-ttu-id="1be0a-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1be0a-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



