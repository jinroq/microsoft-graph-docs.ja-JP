---
title: roleDefinition の更新
description: roleDefinition オブジェクトのプロパティを更新します。
ms.openlocfilehash: debf63b5d0b7116a1e8d1f9274868d97c3cb8931
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067110"
---
# <a name="update-roledefinition"></a><span data-ttu-id="78a01-103">roleDefinition の更新</span><span class="sxs-lookup"><span data-stu-id="78a01-103">Update roleDefinition</span></span>

> <span data-ttu-id="78a01-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="78a01-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="78a01-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="78a01-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="78a01-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="78a01-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="78a01-107">[roleDefinition](../resources/intune-rbac-roledefinition.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="78a01-107">Update the properties of a [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="78a01-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="78a01-108">Prerequisites</span></span>
<span data-ttu-id="78a01-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="78a01-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="78a01-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="78a01-111">Permission type</span></span>|<span data-ttu-id="78a01-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="78a01-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="78a01-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="78a01-113">Delegated (work or school account)</span></span>|<span data-ttu-id="78a01-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="78a01-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="78a01-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="78a01-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="78a01-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="78a01-116">Not supported.</span></span>|
|<span data-ttu-id="78a01-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="78a01-117">Application</span></span>|<span data-ttu-id="78a01-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="78a01-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="78a01-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="78a01-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/roleDefinition
```

## <a name="request-headers"></a><span data-ttu-id="78a01-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="78a01-120">Request headers</span></span>
|<span data-ttu-id="78a01-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="78a01-121">Header</span></span>|<span data-ttu-id="78a01-122">値</span><span class="sxs-lookup"><span data-stu-id="78a01-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="78a01-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="78a01-123">Authorization</span></span>|<span data-ttu-id="78a01-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="78a01-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="78a01-125">Accept</span><span class="sxs-lookup"><span data-stu-id="78a01-125">Accept</span></span>|<span data-ttu-id="78a01-126">application/json</span><span class="sxs-lookup"><span data-stu-id="78a01-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="78a01-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="78a01-127">Request body</span></span>
<span data-ttu-id="78a01-128">要求本文で、[roleDefinition](../resources/intune-rbac-roledefinition.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="78a01-128">In the request body, supply a JSON representation for the [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>

<span data-ttu-id="78a01-129">次の表に、[roleDefinition](../resources/intune-rbac-roledefinition.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="78a01-129">The following table shows the properties that are required when you create the [roleDefinition](../resources/intune-rbac-roledefinition.md).</span></span>

|<span data-ttu-id="78a01-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="78a01-130">Property</span></span>|<span data-ttu-id="78a01-131">型</span><span class="sxs-lookup"><span data-stu-id="78a01-131">Type</span></span>|<span data-ttu-id="78a01-132">説明</span><span class="sxs-lookup"><span data-stu-id="78a01-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="78a01-133">id</span><span class="sxs-lookup"><span data-stu-id="78a01-133">id</span></span>|<span data-ttu-id="78a01-134">String</span><span class="sxs-lookup"><span data-stu-id="78a01-134">String</span></span>|<span data-ttu-id="78a01-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="78a01-135">Key of the entity.</span></span> <span data-ttu-id="78a01-136">これは読み取り専用で、自動生成されます。</span><span class="sxs-lookup"><span data-stu-id="78a01-136">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="78a01-137">displayName</span><span class="sxs-lookup"><span data-stu-id="78a01-137">displayName</span></span>|<span data-ttu-id="78a01-138">String</span><span class="sxs-lookup"><span data-stu-id="78a01-138">String</span></span>|<span data-ttu-id="78a01-139">ロールの定義の表示名。</span><span class="sxs-lookup"><span data-stu-id="78a01-139">Display Name of the Role definition.</span></span>|
|<span data-ttu-id="78a01-140">説明</span><span class="sxs-lookup"><span data-stu-id="78a01-140">description</span></span>|<span data-ttu-id="78a01-141">String</span><span class="sxs-lookup"><span data-stu-id="78a01-141">String</span></span>|<span data-ttu-id="78a01-142">ロールの定義の説明。</span><span class="sxs-lookup"><span data-stu-id="78a01-142">Description of the Role definition.</span></span>|
|<span data-ttu-id="78a01-143">permissions</span><span class="sxs-lookup"><span data-stu-id="78a01-143">permissions</span></span>|<span data-ttu-id="78a01-144">[rolePermission](../resources/intune-rbac-rolepermission.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="78a01-144">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="78a01-145">このロールに実行が許可されている、ロールのアクセス許可のリスト。</span><span class="sxs-lookup"><span data-stu-id="78a01-145">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="78a01-146">これらは、rolePermission の一部として定義されている actionName と一致する必要があります。</span><span class="sxs-lookup"><span data-stu-id="78a01-146">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="78a01-147">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="78a01-147">rolePermissions</span></span>|<span data-ttu-id="78a01-148">[rolePermission](../resources/intune-rbac-rolepermission.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="78a01-148">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="78a01-149">このロールに実行が許可されている、ロールのアクセス許可のリスト。</span><span class="sxs-lookup"><span data-stu-id="78a01-149">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="78a01-150">これらは、rolePermission の一部として定義されている actionName と一致する必要があります。</span><span class="sxs-lookup"><span data-stu-id="78a01-150">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="78a01-151">isBuiltInRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="78a01-151">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="78a01-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="78a01-152">Boolean</span></span>|<span data-ttu-id="78a01-153">ロールの種類。</span><span class="sxs-lookup"><span data-stu-id="78a01-153">Type of Role.</span></span> <span data-ttu-id="78a01-154">組み込みの場合は True に設定し、カスタム ロールの定義の場合は False に設定します。</span><span class="sxs-lookup"><span data-stu-id="78a01-154">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|
|<span data-ttu-id="78a01-155">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="78a01-155">isBuiltIn</span></span>|<span data-ttu-id="78a01-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="78a01-156">Boolean</span></span>|<span data-ttu-id="78a01-157">ロールの種類。</span><span class="sxs-lookup"><span data-stu-id="78a01-157">Type of Role.</span></span> <span data-ttu-id="78a01-158">組み込みの場合は True に設定し、カスタム ロールの定義の場合は False に設定します。</span><span class="sxs-lookup"><span data-stu-id="78a01-158">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|



## <a name="response"></a><span data-ttu-id="78a01-159">応答</span><span class="sxs-lookup"><span data-stu-id="78a01-159">Response</span></span>
<span data-ttu-id="78a01-160">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [roleDefinition](../resources/intune-rbac-roledefinition.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="78a01-160">If successful, this method returns a `200 OK` response code and an updated [roleDefinition](../resources/intune-rbac-roledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="78a01-161">例</span><span class="sxs-lookup"><span data-stu-id="78a01-161">Example</span></span>
### <a name="request"></a><span data-ttu-id="78a01-162">要求</span><span class="sxs-lookup"><span data-stu-id="78a01-162">Request</span></span>
<span data-ttu-id="78a01-163">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="78a01-163">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/roleDefinitions/{roleDefinitionId}
Content-type: application/json
Content-length: 1092

{
  "displayName": "Display Name value",
  "description": "Description value",
  "permissions": [
    {
      "@odata.type": "microsoft.graph.rolePermission",
      "actions": [
        "Actions value"
      ],
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
  "rolePermissions": [
    {
      "@odata.type": "microsoft.graph.rolePermission",
      "actions": [
        "Actions value"
      ],
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
  "isBuiltInRoleDefinition": true,
  "isBuiltIn": true
}
```

### <a name="response"></a><span data-ttu-id="78a01-164">応答</span><span class="sxs-lookup"><span data-stu-id="78a01-164">Response</span></span>
<span data-ttu-id="78a01-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="78a01-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1194

{
  "@odata.type": "#microsoft.graph.roleDefinition",
  "id": "70fdcd08-cd08-70fd-08cd-fd7008cdfd70",
  "displayName": "Display Name value",
  "description": "Description value",
  "permissions": [
    {
      "@odata.type": "microsoft.graph.rolePermission",
      "actions": [
        "Actions value"
      ],
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
  "rolePermissions": [
    {
      "@odata.type": "microsoft.graph.rolePermission",
      "actions": [
        "Actions value"
      ],
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
  "isBuiltInRoleDefinition": true,
  "isBuiltIn": true
}
```





