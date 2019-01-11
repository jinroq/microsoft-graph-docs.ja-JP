---
title: roleDefinition の作成
description: 新しい roleDefinition オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: cb1e4b80388ecb74a4bd521e4b910a24ffb22af6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27858983"
---
# <a name="create-roledefinition"></a><span data-ttu-id="e3ae9-103">roleDefinition の作成</span><span class="sxs-lookup"><span data-stu-id="e3ae9-103">Create roleDefinition</span></span>

> <span data-ttu-id="e3ae9-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e3ae9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e3ae9-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e3ae9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e3ae9-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e3ae9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e3ae9-107">新しい [roleDefinition](../resources/intune-rbac-roledefinition.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="e3ae9-107">Create a new [roleDefinition](../resources/intune-rbac-roledefinition.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e3ae9-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="e3ae9-108">Prerequisites</span></span>
<span data-ttu-id="e3ae9-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e3ae9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e3ae9-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e3ae9-111">Permission type</span></span>|<span data-ttu-id="e3ae9-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="e3ae9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e3ae9-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e3ae9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e3ae9-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3ae9-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="e3ae9-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e3ae9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e3ae9-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e3ae9-116">Not supported.</span></span>|
|<span data-ttu-id="e3ae9-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e3ae9-117">Application</span></span>|<span data-ttu-id="e3ae9-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e3ae9-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e3ae9-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e3ae9-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="e3ae9-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e3ae9-120">Request headers</span></span>
|<span data-ttu-id="e3ae9-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e3ae9-121">Header</span></span>|<span data-ttu-id="e3ae9-122">値</span><span class="sxs-lookup"><span data-stu-id="e3ae9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e3ae9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e3ae9-123">Authorization</span></span>|<span data-ttu-id="e3ae9-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="e3ae9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e3ae9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e3ae9-125">Accept</span></span>|<span data-ttu-id="e3ae9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e3ae9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e3ae9-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="e3ae9-127">Request body</span></span>
<span data-ttu-id="e3ae9-128">要求本文で、roleDefinition オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="e3ae9-128">In the request body, supply a JSON representation for the roleDefinition object.</span></span>

<span data-ttu-id="e3ae9-129">次の表に、roleDefinition の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="e3ae9-129">The following table shows the properties that are required when you create the roleDefinition.</span></span>

|<span data-ttu-id="e3ae9-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e3ae9-130">Property</span></span>|<span data-ttu-id="e3ae9-131">種類</span><span class="sxs-lookup"><span data-stu-id="e3ae9-131">Type</span></span>|<span data-ttu-id="e3ae9-132">説明</span><span class="sxs-lookup"><span data-stu-id="e3ae9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3ae9-133">ID</span><span class="sxs-lookup"><span data-stu-id="e3ae9-133">id</span></span>|<span data-ttu-id="e3ae9-134">String</span><span class="sxs-lookup"><span data-stu-id="e3ae9-134">String</span></span>|<span data-ttu-id="e3ae9-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="e3ae9-135">Key of the entity.</span></span> <span data-ttu-id="e3ae9-136">これは読み取り専用で、自動生成されます。</span><span class="sxs-lookup"><span data-stu-id="e3ae9-136">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="e3ae9-137">displayName</span><span class="sxs-lookup"><span data-stu-id="e3ae9-137">displayName</span></span>|<span data-ttu-id="e3ae9-138">String</span><span class="sxs-lookup"><span data-stu-id="e3ae9-138">String</span></span>|<span data-ttu-id="e3ae9-139">ロールの定義の表示名。</span><span class="sxs-lookup"><span data-stu-id="e3ae9-139">Display Name of the Role definition.</span></span>|
|<span data-ttu-id="e3ae9-140">説明</span><span class="sxs-lookup"><span data-stu-id="e3ae9-140">description</span></span>|<span data-ttu-id="e3ae9-141">String</span><span class="sxs-lookup"><span data-stu-id="e3ae9-141">String</span></span>|<span data-ttu-id="e3ae9-142">ロールの定義の説明。</span><span class="sxs-lookup"><span data-stu-id="e3ae9-142">Description of the Role definition.</span></span>|
|<span data-ttu-id="e3ae9-143">permissions</span><span class="sxs-lookup"><span data-stu-id="e3ae9-143">permissions</span></span>|<span data-ttu-id="e3ae9-144">[rolePermission](../resources/intune-rbac-rolepermission.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e3ae9-144">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="e3ae9-145">このロールに実行が許可されている、ロールのアクセス許可のリスト。</span><span class="sxs-lookup"><span data-stu-id="e3ae9-145">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="e3ae9-146">これらは、rolePermission の一部として定義されている actionName と一致する必要があります。</span><span class="sxs-lookup"><span data-stu-id="e3ae9-146">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="e3ae9-147">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="e3ae9-147">rolePermissions</span></span>|<span data-ttu-id="e3ae9-148">[rolePermission](../resources/intune-rbac-rolepermission.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e3ae9-148">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="e3ae9-149">このロールに実行が許可されている、ロールのアクセス許可のリスト。</span><span class="sxs-lookup"><span data-stu-id="e3ae9-149">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="e3ae9-150">これらは、rolePermission の一部として定義されている actionName と一致する必要があります。</span><span class="sxs-lookup"><span data-stu-id="e3ae9-150">These must match the actionName that is defined as part of the rolePermission.</span></span>|
|<span data-ttu-id="e3ae9-151">isBuiltInRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="e3ae9-151">isBuiltInRoleDefinition</span></span>|<span data-ttu-id="e3ae9-152">Boolean</span><span class="sxs-lookup"><span data-stu-id="e3ae9-152">Boolean</span></span>|<span data-ttu-id="e3ae9-153">ロールの種類。</span><span class="sxs-lookup"><span data-stu-id="e3ae9-153">Type of Role.</span></span> <span data-ttu-id="e3ae9-154">組み込みの場合は True に設定し、カスタム ロールの定義の場合は False に設定します。</span><span class="sxs-lookup"><span data-stu-id="e3ae9-154">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|
|<span data-ttu-id="e3ae9-155">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="e3ae9-155">isBuiltIn</span></span>|<span data-ttu-id="e3ae9-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="e3ae9-156">Boolean</span></span>|<span data-ttu-id="e3ae9-157">ロールの種類。</span><span class="sxs-lookup"><span data-stu-id="e3ae9-157">Type of Role.</span></span> <span data-ttu-id="e3ae9-158">組み込みの場合は True に設定し、カスタム ロールの定義の場合は False に設定します。</span><span class="sxs-lookup"><span data-stu-id="e3ae9-158">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span>|



## <a name="response"></a><span data-ttu-id="e3ae9-159">応答</span><span class="sxs-lookup"><span data-stu-id="e3ae9-159">Response</span></span>
<span data-ttu-id="e3ae9-160">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [roleDefinition](../resources/intune-rbac-roledefinition.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e3ae9-160">If successful, this method returns a `201 Created` response code and a [roleDefinition](../resources/intune-rbac-roledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e3ae9-161">例</span><span class="sxs-lookup"><span data-stu-id="e3ae9-161">Example</span></span>
### <a name="request"></a><span data-ttu-id="e3ae9-162">要求</span><span class="sxs-lookup"><span data-stu-id="e3ae9-162">Request</span></span>
<span data-ttu-id="e3ae9-163">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e3ae9-163">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/roleDefinitions
Content-type: application/json
Content-length: 1145

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
  "isBuiltIn": true
}
```

### <a name="response"></a><span data-ttu-id="e3ae9-164">応答</span><span class="sxs-lookup"><span data-stu-id="e3ae9-164">Response</span></span>
<span data-ttu-id="e3ae9-p108">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e3ae9-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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





