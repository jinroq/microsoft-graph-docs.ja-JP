# <a name="create-deviceandappmanagementroledefinition"></a><span data-ttu-id="ced57-101">deviceAndAppManagementRoleDefinition の作成</span><span class="sxs-lookup"><span data-stu-id="ced57-101">Create deviceAndAppManagementRoleDefinition</span></span>

> <span data-ttu-id="ced57-102">**注:**Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ced57-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ced57-103">新しい [deviceAndAppManagementRoleDefinition](../resources/intune_rbac_deviceandappmanagementroledefinition.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="ced57-103">Create a new [plannerBucket](../resources/intune_rbac_deviceandappmanagementroledefinition.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ced57-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="ced57-104">Prerequisites</span></span>
<span data-ttu-id="ced57-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ced57-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ced57-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ced57-107">Permission type</span></span>|<span data-ttu-id="ced57-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ced57-108">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ced57-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ced57-109">Delegated (work or school account)</span></span>|<span data-ttu-id="ced57-110">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ced57-110">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="ced57-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ced57-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ced57-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ced57-112">Not supported.</span></span>|
|<span data-ttu-id="ced57-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ced57-113">Application</span></span>|<span data-ttu-id="ced57-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ced57-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ced57-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ced57-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="ced57-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ced57-116">Request headers</span></span>
|<span data-ttu-id="ced57-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ced57-117">Header</span></span>|<span data-ttu-id="ced57-118">値</span><span class="sxs-lookup"><span data-stu-id="ced57-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ced57-119">承認</span><span class="sxs-lookup"><span data-stu-id="ced57-119">Authorization</span></span>|<span data-ttu-id="ced57-120">ベアラー &lt;トークン&gt;が必須。</span><span class="sxs-lookup"><span data-stu-id="ced57-120">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="ced57-121">承諾</span><span class="sxs-lookup"><span data-stu-id="ced57-121">Accept</span></span>|<span data-ttu-id="ced57-122">application/json</span><span class="sxs-lookup"><span data-stu-id="ced57-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ced57-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="ced57-123">Request body</span></span>
<span data-ttu-id="ced57-124">要求本文で、deviceAndAppManagementRoleDefinition オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="ced57-124">In the request body, supply a JSON representation of the schemaExtension object.</span></span>

<span data-ttu-id="ced57-125">次の表に、deviceAndAppManagementRoleDefinition の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="ced57-125">The following table shows the properties that are required when you create a user.</span></span>

|<span data-ttu-id="ced57-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ced57-126">Property</span></span>|<span data-ttu-id="ced57-127">型</span><span class="sxs-lookup"><span data-stu-id="ced57-127">Type</span></span>|<span data-ttu-id="ced57-128">説明</span><span class="sxs-lookup"><span data-stu-id="ced57-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ced57-129">id</span><span class="sxs-lookup"><span data-stu-id="ced57-129">id</span></span>|<span data-ttu-id="ced57-130">String</span><span class="sxs-lookup"><span data-stu-id="ced57-130">String</span></span>|<span data-ttu-id="ced57-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="ced57-131">Name of the entity.</span></span> <span data-ttu-id="ced57-132">これは読み取り専用で、自動生成されます。</span><span class="sxs-lookup"><span data-stu-id="ced57-132">This is read-only and automatically generated.</span></span> <span data-ttu-id="ced57-133">[roleDefinition](../resources/intune_rbac_roledefinition.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ced57-133">Inherited from [roleDefinition](../resources/intune_rbac_roledefinition.md)</span></span>|
|<span data-ttu-id="ced57-134">displayName</span><span class="sxs-lookup"><span data-stu-id="ced57-134">displayName</span></span>|<span data-ttu-id="ced57-135">String</span><span class="sxs-lookup"><span data-stu-id="ced57-135">String</span></span>|<span data-ttu-id="ced57-136">ロールの定義の表示名。</span><span class="sxs-lookup"><span data-stu-id="ced57-136">Display Name of the Role definition.</span></span> <span data-ttu-id="ced57-137">[roleDefinition](../resources/intune_rbac_roledefinition.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ced57-137">Inherited from [roleDefinition](../resources/intune_rbac_roledefinition.md)</span></span>|
|<span data-ttu-id="ced57-138">description</span><span class="sxs-lookup"><span data-stu-id="ced57-138">description</span></span>|<span data-ttu-id="ced57-139">String</span><span class="sxs-lookup"><span data-stu-id="ced57-139">String</span></span>|<span data-ttu-id="ced57-140">ロールの定義の説明。</span><span class="sxs-lookup"><span data-stu-id="ced57-140">Description of the Role definition.</span></span> <span data-ttu-id="ced57-141">[roleDefinition](../resources/intune_rbac_roledefinition.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ced57-141">Inherited from [roleDefinition](../resources/intune_rbac_roledefinition.md)</span></span>|
|<span data-ttu-id="ced57-142">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="ced57-142">rolePermissions</span></span>|<span data-ttu-id="ced57-143">[rolePermission](../resources/intune_rbac_rolepermission.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ced57-143">[rolePermission](../resources/intune_rbac_rolepermission.md) collection</span></span>|<span data-ttu-id="ced57-144">このロールに実行が許可されている、ロールのアクセス許可のリスト。</span><span class="sxs-lookup"><span data-stu-id="ced57-144">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="ced57-145">これらは、rolePermission の一部として定義されている actionName と一致する必要があります。</span><span class="sxs-lookup"><span data-stu-id="ced57-145">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="ced57-146">[roleDefinition](../resources/intune_rbac_roledefinition.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ced57-146">Inherited from [roleDefinition](../resources/intune_rbac_roledefinition.md)</span></span>|
|<span data-ttu-id="ced57-147">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="ced57-147">isBuiltIn</span></span>|<span data-ttu-id="ced57-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="ced57-148">Boolean</span></span>|<span data-ttu-id="ced57-149">ロールの種類。</span><span class="sxs-lookup"><span data-stu-id="ced57-149">Type of Role.</span></span> <span data-ttu-id="ced57-150">組み込みの場合は True に設定し、カスタム ロールの定義の場合は False に設定します。</span><span class="sxs-lookup"><span data-stu-id="ced57-150">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="ced57-151">[roleDefinition](../resources/intune_rbac_roledefinition.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ced57-151">Inherited from [roleDefinition](../resources/intune_rbac_roledefinition.md)</span></span>|



## <a name="response"></a><span data-ttu-id="ced57-152">応答</span><span class="sxs-lookup"><span data-stu-id="ced57-152">Response</span></span>
<span data-ttu-id="ced57-153">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [deviceAndAppManagementRoleDefinition](../resources/intune_rbac_deviceandappmanagementroledefinition.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ced57-153">If successful, this method returns a `201 Created` response code and a [section](../resources/intune_rbac_deviceandappmanagementroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ced57-154">例</span><span class="sxs-lookup"><span data-stu-id="ced57-154">Example</span></span>
### <a name="request"></a><span data-ttu-id="ced57-155">要求</span><span class="sxs-lookup"><span data-stu-id="ced57-155">Request</span></span>
<span data-ttu-id="ced57-156">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ced57-156">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/roleDefinitions
Content-type: application/json
Content-length: 602

{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleDefinition",
  "displayName": "Display Name value",
  "description": "Description value",
  "rolePermissions": [
    {
      "@odata.type": "microsoft.graph.rolePermission",
      "resourceActions": [
        {
          "@odata.type": "microsoft.graph.resourceAction",
          "allowedResourceActions": [
            "Allowed Resource Actions value"
          ],
          "notAllowedResourceActions": [
            "Not Allowed Resource Actions value"
          ]
        }
      ]
    }
  ],
  "isBuiltIn": true
}
```

### <a name="response"></a><span data-ttu-id="ced57-157">応答</span><span class="sxs-lookup"><span data-stu-id="ced57-157">Response</span></span>
<span data-ttu-id="ced57-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ced57-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 651

{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleDefinition",
  "id": "bca1dfb5-dfb5-bca1-b5df-a1bcb5dfa1bc",
  "displayName": "Display Name value",
  "description": "Description value",
  "rolePermissions": [
    {
      "@odata.type": "microsoft.graph.rolePermission",
      "resourceActions": [
        {
          "@odata.type": "microsoft.graph.resourceAction",
          "allowedResourceActions": [
            "Allowed Resource Actions value"
          ],
          "notAllowedResourceActions": [
            "Not Allowed Resource Actions value"
          ]
        }
      ]
    }
  ],
  "isBuiltIn": true
}
```



