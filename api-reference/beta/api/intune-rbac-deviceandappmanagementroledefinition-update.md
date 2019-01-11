---
title: deviceAndAppManagementRoleDefinition の更新
description: deviceAndAppManagementRoleDefinition オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: f11266051e85e92d10eecded661f69c40626776b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27809336"
---
# <a name="update-deviceandappmanagementroledefinition"></a><span data-ttu-id="16906-103">deviceAndAppManagementRoleDefinition の更新</span><span class="sxs-lookup"><span data-stu-id="16906-103">Update deviceAndAppManagementRoleDefinition</span></span>

> <span data-ttu-id="16906-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="16906-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="16906-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="16906-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="16906-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="16906-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="16906-107">[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="16906-107">Update the properties of a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="16906-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="16906-108">Prerequisites</span></span>
<span data-ttu-id="16906-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="16906-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="16906-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="16906-111">Permission type</span></span>|<span data-ttu-id="16906-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="16906-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="16906-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="16906-113">Delegated (work or school account)</span></span>|<span data-ttu-id="16906-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="16906-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="16906-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="16906-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="16906-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="16906-116">Not supported.</span></span>|
|<span data-ttu-id="16906-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="16906-117">Application</span></span>|<span data-ttu-id="16906-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="16906-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="16906-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="16906-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/roleDefinition
```

## <a name="request-headers"></a><span data-ttu-id="16906-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="16906-120">Request headers</span></span>
|<span data-ttu-id="16906-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="16906-121">Header</span></span>|<span data-ttu-id="16906-122">値</span><span class="sxs-lookup"><span data-stu-id="16906-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="16906-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="16906-123">Authorization</span></span>|<span data-ttu-id="16906-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="16906-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="16906-125">Accept</span><span class="sxs-lookup"><span data-stu-id="16906-125">Accept</span></span>|<span data-ttu-id="16906-126">application/json</span><span class="sxs-lookup"><span data-stu-id="16906-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="16906-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="16906-127">Request body</span></span>
<span data-ttu-id="16906-128">要求本文で、[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="16906-128">In the request body, supply a JSON representation for the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>

<span data-ttu-id="16906-129">次の表に、[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="16906-129">The following table shows the properties that are required when you create the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span></span>

|<span data-ttu-id="16906-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="16906-130">Property</span></span>|<span data-ttu-id="16906-131">種類</span><span class="sxs-lookup"><span data-stu-id="16906-131">Type</span></span>|<span data-ttu-id="16906-132">説明</span><span class="sxs-lookup"><span data-stu-id="16906-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="16906-133">ID</span><span class="sxs-lookup"><span data-stu-id="16906-133">id</span></span>|<span data-ttu-id="16906-134">String</span><span class="sxs-lookup"><span data-stu-id="16906-134">String</span></span>|<span data-ttu-id="16906-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="16906-135">Key of the entity.</span></span> <span data-ttu-id="16906-136">これは読み取り専用で、自動生成されます。</span><span class="sxs-lookup"><span data-stu-id="16906-136">This is read-only and automatically generated.</span></span> <span data-ttu-id="16906-137">[roleDefinition](../resources/intune-rbac-roledefinition.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="16906-137">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="16906-138">displayName</span><span class="sxs-lookup"><span data-stu-id="16906-138">displayName</span></span>|<span data-ttu-id="16906-139">String</span><span class="sxs-lookup"><span data-stu-id="16906-139">String</span></span>|<span data-ttu-id="16906-140">ロールの定義の表示名。</span><span class="sxs-lookup"><span data-stu-id="16906-140">Display Name of the Role definition.</span></span> <span data-ttu-id="16906-141">[roleDefinition](../resources/intune-rbac-roledefinition.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="16906-141">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="16906-142">説明</span><span class="sxs-lookup"><span data-stu-id="16906-142">description</span></span>|<span data-ttu-id="16906-143">String</span><span class="sxs-lookup"><span data-stu-id="16906-143">String</span></span>|<span data-ttu-id="16906-144">ロールの定義の説明。</span><span class="sxs-lookup"><span data-stu-id="16906-144">Description of the Role definition.</span></span> <span data-ttu-id="16906-145">[roleDefinition](../resources/intune-rbac-roledefinition.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="16906-145">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="16906-146">permissions</span><span class="sxs-lookup"><span data-stu-id="16906-146">permissions</span></span>|<span data-ttu-id="16906-147">[rolePermission](../resources/intune-rbac-rolepermission.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="16906-147">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="16906-148">このロールに実行が許可されている、ロールのアクセス許可のリスト。</span><span class="sxs-lookup"><span data-stu-id="16906-148">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="16906-149">これらは、rolePermission の一部として定義されている actionName と一致する必要があります。</span><span class="sxs-lookup"><span data-stu-id="16906-149">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="16906-150">[roleDefinition](../resources/intune-rbac-roledefinition.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="16906-150">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="16906-151">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="16906-151">rolePermissions</span></span>|<span data-ttu-id="16906-152">[rolePermission](../resources/intune-rbac-rolepermission.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="16906-152">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="16906-153">このロールに実行が許可されている、ロールのアクセス許可のリスト。</span><span class="sxs-lookup"><span data-stu-id="16906-153">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="16906-154">これらは、rolePermission の一部として定義されている actionName と一致する必要があります。</span><span class="sxs-lookup"><span data-stu-id="16906-154">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="16906-155">[roleDefinition](../resources/intune-rbac-roledefinition.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="16906-155">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="16906-156">isBuiltInRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="16906-156">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="16906-157">Boolean</span><span class="sxs-lookup"><span data-stu-id="16906-157">Boolean</span></span>|<span data-ttu-id="16906-158">ロールの種類。</span><span class="sxs-lookup"><span data-stu-id="16906-158">Type of Role.</span></span> <span data-ttu-id="16906-159">組み込みの場合は True に設定し、カスタム ロールの定義の場合は False に設定します。</span><span class="sxs-lookup"><span data-stu-id="16906-159">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="16906-160">[roleDefinition](../resources/intune-rbac-roledefinition.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="16906-160">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="16906-161">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="16906-161">isBuiltIn</span></span>|<span data-ttu-id="16906-162">Boolean</span><span class="sxs-lookup"><span data-stu-id="16906-162">Boolean</span></span>|<span data-ttu-id="16906-163">ロールの種類。</span><span class="sxs-lookup"><span data-stu-id="16906-163">Type of Role.</span></span> <span data-ttu-id="16906-164">組み込みの場合は True に設定し、カスタム ロールの定義の場合は False に設定します。</span><span class="sxs-lookup"><span data-stu-id="16906-164">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="16906-165">[roleDefinition](../resources/intune-rbac-roledefinition.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="16906-165">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|



## <a name="response"></a><span data-ttu-id="16906-166">応答</span><span class="sxs-lookup"><span data-stu-id="16906-166">Response</span></span>
<span data-ttu-id="16906-167">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="16906-167">If successful, this method returns a `200 OK` response code and an updated [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="16906-168">例</span><span class="sxs-lookup"><span data-stu-id="16906-168">Example</span></span>
### <a name="request"></a><span data-ttu-id="16906-169">要求</span><span class="sxs-lookup"><span data-stu-id="16906-169">Request</span></span>
<span data-ttu-id="16906-170">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="16906-170">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="16906-171">応答</span><span class="sxs-lookup"><span data-stu-id="16906-171">Response</span></span>
<span data-ttu-id="16906-p110">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="16906-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1216

{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleDefinition",
  "id": "bca1dfb5-dfb5-bca1-b5df-a1bcb5dfa1bc",
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





