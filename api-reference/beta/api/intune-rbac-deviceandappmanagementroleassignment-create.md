---
title: deviceAndAppManagementRoleAssignment の作成
description: 新しい deviceAndAppManagementRoleAssignment オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 69366bedb13018139c3bd8838009d6d410a7f773
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35984203"
---
# <a name="create-deviceandappmanagementroleassignment"></a><span data-ttu-id="0dff4-103">deviceAndAppManagementRoleAssignment の作成</span><span class="sxs-lookup"><span data-stu-id="0dff4-103">Create deviceAndAppManagementRoleAssignment</span></span>

> <span data-ttu-id="0dff4-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0dff4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0dff4-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0dff4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0dff4-106">新しい [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="0dff4-106">Create a new [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0dff4-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="0dff4-107">Prerequisites</span></span>
<span data-ttu-id="0dff4-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0dff4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0dff4-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0dff4-110">Permission type</span></span>|<span data-ttu-id="0dff4-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="0dff4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0dff4-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0dff4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0dff4-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0dff4-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="0dff4-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0dff4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0dff4-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0dff4-115">Not supported.</span></span>|
|<span data-ttu-id="0dff4-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0dff4-116">Application</span></span>|<span data-ttu-id="0dff4-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0dff4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0dff4-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0dff4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="0dff4-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0dff4-119">Request headers</span></span>
|<span data-ttu-id="0dff4-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0dff4-120">Header</span></span>|<span data-ttu-id="0dff4-121">値</span><span class="sxs-lookup"><span data-stu-id="0dff4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0dff4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0dff4-122">Authorization</span></span>|<span data-ttu-id="0dff4-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="0dff4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0dff4-124">承諾</span><span class="sxs-lookup"><span data-stu-id="0dff4-124">Accept</span></span>|<span data-ttu-id="0dff4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0dff4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0dff4-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="0dff4-126">Request body</span></span>
<span data-ttu-id="0dff4-127">要求本文で、deviceAndAppManagementRoleAssignment オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="0dff4-127">In the request body, supply a JSON representation for the deviceAndAppManagementRoleAssignment object.</span></span>

<span data-ttu-id="0dff4-128">次の表に、deviceAndAppManagementRoleAssignment の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="0dff4-128">The following table shows the properties that are required when you create the deviceAndAppManagementRoleAssignment.</span></span>

|<span data-ttu-id="0dff4-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0dff4-129">Property</span></span>|<span data-ttu-id="0dff4-130">型</span><span class="sxs-lookup"><span data-stu-id="0dff4-130">Type</span></span>|<span data-ttu-id="0dff4-131">説明</span><span class="sxs-lookup"><span data-stu-id="0dff4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0dff4-132">id</span><span class="sxs-lookup"><span data-stu-id="0dff4-132">id</span></span>|<span data-ttu-id="0dff4-133">文字列</span><span class="sxs-lookup"><span data-stu-id="0dff4-133">String</span></span>|<span data-ttu-id="0dff4-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="0dff4-134">Key of the entity.</span></span> <span data-ttu-id="0dff4-135">これは読み取り専用で、自動生成されます。</span><span class="sxs-lookup"><span data-stu-id="0dff4-135">This is read-only and automatically generated.</span></span> <span data-ttu-id="0dff4-136">[roleAssignment](../resources/intune-rbac-roleassignment.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0dff4-136">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="0dff4-137">displayName</span><span class="sxs-lookup"><span data-stu-id="0dff4-137">displayName</span></span>|<span data-ttu-id="0dff4-138">String</span><span class="sxs-lookup"><span data-stu-id="0dff4-138">String</span></span>|<span data-ttu-id="0dff4-139">ロール割り当ての表示名またはフレンドリ名。</span><span class="sxs-lookup"><span data-stu-id="0dff4-139">The display or friendly name of the role Assignment.</span></span> <span data-ttu-id="0dff4-140">[roleAssignment](../resources/intune-rbac-roleassignment.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0dff4-140">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="0dff4-141">description</span><span class="sxs-lookup"><span data-stu-id="0dff4-141">description</span></span>|<span data-ttu-id="0dff4-142">String</span><span class="sxs-lookup"><span data-stu-id="0dff4-142">String</span></span>|<span data-ttu-id="0dff4-143">ロール割り当ての説明。</span><span class="sxs-lookup"><span data-stu-id="0dff4-143">Description of the Role Assignment.</span></span> <span data-ttu-id="0dff4-144">[roleAssignment](../resources/intune-rbac-roleassignment.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0dff4-144">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="0dff4-145">scopeMembers</span><span class="sxs-lookup"><span data-stu-id="0dff4-145">scopeMembers</span></span>|<span data-ttu-id="0dff4-146">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="0dff4-146">String collection</span></span>|<span data-ttu-id="0dff4-147">役割のスコープ メンバーのセキュリティ グループの ID リスト。</span><span class="sxs-lookup"><span data-stu-id="0dff4-147">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="0dff4-148">Azure Active Directory の ID です。</span><span class="sxs-lookup"><span data-stu-id="0dff4-148">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="0dff4-149">[roleAssignment](../resources/intune-rbac-roleassignment.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0dff4-149">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="0dff4-150">scopeType</span><span class="sxs-lookup"><span data-stu-id="0dff4-150">scopeType</span></span>|[<span data-ttu-id="0dff4-151">roleAssignmentScopeType</span><span class="sxs-lookup"><span data-stu-id="0dff4-151">roleAssignmentScopeType</span></span>](../resources/intune-rbac-roleassignmentscopetype.md)|<span data-ttu-id="0dff4-152">役割の割り当てのスコープの種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="0dff4-152">Specifies the type of scope for a Role Assignment.</span></span> <span data-ttu-id="0dff4-153">既定の種類 ' ResourceScope ' では、を割り当てることができます。</span><span class="sxs-lookup"><span data-stu-id="0dff4-153">Default type 'ResourceScope' allows assignment of ResourceScopes.</span></span> <span data-ttu-id="0dff4-154">' AllDevices '、' AllLicensedUsers '、および ' AllDevicesAndLicensedUsers ' の場合、ResourceScopes プロパティは空のままにする必要があります。</span><span class="sxs-lookup"><span data-stu-id="0dff4-154">For 'AllDevices', 'AllLicensedUsers', and 'AllDevicesAndLicensedUsers', the ResourceScopes property should be left empty.</span></span> <span data-ttu-id="0dff4-155">[Roleassignment](../resources/intune-rbac-roleassignment.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="0dff4-155">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span> <span data-ttu-id="0dff4-156">使用可能な値は、`resourceScope`、`allDevices`、`allLicensedUsers`、`allDevicesAndLicensedUsers` です。</span><span class="sxs-lookup"><span data-stu-id="0dff4-156">Possible values are: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span></span>|
|<span data-ttu-id="0dff4-157">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="0dff4-157">resourceScopes</span></span>|<span data-ttu-id="0dff4-158">文字列コレクション</span><span class="sxs-lookup"><span data-stu-id="0dff4-158">String collection</span></span>|<span data-ttu-id="0dff4-159">役割のスコープ メンバーのセキュリティ グループの ID リスト。</span><span class="sxs-lookup"><span data-stu-id="0dff4-159">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="0dff4-160">Azure Active Directory の ID です。</span><span class="sxs-lookup"><span data-stu-id="0dff4-160">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="0dff4-161">[roleAssignment](../resources/intune-rbac-roleassignment.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0dff4-161">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="0dff4-162">members</span><span class="sxs-lookup"><span data-stu-id="0dff4-162">members</span></span>|<span data-ttu-id="0dff4-163">String コレクション</span><span class="sxs-lookup"><span data-stu-id="0dff4-163">String collection</span></span>|<span data-ttu-id="0dff4-164">ロール メンバーのセキュリティ グループの ID リスト。</span><span class="sxs-lookup"><span data-stu-id="0dff4-164">The list of ids of role member security groups.</span></span> <span data-ttu-id="0dff4-165">Azure Active Directory の ID。</span><span class="sxs-lookup"><span data-stu-id="0dff4-165">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="0dff4-166">応答</span><span class="sxs-lookup"><span data-stu-id="0dff4-166">Response</span></span>
<span data-ttu-id="0dff4-167">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="0dff4-167">If successful, this method returns a `201 Created` response code and a [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0dff4-168">例</span><span class="sxs-lookup"><span data-stu-id="0dff4-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="0dff4-169">要求</span><span class="sxs-lookup"><span data-stu-id="0dff4-169">Request</span></span>
<span data-ttu-id="0dff4-170">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0dff4-170">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/roleAssignments
Content-type: application/json
Content-length: 342

{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleAssignment",
  "displayName": "Display Name value",
  "description": "Description value",
  "scopeMembers": [
    "Scope Members value"
  ],
  "scopeType": "allDevices",
  "resourceScopes": [
    "Resource Scopes value"
  ],
  "members": [
    "Members value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="0dff4-171">応答</span><span class="sxs-lookup"><span data-stu-id="0dff4-171">Response</span></span>
<span data-ttu-id="0dff4-p109">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0dff4-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 391

{
  "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleAssignment",
  "id": "a12e8ebb-8ebb-a12e-bb8e-2ea1bb8e2ea1",
  "displayName": "Display Name value",
  "description": "Description value",
  "scopeMembers": [
    "Scope Members value"
  ],
  "scopeType": "allDevices",
  "resourceScopes": [
    "Resource Scopes value"
  ],
  "members": [
    "Members value"
  ]
}
```





