# <a name="update-roledefinition"></a><span data-ttu-id="e7938-101">roleDefinition の更新</span><span class="sxs-lookup"><span data-stu-id="e7938-101">Update roleDefinition</span></span>

> <span data-ttu-id="e7938-102">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e7938-102">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e7938-103">[roleDefinition](../resources/intune_rbac_roledefinition.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="e7938-103">Update the properties of a [roleDefinition](../resources/intune_rbac_roledefinition.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e7938-104">前提条件</span><span class="sxs-lookup"><span data-stu-id="e7938-104">Prerequisites</span></span>
<span data-ttu-id="e7938-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](../../../concepts/permissions_reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e7938-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](../../../concepts/permissions_reference.md).</span></span>

|<span data-ttu-id="e7938-107">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e7938-107">Permission type</span></span>|<span data-ttu-id="e7938-108">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="e7938-108">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e7938-109">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e7938-109">Delegated (work or school account)</span></span>|<span data-ttu-id="e7938-110">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7938-110">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="e7938-111">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e7938-111">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e7938-112">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e7938-112">Not supported.</span></span>|
|<span data-ttu-id="e7938-113">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e7938-113">Application</span></span>|<span data-ttu-id="e7938-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e7938-114">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e7938-115">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e7938-115">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/roleDefinition
```

## <a name="request-headers"></a><span data-ttu-id="e7938-116">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e7938-116">Request headers</span></span>
|<span data-ttu-id="e7938-117">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e7938-117">Header</span></span>|<span data-ttu-id="e7938-118">値</span><span class="sxs-lookup"><span data-stu-id="e7938-118">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e7938-119">Authorization</span><span class="sxs-lookup"><span data-stu-id="e7938-119">Authorization</span></span>|<span data-ttu-id="e7938-120">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="e7938-120">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e7938-121">Accept</span><span class="sxs-lookup"><span data-stu-id="e7938-121">Accept</span></span>|<span data-ttu-id="e7938-122">application/json</span><span class="sxs-lookup"><span data-stu-id="e7938-122">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e7938-123">要求本文</span><span class="sxs-lookup"><span data-stu-id="e7938-123">Request body</span></span>
<span data-ttu-id="e7938-124">要求本文で、[roleDefinition](../resources/intune_rbac_roledefinition.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="e7938-124">In the request body, supply a JSON representation for the [roleDefinition](../resources/intune_rbac_roledefinition.md) object.</span></span>

<span data-ttu-id="e7938-125">次の表に、[roleDefinition](../resources/intune_rbac_roledefinition.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="e7938-125">The following table shows the properties that are required when you create the [roleDefinition](../resources/intune_rbac_roledefinition.md).</span></span>

|<span data-ttu-id="e7938-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e7938-126">Property</span></span>|<span data-ttu-id="e7938-127">型</span><span class="sxs-lookup"><span data-stu-id="e7938-127">Type</span></span>|<span data-ttu-id="e7938-128">説明</span><span class="sxs-lookup"><span data-stu-id="e7938-128">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e7938-129">id</span><span class="sxs-lookup"><span data-stu-id="e7938-129">id</span></span>|<span data-ttu-id="e7938-130">String</span><span class="sxs-lookup"><span data-stu-id="e7938-130">String</span></span>|<span data-ttu-id="e7938-131">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="e7938-131">Key of the entity.</span></span> <span data-ttu-id="e7938-132">これは読み取り専用で、自動生成されます。</span><span class="sxs-lookup"><span data-stu-id="e7938-132">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="e7938-133">displayName</span><span class="sxs-lookup"><span data-stu-id="e7938-133">displayName</span></span>|<span data-ttu-id="e7938-134">String</span><span class="sxs-lookup"><span data-stu-id="e7938-134">String</span></span>|<span data-ttu-id="e7938-135">ロールの定義の表示名。</span><span class="sxs-lookup"><span data-stu-id="e7938-135">Display Name of the Role definition.</span></span>|
|<span data-ttu-id="e7938-136">description</span><span class="sxs-lookup"><span data-stu-id="e7938-136">description</span></span>|<span data-ttu-id="e7938-137">String</span><span class="sxs-lookup"><span data-stu-id="e7938-137">String</span></span>|<span data-ttu-id="e7938-138">ロールの定義の説明。</span><span class="sxs-lookup"><span data-stu-id="e7938-138">Description of the Role definition.</span></span>|
|<span data-ttu-id="e7938-139">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="e7938-139">rolePermissions</span></span>|<span data-ttu-id="e7938-140">[rolePermission](../resources/intune_rbac_rolepermission.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e7938-140">[rolePermission](../resources/intune_rbac_rolepermission.md) collection</span></span>|<span data-ttu-id="e7938-141">このロールに実行が許可されている、ロールのアクセス許可のリスト。</span><span class="sxs-lookup"><span data-stu-id="e7938-141">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="e7938-142">これらは、rolePermission の一部として定義されている actionName と一致する必要があります。</span><span class="sxs-lookup"><span data-stu-id="e7938-142">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="e7938-143">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="e7938-143">isBuiltIn</span></span>|<span data-ttu-id="e7938-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="e7938-144">Boolean</span></span>|<span data-ttu-id="e7938-145">ロールの種類。</span><span class="sxs-lookup"><span data-stu-id="e7938-145">Type of Role.</span></span> <span data-ttu-id="e7938-146">組み込みの場合は True に設定し、カスタム ロールの定義の場合は False に設定します。</span><span class="sxs-lookup"><span data-stu-id="e7938-146">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|



## <a name="response"></a><span data-ttu-id="e7938-147">応答</span><span class="sxs-lookup"><span data-stu-id="e7938-147">Response</span></span>
<span data-ttu-id="e7938-148">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [roleDefinition](../resources/intune_rbac_roledefinition.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e7938-148">If successful, this method returns a `200 OK` response code and an updated [roleDefinition](../resources/intune_rbac_roledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e7938-149">例</span><span class="sxs-lookup"><span data-stu-id="e7938-149">Example</span></span>
### <a name="request"></a><span data-ttu-id="e7938-150">要求</span><span class="sxs-lookup"><span data-stu-id="e7938-150">Request</span></span>
<span data-ttu-id="e7938-151">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e7938-151">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/roleDefinitions/{roleDefinitionId}
Content-type: application/json
Content-length: 580

{
  "@odata.type": "#microsoft.graph.roleDefinition",
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

### <a name="response"></a><span data-ttu-id="e7938-152">応答</span><span class="sxs-lookup"><span data-stu-id="e7938-152">Response</span></span>
<span data-ttu-id="e7938-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e7938-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 629

{
  "@odata.type": "#microsoft.graph.roleDefinition",
  "id": "70fdcd08-cd08-70fd-08cd-fd7008cdfd70",
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



