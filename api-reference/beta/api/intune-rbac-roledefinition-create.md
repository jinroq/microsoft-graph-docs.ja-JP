---
title: roleDefinition の作成
description: 新しい roleDefinition オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8fa847f21b18fcdbb37429ff56a504d0b4e0caae
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33899467"
---
# <a name="create-roledefinition"></a><span data-ttu-id="91b7b-103">roleDefinition の作成</span><span class="sxs-lookup"><span data-stu-id="91b7b-103">Create roleDefinition</span></span>

> <span data-ttu-id="91b7b-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="91b7b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="91b7b-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="91b7b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="91b7b-106">新しい [roleDefinition](../resources/intune-rbac-roledefinition.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="91b7b-106">Create a new [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="91b7b-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="91b7b-107">Prerequisites</span></span>
<span data-ttu-id="91b7b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="91b7b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="91b7b-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="91b7b-110">Permission type</span></span>|<span data-ttu-id="91b7b-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="91b7b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="91b7b-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="91b7b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="91b7b-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91b7b-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="91b7b-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="91b7b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="91b7b-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="91b7b-115">Not supported.</span></span>|
|<span data-ttu-id="91b7b-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="91b7b-116">Application</span></span>|<span data-ttu-id="91b7b-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="91b7b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="91b7b-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="91b7b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="91b7b-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="91b7b-119">Request headers</span></span>
|<span data-ttu-id="91b7b-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="91b7b-120">Header</span></span>|<span data-ttu-id="91b7b-121">値</span><span class="sxs-lookup"><span data-stu-id="91b7b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="91b7b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="91b7b-122">Authorization</span></span>|<span data-ttu-id="91b7b-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="91b7b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="91b7b-124">承諾</span><span class="sxs-lookup"><span data-stu-id="91b7b-124">Accept</span></span>|<span data-ttu-id="91b7b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="91b7b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="91b7b-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="91b7b-126">Request body</span></span>
<span data-ttu-id="91b7b-127">要求本文で、roleDefinition オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="91b7b-127">In the request body, supply a JSON representation for the roleDefinition object.</span></span>

<span data-ttu-id="91b7b-128">次の表に、roleDefinition の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="91b7b-128">The following table shows the properties that are required when you create the roleDefinition.</span></span>

|<span data-ttu-id="91b7b-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="91b7b-129">Property</span></span>|<span data-ttu-id="91b7b-130">型</span><span class="sxs-lookup"><span data-stu-id="91b7b-130">Type</span></span>|<span data-ttu-id="91b7b-131">説明</span><span class="sxs-lookup"><span data-stu-id="91b7b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="91b7b-132">id</span><span class="sxs-lookup"><span data-stu-id="91b7b-132">id</span></span>|<span data-ttu-id="91b7b-133">文字列</span><span class="sxs-lookup"><span data-stu-id="91b7b-133">String</span></span>|<span data-ttu-id="91b7b-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="91b7b-134">Key of the entity.</span></span> <span data-ttu-id="91b7b-135">これは読み取り専用で、自動生成されます。</span><span class="sxs-lookup"><span data-stu-id="91b7b-135">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="91b7b-136">displayName</span><span class="sxs-lookup"><span data-stu-id="91b7b-136">displayName</span></span>|<span data-ttu-id="91b7b-137">String</span><span class="sxs-lookup"><span data-stu-id="91b7b-137">String</span></span>|<span data-ttu-id="91b7b-138">ロールの定義の表示名。</span><span class="sxs-lookup"><span data-stu-id="91b7b-138">Display Name of the Role definition.</span></span>|
|<span data-ttu-id="91b7b-139">description</span><span class="sxs-lookup"><span data-stu-id="91b7b-139">description</span></span>|<span data-ttu-id="91b7b-140">String</span><span class="sxs-lookup"><span data-stu-id="91b7b-140">String</span></span>|<span data-ttu-id="91b7b-141">ロールの定義の説明。</span><span class="sxs-lookup"><span data-stu-id="91b7b-141">Description of the Role definition.</span></span>|
|<span data-ttu-id="91b7b-142">アクセス許可</span><span class="sxs-lookup"><span data-stu-id="91b7b-142">permissions</span></span>|<span data-ttu-id="91b7b-143">[rolePermission](../resources/intune-rbac-rolepermission.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="91b7b-143">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="91b7b-144">このロールに実行が許可されている、ロールのアクセス許可のリスト。</span><span class="sxs-lookup"><span data-stu-id="91b7b-144">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="91b7b-145">これらは、rolePermission の一部として定義されている actionName と一致する必要があります。</span><span class="sxs-lookup"><span data-stu-id="91b7b-145">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="91b7b-146">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="91b7b-146">rolePermissions</span></span>|<span data-ttu-id="91b7b-147">[rolePermission](../resources/intune-rbac-rolepermission.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="91b7b-147">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="91b7b-148">このロールに実行が許可されている、ロールのアクセス許可のリスト。</span><span class="sxs-lookup"><span data-stu-id="91b7b-148">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="91b7b-149">これらは、rolePermission の一部として定義されている actionName と一致する必要があります。</span><span class="sxs-lookup"><span data-stu-id="91b7b-149">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="91b7b-150">isBuiltInRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="91b7b-150">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="91b7b-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="91b7b-151">Boolean</span></span>|<span data-ttu-id="91b7b-152">ロールの種類。</span><span class="sxs-lookup"><span data-stu-id="91b7b-152">Type of Role.</span></span> <span data-ttu-id="91b7b-153">組み込みの場合は True に設定し、カスタム ロールの定義の場合は False に設定します。</span><span class="sxs-lookup"><span data-stu-id="91b7b-153">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|
|<span data-ttu-id="91b7b-154">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="91b7b-154">isBuiltIn</span></span>|<span data-ttu-id="91b7b-155">Boolean</span><span class="sxs-lookup"><span data-stu-id="91b7b-155">Boolean</span></span>|<span data-ttu-id="91b7b-156">ロールの種類。</span><span class="sxs-lookup"><span data-stu-id="91b7b-156">Type of Role.</span></span> <span data-ttu-id="91b7b-157">組み込みの場合は True に設定し、カスタム ロールの定義の場合は False に設定します。</span><span class="sxs-lookup"><span data-stu-id="91b7b-157">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|
|<span data-ttu-id="91b7b-158">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="91b7b-158">roleScopeTagIds</span></span>|<span data-ttu-id="91b7b-159">String collection</span><span class="sxs-lookup"><span data-stu-id="91b7b-159">String collection</span></span>|<span data-ttu-id="91b7b-160">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="91b7b-160">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="91b7b-161">応答</span><span class="sxs-lookup"><span data-stu-id="91b7b-161">Response</span></span>
<span data-ttu-id="91b7b-162">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [roleDefinition](../resources/intune-rbac-roledefinition.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="91b7b-162">If successful, this method returns a `201 Created` response code and a [roleDefinition](../resources/intune-rbac-roledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="91b7b-163">例</span><span class="sxs-lookup"><span data-stu-id="91b7b-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="91b7b-164">要求</span><span class="sxs-lookup"><span data-stu-id="91b7b-164">Request</span></span>
<span data-ttu-id="91b7b-165">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="91b7b-165">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/roleDefinitions
Content-type: application/json
Content-length: 1207

{
  "@odata.type": "#microsoft.graph.roleDefinition",
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

### <a name="response"></a><span data-ttu-id="91b7b-166">応答</span><span class="sxs-lookup"><span data-stu-id="91b7b-166">Response</span></span>
<span data-ttu-id="91b7b-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="91b7b-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 1256

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
  "isBuiltIn": true,
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```




