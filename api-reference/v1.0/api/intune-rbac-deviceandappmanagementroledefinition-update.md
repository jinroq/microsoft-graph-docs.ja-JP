---
title: deviceAndAppManagementRoleDefinition の更新
description: deviceAndAppManagementRoleDefinition オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dfcc2f315f528588739a780ea7f70b0207cab67d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32467303"
---
# <a name="update-deviceandappmanagementroledefinition"></a><span data-ttu-id="8587f-103">deviceAndAppManagementRoleDefinition の更新</span><span class="sxs-lookup"><span data-stu-id="8587f-103">Update deviceAndAppManagementRoleDefinition</span></span>

> <span data-ttu-id="8587f-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8587f-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8587f-105">[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="8587f-105">Update the properties of a [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8587f-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="8587f-106">Prerequisites</span></span>
<span data-ttu-id="8587f-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8587f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8587f-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8587f-109">Permission type</span></span>|<span data-ttu-id="8587f-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="8587f-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8587f-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8587f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8587f-112">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8587f-112">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="8587f-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8587f-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8587f-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8587f-114">Not supported.</span></span>|
|<span data-ttu-id="8587f-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8587f-115">Application</span></span>|<span data-ttu-id="8587f-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8587f-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8587f-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8587f-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/roleDefinition
```

## <a name="request-headers"></a><span data-ttu-id="8587f-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8587f-118">Request headers</span></span>
|<span data-ttu-id="8587f-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8587f-119">Header</span></span>|<span data-ttu-id="8587f-120">値</span><span class="sxs-lookup"><span data-stu-id="8587f-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8587f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="8587f-121">Authorization</span></span>|<span data-ttu-id="8587f-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="8587f-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8587f-123">承諾</span><span class="sxs-lookup"><span data-stu-id="8587f-123">Accept</span></span>|<span data-ttu-id="8587f-124">application/json</span><span class="sxs-lookup"><span data-stu-id="8587f-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8587f-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="8587f-125">Request body</span></span>
<span data-ttu-id="8587f-126">要求本文で、[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="8587f-126">In the request body, supply a JSON representation for the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>

<span data-ttu-id="8587f-127">次の表に、[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="8587f-127">The following table shows the properties that are required when you create the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md).</span></span>

|<span data-ttu-id="8587f-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8587f-128">Property</span></span>|<span data-ttu-id="8587f-129">型</span><span class="sxs-lookup"><span data-stu-id="8587f-129">Type</span></span>|<span data-ttu-id="8587f-130">説明</span><span class="sxs-lookup"><span data-stu-id="8587f-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8587f-131">id</span><span class="sxs-lookup"><span data-stu-id="8587f-131">id</span></span>|<span data-ttu-id="8587f-132">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="8587f-132">String</span></span>|<span data-ttu-id="8587f-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="8587f-133">Key of the entity.</span></span> <span data-ttu-id="8587f-134">これは読み取り専用で、自動生成されます。</span><span class="sxs-lookup"><span data-stu-id="8587f-134">This is read-only and automatically generated.</span></span> <span data-ttu-id="8587f-135">[roleDefinition](../resources/intune-rbac-roledefinition.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8587f-135">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="8587f-136">displayName</span><span class="sxs-lookup"><span data-stu-id="8587f-136">displayName</span></span>|<span data-ttu-id="8587f-137">String</span><span class="sxs-lookup"><span data-stu-id="8587f-137">String</span></span>|<span data-ttu-id="8587f-138">ロールの定義の表示名。</span><span class="sxs-lookup"><span data-stu-id="8587f-138">Display Name of the Role definition.</span></span> <span data-ttu-id="8587f-139">[roleDefinition](../resources/intune-rbac-roledefinition.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8587f-139">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="8587f-140">説明</span><span class="sxs-lookup"><span data-stu-id="8587f-140">description</span></span>|<span data-ttu-id="8587f-141">String</span><span class="sxs-lookup"><span data-stu-id="8587f-141">String</span></span>|<span data-ttu-id="8587f-142">ロールの定義の説明。</span><span class="sxs-lookup"><span data-stu-id="8587f-142">Description of the Role definition.</span></span> <span data-ttu-id="8587f-143">[roleDefinition](../resources/intune-rbac-roledefinition.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8587f-143">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="8587f-144">rolePermissions</span><span class="sxs-lookup"><span data-stu-id="8587f-144">rolePermissions</span></span>|<span data-ttu-id="8587f-145">[rolePermission](../resources/intune-rbac-rolepermission.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="8587f-145">[rolePermission](../resources/intune-rbac-rolepermission.md) collection</span></span>|<span data-ttu-id="8587f-146">このロールに実行が許可されている、ロールのアクセス許可のリスト。</span><span class="sxs-lookup"><span data-stu-id="8587f-146">List of Role Permissions this role is allowed to perform.</span></span> <span data-ttu-id="8587f-147">これらは、rolePermission の一部として定義されている actionName と一致する必要があります。</span><span class="sxs-lookup"><span data-stu-id="8587f-147">These must match the actionName that is defined as part of the rolePermission.</span></span> <span data-ttu-id="8587f-148">[roleDefinition](../resources/intune-rbac-roledefinition.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8587f-148">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|
|<span data-ttu-id="8587f-149">isBuiltIn</span><span class="sxs-lookup"><span data-stu-id="8587f-149">isBuiltIn</span></span>|<span data-ttu-id="8587f-150">Boolean</span><span class="sxs-lookup"><span data-stu-id="8587f-150">Boolean</span></span>|<span data-ttu-id="8587f-151">ロールの種類。</span><span class="sxs-lookup"><span data-stu-id="8587f-151">Type of Role.</span></span> <span data-ttu-id="8587f-152">組み込みの場合は True に設定し、カスタム ロールの定義の場合は False に設定します。</span><span class="sxs-lookup"><span data-stu-id="8587f-152">Set to True if it is built-in, or set to False if it is a custom role definition.</span></span> <span data-ttu-id="8587f-153">[roleDefinition](../resources/intune-rbac-roledefinition.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="8587f-153">Inherited from [roleDefinition](../resources/intune-rbac-roledefinition.md)</span></span>|



## <a name="response"></a><span data-ttu-id="8587f-154">応答</span><span class="sxs-lookup"><span data-stu-id="8587f-154">Response</span></span>
<span data-ttu-id="8587f-155">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="8587f-155">If successful, this method returns a `200 OK` response code and an updated [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8587f-156">例</span><span class="sxs-lookup"><span data-stu-id="8587f-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="8587f-157">要求</span><span class="sxs-lookup"><span data-stu-id="8587f-157">Request</span></span>
<span data-ttu-id="8587f-158">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8587f-158">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/roleDefinitions/{roleDefinitionId}
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

### <a name="response"></a><span data-ttu-id="8587f-159">応答</span><span class="sxs-lookup"><span data-stu-id="8587f-159">Response</span></span>
<span data-ttu-id="8587f-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8587f-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



