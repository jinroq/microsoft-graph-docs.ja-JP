---
title: deviceAndAppManagementRoleDefinition の作成
description: 新しい deviceAndAppManagementRoleDefinition オブジェクトを作成します。
ms.openlocfilehash: 71ac4a42dcf0795ad9e1e26d20be5be09fbf0705
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023577"
---
# <a name="create-deviceandappmanagementroledefinition"></a><span data-ttu-id="5e682-103">deviceAndAppManagementRoleDefinition の作成</span><span class="sxs-lookup"><span data-stu-id="5e682-103">Create deviceAndAppManagementRoleDefinition</span></span>

> <span data-ttu-id="5e682-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="5e682-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5e682-105">新しい [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="5e682-105">Create a new [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5e682-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="5e682-106">Prerequisites</span></span>
<span data-ttu-id="5e682-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5e682-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5e682-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5e682-109">Permission type</span></span>|<span data-ttu-id="5e682-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="5e682-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5e682-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5e682-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5e682-112">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5e682-112">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="5e682-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5e682-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5e682-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5e682-114">Not supported.</span></span>|
|<span data-ttu-id="5e682-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5e682-115">Application</span></span>|<span data-ttu-id="5e682-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5e682-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5e682-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5e682-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="5e682-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5e682-118">Request headers</span></span>
|<span data-ttu-id="5e682-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5e682-119">Header</span></span>|<span data-ttu-id="5e682-120">値</span><span class="sxs-lookup"><span data-stu-id="5e682-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5e682-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5e682-121">Authorization</span></span>|<span data-ttu-id="5e682-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="5e682-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5e682-123">Accept</span><span class="sxs-lookup"><span data-stu-id="5e682-123">Accept</span></span>|<span data-ttu-id="5e682-124">application/json</span><span class="sxs-lookup"><span data-stu-id="5e682-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5e682-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="5e682-125">Request body</span></span>
<span data-ttu-id="5e682-126">要求本文で、deviceAndAppManagementRoleDefinition オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="5e682-126">In the request body, supply a JSON representation for the deviceAndAppManagementRoleDefinition object.</span></span>

<span data-ttu-id="5e682-127">次の表に、deviceAndAppManagementRoleDefinition の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="5e682-127">The following table shows the properties that are required when you create the deviceAndAppManagementRoleDefinition.</span></span>

|<span data-ttu-id="5e682-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5e682-128">Property</span></span>|<span data-ttu-id="5e682-129">型</span><span class="sxs-lookup"><span data-stu-id="5e682-129">Type</span></span>|<span data-ttu-id="5e682-130">説明</span><span class="sxs-lookup"><span data-stu-id="5e682-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5e682-131">id</span><span class="sxs-lookup"><span data-stu-id="5e682-131">id</span></span>|<span data-ttu-id="5e682-132">String</span><span class="sxs-lookup"><span data-stu-id="5e682-132">String</span></span>|<span data-ttu-id="5e682-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="5e682-133">Key of the entity.</span></span> <span data-ttu-id="5e682-134">これは読み取り専用で、自動生成されます。</span><span class="sxs-lookup"><span data-stu-id="5e682-134">This is read-only and automatically generated.</span></span> <span data-ttu-id="5e682-135">[roleDefinition](../resources/intune-rbac-roledefinition.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5e682-135">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="5e682-136">displayName</span><span class="sxs-lookup"><span data-stu-id="5e682-136">displayName</span></span>|<span data-ttu-id="5e682-137">String</span><span class="sxs-lookup"><span data-stu-id="5e682-137">String</span></span>|<span data-ttu-id="5e682-138">ロールの定義の表示名。</span><span class="sxs-lookup"><span data-stu-id="5e682-138">Display Name of the Role definition.</span></span> <span data-ttu-id="5e682-139">[roleDefinition](../resources/intune-rbac-roledefinition.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5e682-139">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="5e682-140">説明</span><span class="sxs-lookup"><span data-stu-id="5e682-140">description</span></span>|<span data-ttu-id="5e682-141">String</span><span class="sxs-lookup"><span data-stu-id="5e682-141">String</span></span>|<span data-ttu-id="5e682-142">ロールの定義の説明。</span><span class="sxs-lookup"><span data-stu-id="5e682-142">Description of the Role definition.</span></span> <span data-ttu-id="5e682-143">[roleDefinition](../resources/intune-rbac-roledefinition.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5e682-143">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="5e682-144">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="5e682-144">rolePermissions</span></span>|<span data-ttu-id="5e682-145">[rolePermission](../resources/intune-rbac-rolepermission.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="5e682-145">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="5e682-146">このロールに実行が許可されている、ロールのアクセス許可のリスト。</span><span class="sxs-lookup"><span data-stu-id="5e682-146">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="5e682-147">これらは、rolePermission の一部として定義されている actionName と一致する必要があります。</span><span class="sxs-lookup"><span data-stu-id="5e682-147">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="5e682-148">[roleDefinition](../resources/intune-rbac-roledefinition.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5e682-148">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="5e682-149">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="5e682-149">isBuiltIn</span></span>|<span data-ttu-id="5e682-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="5e682-150">Boolean</span></span>|<span data-ttu-id="5e682-151">ロールの種類。</span><span class="sxs-lookup"><span data-stu-id="5e682-151">Type of Role.</span></span> <span data-ttu-id="5e682-152">組み込みの場合は True に設定し、カスタム ロールの定義の場合は False に設定します。</span><span class="sxs-lookup"><span data-stu-id="5e682-152">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="5e682-153">[roleDefinition](../resources/intune-rbac-roledefinition.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="5e682-153">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|



## <a name="response"></a><span data-ttu-id="5e682-154">応答</span><span class="sxs-lookup"><span data-stu-id="5e682-154">Response</span></span>
<span data-ttu-id="5e682-155">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="5e682-155">If successful, this method returns a `201 Created` response code and a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5e682-156">例</span><span class="sxs-lookup"><span data-stu-id="5e682-156">Example</span></span>
### <a name="request"></a><span data-ttu-id="5e682-157">要求</span><span class="sxs-lookup"><span data-stu-id="5e682-157">Request</span></span>
<span data-ttu-id="5e682-158">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5e682-158">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5e682-159">応答</span><span class="sxs-lookup"><span data-stu-id="5e682-159">Response</span></span>
<span data-ttu-id="5e682-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="5e682-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


