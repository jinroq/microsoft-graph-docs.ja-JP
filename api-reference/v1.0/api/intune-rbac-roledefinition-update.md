---
title: roleDefinition の更新
description: roleDefinition オブジェクトのプロパティを更新します。
ms.openlocfilehash: 2ceb1024b45efdf47deabac3c90fe923638f42d8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27021303"
---
# <a name="update-roledefinition"></a><span data-ttu-id="b9f20-103">roleDefinition の更新</span><span class="sxs-lookup"><span data-stu-id="b9f20-103">Update roleDefinition</span></span>

> <span data-ttu-id="b9f20-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="b9f20-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b9f20-105">[roleDefinition](../resources/intune-rbac-roledefinition.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="b9f20-105">Update the properties of a [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b9f20-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="b9f20-106">Prerequisites</span></span>
<span data-ttu-id="b9f20-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b9f20-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9f20-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b9f20-109">Permission type</span></span>|<span data-ttu-id="b9f20-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="b9f20-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b9f20-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b9f20-111">Delegated (work or school account)</span></span>|<span data-ttu-id="b9f20-112">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9f20-112">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="b9f20-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b9f20-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b9f20-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b9f20-114">Not supported.</span></span>|
|<span data-ttu-id="b9f20-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b9f20-115">Application</span></span>|<span data-ttu-id="b9f20-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b9f20-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b9f20-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b9f20-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/roleDefinition
```

## <a name="request-headers"></a><span data-ttu-id="b9f20-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b9f20-118">Request headers</span></span>
|<span data-ttu-id="b9f20-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b9f20-119">Header</span></span>|<span data-ttu-id="b9f20-120">値</span><span class="sxs-lookup"><span data-stu-id="b9f20-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b9f20-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b9f20-121">Authorization</span></span>|<span data-ttu-id="b9f20-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="b9f20-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b9f20-123">Accept</span><span class="sxs-lookup"><span data-stu-id="b9f20-123">Accept</span></span>|<span data-ttu-id="b9f20-124">application/json</span><span class="sxs-lookup"><span data-stu-id="b9f20-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b9f20-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="b9f20-125">Request body</span></span>
<span data-ttu-id="b9f20-126">要求本文で、[roleDefinition](../resources/intune-rbac-roledefinition.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="b9f20-126">In the request body, supply a JSON representation for the [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>

<span data-ttu-id="b9f20-127">次の表に、[roleDefinition](../resources/intune-rbac-roledefinition.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="b9f20-127">The following table shows the properties that are required when you create the [roleDefinition](../resources/intune-rbac-roledefinition.md).</span></span>

|<span data-ttu-id="b9f20-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b9f20-128">Property</span></span>|<span data-ttu-id="b9f20-129">型</span><span class="sxs-lookup"><span data-stu-id="b9f20-129">Type</span></span>|<span data-ttu-id="b9f20-130">説明</span><span class="sxs-lookup"><span data-stu-id="b9f20-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9f20-131">id</span><span class="sxs-lookup"><span data-stu-id="b9f20-131">id</span></span>|<span data-ttu-id="b9f20-132">String</span><span class="sxs-lookup"><span data-stu-id="b9f20-132">String</span></span>|<span data-ttu-id="b9f20-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="b9f20-133">Key of the entity.</span></span> <span data-ttu-id="b9f20-134">これは読み取り専用で、自動生成されます。</span><span class="sxs-lookup"><span data-stu-id="b9f20-134">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="b9f20-135">displayName</span><span class="sxs-lookup"><span data-stu-id="b9f20-135">displayName</span></span>|<span data-ttu-id="b9f20-136">String</span><span class="sxs-lookup"><span data-stu-id="b9f20-136">String</span></span>|<span data-ttu-id="b9f20-137">ロールの定義の表示名。</span><span class="sxs-lookup"><span data-stu-id="b9f20-137">Display Name of the Role definition.</span></span>|
|<span data-ttu-id="b9f20-138">説明</span><span class="sxs-lookup"><span data-stu-id="b9f20-138">description</span></span>|<span data-ttu-id="b9f20-139">String</span><span class="sxs-lookup"><span data-stu-id="b9f20-139">String</span></span>|<span data-ttu-id="b9f20-140">ロールの定義の説明。</span><span class="sxs-lookup"><span data-stu-id="b9f20-140">Description of the Role definition.</span></span>|
|<span data-ttu-id="b9f20-141">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="b9f20-141">rolePermissions</span></span>|<span data-ttu-id="b9f20-142">[rolePermission](../resources/intune-rbac-rolepermission.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b9f20-142">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="b9f20-143">このロールに実行が許可されている、ロールのアクセス許可のリスト。</span><span class="sxs-lookup"><span data-stu-id="b9f20-143">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="b9f20-144">これらは、rolePermission の一部として定義されている actionName と一致する必要があります。</span><span class="sxs-lookup"><span data-stu-id="b9f20-144">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="b9f20-145">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="b9f20-145">isBuiltIn</span></span>|<span data-ttu-id="b9f20-146">Boolean</span><span class="sxs-lookup"><span data-stu-id="b9f20-146">Boolean</span></span>|<span data-ttu-id="b9f20-147">ロールの種類。</span><span class="sxs-lookup"><span data-stu-id="b9f20-147">Type of Role.</span></span> <span data-ttu-id="b9f20-148">組み込みの場合は True に設定し、カスタム ロールの定義の場合は False に設定します。</span><span class="sxs-lookup"><span data-stu-id="b9f20-148">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|



## <a name="response"></a><span data-ttu-id="b9f20-149">応答</span><span class="sxs-lookup"><span data-stu-id="b9f20-149">Response</span></span>
<span data-ttu-id="b9f20-150">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [roleDefinition](../resources/intune-rbac-roledefinition.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="b9f20-150">If successful, this method returns a `200 OK` response code and an updated [roleDefinition](../resources/intune-rbac-roledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9f20-151">例</span><span class="sxs-lookup"><span data-stu-id="b9f20-151">Example</span></span>
### <a name="request"></a><span data-ttu-id="b9f20-152">要求</span><span class="sxs-lookup"><span data-stu-id="b9f20-152">Request</span></span>
<span data-ttu-id="b9f20-153">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b9f20-153">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b9f20-154">応答</span><span class="sxs-lookup"><span data-stu-id="b9f20-154">Response</span></span>
<span data-ttu-id="b9f20-p105">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b9f20-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



