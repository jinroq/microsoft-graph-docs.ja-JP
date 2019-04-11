---
title: deviceAndAppManagementRoleDefinition の更新
description: deviceAndAppManagementRoleDefinition オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2279a89aa47802b94f58f92851014d1e0b0eb312
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31785581"
---
# <a name="update-deviceandappmanagementroledefinition"></a><span data-ttu-id="20606-103">deviceAndAppManagementRoleDefinition の更新</span><span class="sxs-lookup"><span data-stu-id="20606-103">Update deviceAndAppManagementRoleDefinition</span></span>

> <span data-ttu-id="20606-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="20606-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="20606-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="20606-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="20606-106">[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="20606-106">Update the properties of a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="20606-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="20606-107">Prerequisites</span></span>
<span data-ttu-id="20606-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="20606-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="20606-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="20606-110">Permission type</span></span>|<span data-ttu-id="20606-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="20606-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="20606-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="20606-112">Delegated (work or school account)</span></span>|<span data-ttu-id="20606-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="20606-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="20606-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="20606-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="20606-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="20606-115">Not supported.</span></span>|
|<span data-ttu-id="20606-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="20606-116">Application</span></span>|<span data-ttu-id="20606-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="20606-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="20606-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="20606-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/roleDefinition
```

## <a name="request-headers"></a><span data-ttu-id="20606-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="20606-119">Request headers</span></span>
|<span data-ttu-id="20606-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="20606-120">Header</span></span>|<span data-ttu-id="20606-121">値</span><span class="sxs-lookup"><span data-stu-id="20606-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="20606-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="20606-122">Authorization</span></span>|<span data-ttu-id="20606-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="20606-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="20606-124">承諾</span><span class="sxs-lookup"><span data-stu-id="20606-124">Accept</span></span>|<span data-ttu-id="20606-125">application/json</span><span class="sxs-lookup"><span data-stu-id="20606-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="20606-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="20606-126">Request body</span></span>
<span data-ttu-id="20606-127">要求本文で、[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="20606-127">In the request body, supply a JSON representation for the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>

<span data-ttu-id="20606-128">次の表に、[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="20606-128">The following table shows the properties that are required when you create the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span></span>

|<span data-ttu-id="20606-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="20606-129">Property</span></span>|<span data-ttu-id="20606-130">型</span><span class="sxs-lookup"><span data-stu-id="20606-130">Type</span></span>|<span data-ttu-id="20606-131">説明</span><span class="sxs-lookup"><span data-stu-id="20606-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="20606-132">id</span><span class="sxs-lookup"><span data-stu-id="20606-132">id</span></span>|<span data-ttu-id="20606-133">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="20606-133">String</span></span>|<span data-ttu-id="20606-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="20606-134">Key of the entity.</span></span> <span data-ttu-id="20606-135">これは読み取り専用で、自動生成されます。</span><span class="sxs-lookup"><span data-stu-id="20606-135">This is read-only and automatically generated.</span></span> <span data-ttu-id="20606-136">[roleDefinition](../resources/intune-rbac-roledefinition.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="20606-136">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="20606-137">displayName</span><span class="sxs-lookup"><span data-stu-id="20606-137">displayName</span></span>|<span data-ttu-id="20606-138">String</span><span class="sxs-lookup"><span data-stu-id="20606-138">String</span></span>|<span data-ttu-id="20606-139">ロールの定義の表示名。</span><span class="sxs-lookup"><span data-stu-id="20606-139">Display Name of the Role definition.</span></span> <span data-ttu-id="20606-140">[roleDefinition](../resources/intune-rbac-roledefinition.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="20606-140">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="20606-141">説明</span><span class="sxs-lookup"><span data-stu-id="20606-141">description</span></span>|<span data-ttu-id="20606-142">String</span><span class="sxs-lookup"><span data-stu-id="20606-142">String</span></span>|<span data-ttu-id="20606-143">ロールの定義の説明。</span><span class="sxs-lookup"><span data-stu-id="20606-143">Description of the Role definition.</span></span> <span data-ttu-id="20606-144">[roleDefinition](../resources/intune-rbac-roledefinition.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="20606-144">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="20606-145">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="20606-145">permissions</span></span>|<span data-ttu-id="20606-146">[rolePermission](../resources/intune-rbac-rolepermission.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="20606-146">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="20606-147">このロールに実行が許可されている、ロールのアクセス許可のリスト。</span><span class="sxs-lookup"><span data-stu-id="20606-147">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="20606-148">これらは、rolePermission の一部として定義されている actionName と一致する必要があります。</span><span class="sxs-lookup"><span data-stu-id="20606-148">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="20606-149">[roleDefinition](../resources/intune-rbac-roledefinition.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="20606-149">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="20606-150">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="20606-150">rolePermissions</span></span>|<span data-ttu-id="20606-151">[rolePermission](../resources/intune-rbac-rolepermission.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="20606-151">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="20606-152">このロールに実行が許可されている、ロールのアクセス許可のリスト。</span><span class="sxs-lookup"><span data-stu-id="20606-152">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="20606-153">これらは、rolePermission の一部として定義されている actionName と一致する必要があります。</span><span class="sxs-lookup"><span data-stu-id="20606-153">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="20606-154">[roleDefinition](../resources/intune-rbac-roledefinition.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="20606-154">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="20606-155">isBuiltInRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="20606-155">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="20606-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="20606-156">Boolean</span></span>|<span data-ttu-id="20606-157">ロールの種類。</span><span class="sxs-lookup"><span data-stu-id="20606-157">Type of Role.</span></span> <span data-ttu-id="20606-158">組み込みの場合は True に設定し、カスタム ロールの定義の場合は False に設定します。</span><span class="sxs-lookup"><span data-stu-id="20606-158">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="20606-159">[roleDefinition](../resources/intune-rbac-roledefinition.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="20606-159">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="20606-160">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="20606-160">isBuiltIn</span></span>|<span data-ttu-id="20606-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="20606-161">Boolean</span></span>|<span data-ttu-id="20606-162">ロールの種類。</span><span class="sxs-lookup"><span data-stu-id="20606-162">Type of Role.</span></span> <span data-ttu-id="20606-163">組み込みの場合は True に設定し、カスタム ロールの定義の場合は False に設定します。</span><span class="sxs-lookup"><span data-stu-id="20606-163">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="20606-164">[roleDefinition](../resources/intune-rbac-roledefinition.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="20606-164">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="20606-165">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="20606-165">roleScopeTagIds</span></span>|<span data-ttu-id="20606-166">String コレクション</span><span class="sxs-lookup"><span data-stu-id="20606-166">String collection</span></span>|<span data-ttu-id="20606-167">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="20606-167">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="20606-168">[roleDefinition](../resources/intune-rbac-roledefinition.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="20606-168">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|



## <a name="response"></a><span data-ttu-id="20606-169">応答</span><span class="sxs-lookup"><span data-stu-id="20606-169">Response</span></span>
<span data-ttu-id="20606-170">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="20606-170">If successful, this method returns a `200 OK` response code and an updated [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="20606-171">例</span><span class="sxs-lookup"><span data-stu-id="20606-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="20606-172">要求</span><span class="sxs-lookup"><span data-stu-id="20606-172">Request</span></span>
<span data-ttu-id="20606-173">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="20606-173">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/roleDefinitions/{roleDefinitionId}
Content-type: application/json
Content-length: 1229

{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleDefinition",
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
  "isBuiltIn": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="20606-174">応答</span><span class="sxs-lookup"><span data-stu-id="20606-174">Response</span></span>
<span data-ttu-id="20606-p110">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="20606-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1278

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
  "isBuiltIn": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```





