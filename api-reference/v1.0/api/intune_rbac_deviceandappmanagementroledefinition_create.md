# <a name="create-deviceandappmanagementroledefinition"></a><span data-ttu-id="ec215-101">deviceAndAppManagementRoleDefinition の作成</span><span class="sxs-lookup"><span data-stu-id="ec215-101">Create deviceAndAppManagementRoleDefinition</span></span>

> <span data-ttu-id="ec215-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="ec215-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ec215-103">新しい [deviceAndAppManagementRoleDefinition](../resources/intune_rbac_deviceandappmanagementroledefinition.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="ec215-103">Create a new [deviceAndAppManagementRoleDefinition](../resources/intune_rbac_deviceandappmanagementroledefinition.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ec215-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="ec215-104">Prerequisites</span></span>
<span data-ttu-id="ec215-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ec215-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="ec215-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ec215-107">Permission type</span></span>|<span data-ttu-id="ec215-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ec215-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ec215-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ec215-109">Delegated (work or school account)</span></span>|<span data-ttu-id="ec215-110">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec215-110">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="ec215-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ec215-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ec215-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ec215-112">Not supported.</span></span>|
|<span data-ttu-id="ec215-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ec215-113">Application</span></span>|<span data-ttu-id="ec215-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ec215-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ec215-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ec215-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="ec215-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ec215-116">Request headers</span></span>
|<span data-ttu-id="ec215-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ec215-117">Header</span></span>|<span data-ttu-id="ec215-118">値</span><span class="sxs-lookup"><span data-stu-id="ec215-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ec215-119">承認</span><span class="sxs-lookup"><span data-stu-id="ec215-119">Authorization</span></span>|<span data-ttu-id="ec215-120">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="ec215-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ec215-121">承諾</span><span class="sxs-lookup"><span data-stu-id="ec215-121">Accept</span></span>|<span data-ttu-id="ec215-122">アプリケーションまたは json</span><span class="sxs-lookup"><span data-stu-id="ec215-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ec215-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="ec215-123">Request body</span></span>
<span data-ttu-id="ec215-124">要求本文で、deviceAndAppManagementRoleDefinition オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="ec215-124">In the request body, supply a JSON representation for the deviceAndAppManagementRoleDefinition object.</span></span>

<span data-ttu-id="ec215-125">次の表に、deviceAndAppManagementRoleDefinition の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="ec215-125">The following table shows the properties that are required when you create the deviceAndAppManagementRoleDefinition.</span></span>

|<span data-ttu-id="ec215-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ec215-126">Property</span></span>|<span data-ttu-id="ec215-127">型</span><span class="sxs-lookup"><span data-stu-id="ec215-127">Type</span></span>|<span data-ttu-id="ec215-128">説明</span><span class="sxs-lookup"><span data-stu-id="ec215-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ec215-129">ID</span><span class="sxs-lookup"><span data-stu-id="ec215-129">id</span></span>|<span data-ttu-id="ec215-130">文字列</span><span class="sxs-lookup"><span data-stu-id="ec215-130">String</span></span>|<span data-ttu-id="ec215-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="ec215-131">Key of the entity.</span></span> <span data-ttu-id="ec215-132">これは読み取り専用で、自動生成されます。</span><span class="sxs-lookup"><span data-stu-id="ec215-132">This is read-only and automatically generated.</span></span> <span data-ttu-id="ec215-133">[roleDefinition](../resources/intune_rbac_roledefinition.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ec215-133">Inherited from [roleDefinition](../resources/intune_rbac_roledefinition.md)</span></span>|
|<span data-ttu-id="ec215-134">displayName</span><span class="sxs-lookup"><span data-stu-id="ec215-134">displayName</span></span>|<span data-ttu-id="ec215-135">文字列</span><span class="sxs-lookup"><span data-stu-id="ec215-135">String</span></span>|<span data-ttu-id="ec215-136">ロールの定義の表示名。</span><span class="sxs-lookup"><span data-stu-id="ec215-136">Display Name of the Role definition.</span></span> <span data-ttu-id="ec215-137">[roleDefinition](../resources/intune_rbac_roledefinition.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ec215-137">Inherited from [roleDefinition](../resources/intune_rbac_roledefinition.md)</span></span>|
|<span data-ttu-id="ec215-138">説明</span><span class="sxs-lookup"><span data-stu-id="ec215-138">description</span></span>|<span data-ttu-id="ec215-139">文字列</span><span class="sxs-lookup"><span data-stu-id="ec215-139">String</span></span>|<span data-ttu-id="ec215-140">ロールの定義の説明。</span><span class="sxs-lookup"><span data-stu-id="ec215-140">Description of the Role definition.</span></span> <span data-ttu-id="ec215-141">[roleDefinition](../resources/intune_rbac_roledefinition.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ec215-141">Inherited from [roleDefinition](../resources/intune_rbac_roledefinition.md)</span></span>|
|<span data-ttu-id="ec215-142">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="ec215-142">rolePermissions</span></span>|<span data-ttu-id="ec215-143">[rolePermission](../resources/intune_rbac_rolepermission.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ec215-143">[rolePermission](../resources/intune_rbac_rolepermission.md) collection</span></span>|<span data-ttu-id="ec215-144">このロールに実行が許可されている、ロールのアクセス許可のリスト。</span><span class="sxs-lookup"><span data-stu-id="ec215-144">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="ec215-145">これらは、rolePermission の一部として定義されている actionName と一致する必要があります。</span><span class="sxs-lookup"><span data-stu-id="ec215-145">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="ec215-146">[roleDefinition](../resources/intune_rbac_roledefinition.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ec215-146">Inherited from [roleDefinition](../resources/intune_rbac_roledefinition.md)</span></span>|
|<span data-ttu-id="ec215-147">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="ec215-147">isBuiltIn</span></span>|<span data-ttu-id="ec215-148">ブール値</span><span class="sxs-lookup"><span data-stu-id="ec215-148">Boolean</span></span>|<span data-ttu-id="ec215-149">ロールの種類。</span><span class="sxs-lookup"><span data-stu-id="ec215-149">Type of Role.</span></span> <span data-ttu-id="ec215-150">組み込みの場合は True に設定し、カスタム ロールの定義の場合は False に設定します。</span><span class="sxs-lookup"><span data-stu-id="ec215-150">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="ec215-151">[roleDefinition](../resources/intune_rbac_roledefinition.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ec215-151">Inherited from [roleDefinition](../resources/intune_rbac_roledefinition.md)</span></span>|



## <a name="response"></a><span data-ttu-id="ec215-152">応答</span><span class="sxs-lookup"><span data-stu-id="ec215-152">Response</span></span>
<span data-ttu-id="ec215-153">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [deviceAndAppManagementRoleDefinition](../resources/intune_rbac_deviceandappmanagementroledefinition.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ec215-153">If successful, this method returns a `201 Created` response code and a [deviceAndAppManagementRoleDefinition](../resources/intune_rbac_deviceandappmanagementroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ec215-154">例</span><span class="sxs-lookup"><span data-stu-id="ec215-154">Example</span></span>
### <a name="request"></a><span data-ttu-id="ec215-155">要求</span><span class="sxs-lookup"><span data-stu-id="ec215-155">Request</span></span>
<span data-ttu-id="ec215-156">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ec215-156">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ec215-157">応答</span><span class="sxs-lookup"><span data-stu-id="ec215-157">Response</span></span>
<span data-ttu-id="ec215-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ec215-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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








