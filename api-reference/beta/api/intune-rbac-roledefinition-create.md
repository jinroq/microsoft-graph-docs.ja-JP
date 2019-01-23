---
title: roleDefinition の作成
description: 新しい roleDefinition オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a274621d13246cbbbe7071353fa7126ea3568d47
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29412661"
---
# <a name="create-roledefinition"></a><span data-ttu-id="a175d-103">roleDefinition の作成</span><span class="sxs-lookup"><span data-stu-id="a175d-103">Create roleDefinition</span></span>

> <span data-ttu-id="a175d-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a175d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a175d-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a175d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a175d-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a175d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a175d-107">新しい [roleDefinition](../resources/intune-rbac-roledefinition.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="a175d-107">Create a new [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a175d-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="a175d-108">Prerequisites</span></span>
<span data-ttu-id="a175d-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a175d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a175d-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a175d-111">Permission type</span></span>|<span data-ttu-id="a175d-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a175d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a175d-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a175d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a175d-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a175d-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="a175d-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a175d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a175d-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a175d-116">Not supported.</span></span>|
|<span data-ttu-id="a175d-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a175d-117">Application</span></span>|<span data-ttu-id="a175d-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a175d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a175d-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a175d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="a175d-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a175d-120">Request headers</span></span>
|<span data-ttu-id="a175d-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a175d-121">Header</span></span>|<span data-ttu-id="a175d-122">値</span><span class="sxs-lookup"><span data-stu-id="a175d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a175d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a175d-123">Authorization</span></span>|<span data-ttu-id="a175d-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="a175d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a175d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a175d-125">Accept</span></span>|<span data-ttu-id="a175d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a175d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a175d-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="a175d-127">Request body</span></span>
<span data-ttu-id="a175d-128">要求本文で、roleDefinition オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="a175d-128">In the request body, supply a JSON representation for the roleDefinition object.</span></span>

<span data-ttu-id="a175d-129">次の表に、roleDefinition の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="a175d-129">The following table shows the properties that are required when you create the roleDefinition.</span></span>

|<span data-ttu-id="a175d-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a175d-130">Property</span></span>|<span data-ttu-id="a175d-131">型</span><span class="sxs-lookup"><span data-stu-id="a175d-131">Type</span></span>|<span data-ttu-id="a175d-132">説明</span><span class="sxs-lookup"><span data-stu-id="a175d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a175d-133">id</span><span class="sxs-lookup"><span data-stu-id="a175d-133">id</span></span>|<span data-ttu-id="a175d-134">String</span><span class="sxs-lookup"><span data-stu-id="a175d-134">String</span></span>|<span data-ttu-id="a175d-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="a175d-135">Key of the entity.</span></span> <span data-ttu-id="a175d-136">これは読み取り専用で、自動生成されます。</span><span class="sxs-lookup"><span data-stu-id="a175d-136">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="a175d-137">displayName</span><span class="sxs-lookup"><span data-stu-id="a175d-137">displayName</span></span>|<span data-ttu-id="a175d-138">String</span><span class="sxs-lookup"><span data-stu-id="a175d-138">String</span></span>|<span data-ttu-id="a175d-139">ロールの定義の表示名。</span><span class="sxs-lookup"><span data-stu-id="a175d-139">Display Name of the Role definition.</span></span>|
|<span data-ttu-id="a175d-140">説明</span><span class="sxs-lookup"><span data-stu-id="a175d-140">description</span></span>|<span data-ttu-id="a175d-141">String</span><span class="sxs-lookup"><span data-stu-id="a175d-141">String</span></span>|<span data-ttu-id="a175d-142">ロールの定義の説明。</span><span class="sxs-lookup"><span data-stu-id="a175d-142">Description of the Role definition.</span></span>|
|<span data-ttu-id="a175d-143">permissions</span><span class="sxs-lookup"><span data-stu-id="a175d-143">permissions</span></span>|<span data-ttu-id="a175d-144">[rolePermission](../resources/intune-rbac-rolepermission.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a175d-144">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="a175d-145">このロールに実行が許可されている、ロールのアクセス許可のリスト。</span><span class="sxs-lookup"><span data-stu-id="a175d-145">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="a175d-146">これらは、rolePermission の一部として定義されている actionName と一致する必要があります。</span><span class="sxs-lookup"><span data-stu-id="a175d-146">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="a175d-147">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="a175d-147">rolePermissions</span></span>|<span data-ttu-id="a175d-148">[rolePermission](../resources/intune-rbac-rolepermission.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="a175d-148">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="a175d-149">このロールに実行が許可されている、ロールのアクセス許可のリスト。</span><span class="sxs-lookup"><span data-stu-id="a175d-149">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="a175d-150">これらは、rolePermission の一部として定義されている actionName と一致する必要があります。</span><span class="sxs-lookup"><span data-stu-id="a175d-150">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="a175d-151">isBuiltInRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="a175d-151">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="a175d-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="a175d-152">Boolean</span></span>|<span data-ttu-id="a175d-153">ロールの種類。</span><span class="sxs-lookup"><span data-stu-id="a175d-153">Type of Role.</span></span> <span data-ttu-id="a175d-154">組み込みの場合は True に設定し、カスタム ロールの定義の場合は False に設定します。</span><span class="sxs-lookup"><span data-stu-id="a175d-154">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|
|<span data-ttu-id="a175d-155">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="a175d-155">isBuiltIn</span></span>|<span data-ttu-id="a175d-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="a175d-156">Boolean</span></span>|<span data-ttu-id="a175d-157">ロールの種類。</span><span class="sxs-lookup"><span data-stu-id="a175d-157">Type of Role.</span></span> <span data-ttu-id="a175d-158">組み込みの場合は True に設定し、カスタム ロールの定義の場合は False に設定します。</span><span class="sxs-lookup"><span data-stu-id="a175d-158">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|
|<span data-ttu-id="a175d-159">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="a175d-159">roleScopeTagIds</span></span>|<span data-ttu-id="a175d-160">String コレクション</span><span class="sxs-lookup"><span data-stu-id="a175d-160">String collection</span></span>|<span data-ttu-id="a175d-161">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="a175d-161">List of Scope Tags for this Entity instance.</span></span>|



## <a name="response"></a><span data-ttu-id="a175d-162">応答</span><span class="sxs-lookup"><span data-stu-id="a175d-162">Response</span></span>
<span data-ttu-id="a175d-163">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [roleDefinition](../resources/intune-rbac-roledefinition.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a175d-163">If successful, this method returns a `201 Created` response code and a [roleDefinition](../resources/intune-rbac-roledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a175d-164">例</span><span class="sxs-lookup"><span data-stu-id="a175d-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="a175d-165">要求</span><span class="sxs-lookup"><span data-stu-id="a175d-165">Request</span></span>
<span data-ttu-id="a175d-166">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a175d-166">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a175d-167">応答</span><span class="sxs-lookup"><span data-stu-id="a175d-167">Response</span></span>
<span data-ttu-id="a175d-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a175d-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




