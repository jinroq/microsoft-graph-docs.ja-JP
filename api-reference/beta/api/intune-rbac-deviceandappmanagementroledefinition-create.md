---
title: deviceAndAppManagementRoleDefinition の作成
description: 新しい deviceAndAppManagementRoleDefinition オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f6ca8009eeb873cd10fdec05a444e49ea74517bb
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30970752"
---
# <a name="create-deviceandappmanagementroledefinition"></a><span data-ttu-id="ca7f3-103">deviceAndAppManagementRoleDefinition の作成</span><span class="sxs-lookup"><span data-stu-id="ca7f3-103">Create deviceAndAppManagementRoleDefinition</span></span>

> <span data-ttu-id="ca7f3-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ca7f3-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ca7f3-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ca7f3-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ca7f3-106">新しい [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="ca7f3-106">Create a new [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ca7f3-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="ca7f3-107">Prerequisites</span></span>
<span data-ttu-id="ca7f3-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ca7f3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ca7f3-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ca7f3-110">Permission type</span></span>|<span data-ttu-id="ca7f3-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ca7f3-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ca7f3-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ca7f3-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ca7f3-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca7f3-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="ca7f3-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ca7f3-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ca7f3-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ca7f3-115">Not supported.</span></span>|
|<span data-ttu-id="ca7f3-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ca7f3-116">Application</span></span>|<span data-ttu-id="ca7f3-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ca7f3-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ca7f3-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ca7f3-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="ca7f3-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ca7f3-119">Request headers</span></span>
|<span data-ttu-id="ca7f3-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ca7f3-120">Header</span></span>|<span data-ttu-id="ca7f3-121">値</span><span class="sxs-lookup"><span data-stu-id="ca7f3-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ca7f3-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ca7f3-122">Authorization</span></span>|<span data-ttu-id="ca7f3-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="ca7f3-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ca7f3-124">承諾</span><span class="sxs-lookup"><span data-stu-id="ca7f3-124">Accept</span></span>|<span data-ttu-id="ca7f3-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ca7f3-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ca7f3-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="ca7f3-126">Request body</span></span>
<span data-ttu-id="ca7f3-127">要求本文で、deviceAndAppManagementRoleDefinition オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="ca7f3-127">In the request body, supply a JSON representation for the deviceAndAppManagementRoleDefinition object.</span></span>

<span data-ttu-id="ca7f3-128">次の表に、deviceAndAppManagementRoleDefinition の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="ca7f3-128">The following table shows the properties that are required when you create the deviceAndAppManagementRoleDefinition.</span></span>

|<span data-ttu-id="ca7f3-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ca7f3-129">Property</span></span>|<span data-ttu-id="ca7f3-130">型</span><span class="sxs-lookup"><span data-stu-id="ca7f3-130">Type</span></span>|<span data-ttu-id="ca7f3-131">説明</span><span class="sxs-lookup"><span data-stu-id="ca7f3-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca7f3-132">id</span><span class="sxs-lookup"><span data-stu-id="ca7f3-132">id</span></span>|<span data-ttu-id="ca7f3-133">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="ca7f3-133">String</span></span>|<span data-ttu-id="ca7f3-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="ca7f3-134">Key of the entity.</span></span> <span data-ttu-id="ca7f3-135">これは読み取り専用で、自動生成されます。</span><span class="sxs-lookup"><span data-stu-id="ca7f3-135">This is read-only and automatically generated.</span></span> <span data-ttu-id="ca7f3-136">[roleDefinition](../resources/intune-rbac-roledefinition.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ca7f3-136">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="ca7f3-137">displayName</span><span class="sxs-lookup"><span data-stu-id="ca7f3-137">displayName</span></span>|<span data-ttu-id="ca7f3-138">String</span><span class="sxs-lookup"><span data-stu-id="ca7f3-138">String</span></span>|<span data-ttu-id="ca7f3-139">ロールの定義の表示名。</span><span class="sxs-lookup"><span data-stu-id="ca7f3-139">Display Name of the Role definition.</span></span> <span data-ttu-id="ca7f3-140">[roleDefinition](../resources/intune-rbac-roledefinition.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ca7f3-140">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="ca7f3-141">description</span><span class="sxs-lookup"><span data-stu-id="ca7f3-141">description</span></span>|<span data-ttu-id="ca7f3-142">String</span><span class="sxs-lookup"><span data-stu-id="ca7f3-142">String</span></span>|<span data-ttu-id="ca7f3-143">ロールの定義の説明。</span><span class="sxs-lookup"><span data-stu-id="ca7f3-143">Description of the Role definition.</span></span> <span data-ttu-id="ca7f3-144">[roleDefinition](../resources/intune-rbac-roledefinition.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ca7f3-144">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="ca7f3-145">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="ca7f3-145">permissions</span></span>|<span data-ttu-id="ca7f3-146">[rolePermission](../resources/intune-rbac-rolepermission.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ca7f3-146">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="ca7f3-147">このロールに実行が許可されている、ロールのアクセス許可のリスト。</span><span class="sxs-lookup"><span data-stu-id="ca7f3-147">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="ca7f3-148">これらは、rolePermission の一部として定義されている actionName と一致する必要があります。</span><span class="sxs-lookup"><span data-stu-id="ca7f3-148">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="ca7f3-149">[roleDefinition](../resources/intune-rbac-roledefinition.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ca7f3-149">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="ca7f3-150">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="ca7f3-150">rolePermissions</span></span>|<span data-ttu-id="ca7f3-151">[rolePermission](../resources/intune-rbac-rolepermission.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="ca7f3-151">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="ca7f3-152">このロールに実行が許可されている、ロールのアクセス許可のリスト。</span><span class="sxs-lookup"><span data-stu-id="ca7f3-152">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="ca7f3-153">これらは、rolePermission の一部として定義されている actionName と一致する必要があります。</span><span class="sxs-lookup"><span data-stu-id="ca7f3-153">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="ca7f3-154">[roleDefinition](../resources/intune-rbac-roledefinition.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ca7f3-154">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="ca7f3-155">isBuiltInRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="ca7f3-155">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="ca7f3-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="ca7f3-156">Boolean</span></span>|<span data-ttu-id="ca7f3-157">ロールの種類。</span><span class="sxs-lookup"><span data-stu-id="ca7f3-157">Type of Role.</span></span> <span data-ttu-id="ca7f3-158">組み込みの場合は True に設定し、カスタム ロールの定義の場合は False に設定します。</span><span class="sxs-lookup"><span data-stu-id="ca7f3-158">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="ca7f3-159">[roleDefinition](../resources/intune-rbac-roledefinition.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ca7f3-159">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="ca7f3-160">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="ca7f3-160">isBuiltIn</span></span>|<span data-ttu-id="ca7f3-161">Boolean</span><span class="sxs-lookup"><span data-stu-id="ca7f3-161">Boolean</span></span>|<span data-ttu-id="ca7f3-162">ロールの種類。</span><span class="sxs-lookup"><span data-stu-id="ca7f3-162">Type of Role.</span></span> <span data-ttu-id="ca7f3-163">組み込みの場合は True に設定し、カスタム ロールの定義の場合は False に設定します。</span><span class="sxs-lookup"><span data-stu-id="ca7f3-163">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="ca7f3-164">[roleDefinition](../resources/intune-rbac-roledefinition.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ca7f3-164">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="ca7f3-165">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="ca7f3-165">roleScopeTagIds</span></span>|<span data-ttu-id="ca7f3-166">String collection</span><span class="sxs-lookup"><span data-stu-id="ca7f3-166">String collection</span></span>|<span data-ttu-id="ca7f3-167">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="ca7f3-167">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="ca7f3-168">[roleDefinition](../resources/intune-rbac-roledefinition.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="ca7f3-168">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|



## <a name="response"></a><span data-ttu-id="ca7f3-169">応答</span><span class="sxs-lookup"><span data-stu-id="ca7f3-169">Response</span></span>
<span data-ttu-id="ca7f3-170">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ca7f3-170">If successful, this method returns a `201 Created` response code and a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ca7f3-171">例</span><span class="sxs-lookup"><span data-stu-id="ca7f3-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="ca7f3-172">要求</span><span class="sxs-lookup"><span data-stu-id="ca7f3-172">Request</span></span>
<span data-ttu-id="ca7f3-173">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ca7f3-173">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/roleDefinitions
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

### <a name="response"></a><span data-ttu-id="ca7f3-174">応答</span><span class="sxs-lookup"><span data-stu-id="ca7f3-174">Response</span></span>
<span data-ttu-id="ca7f3-p110">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ca7f3-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




