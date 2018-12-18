---
title: deviceAndAppManagementRoleAssignment の更新
description: deviceAndAppManagementRoleAssignment オブジェクトのプロパティを更新します。
author: tfitzmac
ms.openlocfilehash: 79c7f35a52f7d0d853a77ec4186a957a287ec3ed
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27357254"
---
# <a name="update-deviceandappmanagementroleassignment"></a><span data-ttu-id="09211-103">deviceAndAppManagementRoleAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="09211-103">Update deviceAndAppManagementRoleAssignment</span></span>

> <span data-ttu-id="09211-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="09211-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="09211-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="09211-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="09211-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="09211-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="09211-107">[deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="09211-107">Update the properties of a [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="09211-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="09211-108">Prerequisites</span></span>
<span data-ttu-id="09211-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="09211-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="09211-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="09211-111">Permission type</span></span>|<span data-ttu-id="09211-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="09211-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="09211-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="09211-113">Delegated (work or school account)</span></span>|<span data-ttu-id="09211-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09211-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="09211-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="09211-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="09211-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="09211-116">Not supported.</span></span>|
|<span data-ttu-id="09211-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="09211-117">Application</span></span>|<span data-ttu-id="09211-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="09211-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="09211-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="09211-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleAssignments/{deviceAndAppManagementRoleAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="09211-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="09211-120">Request headers</span></span>
|<span data-ttu-id="09211-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="09211-121">Header</span></span>|<span data-ttu-id="09211-122">値</span><span class="sxs-lookup"><span data-stu-id="09211-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="09211-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="09211-123">Authorization</span></span>|<span data-ttu-id="09211-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="09211-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="09211-125">Accept</span><span class="sxs-lookup"><span data-stu-id="09211-125">Accept</span></span>|<span data-ttu-id="09211-126">application/json</span><span class="sxs-lookup"><span data-stu-id="09211-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="09211-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="09211-127">Request body</span></span>
<span data-ttu-id="09211-128">要求本文で、[deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="09211-128">In the request body, supply a JSON representation for the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>

<span data-ttu-id="09211-129">次の表に、[deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="09211-129">The following table shows the properties that are required when you create the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span></span>

|<span data-ttu-id="09211-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="09211-130">Property</span></span>|<span data-ttu-id="09211-131">種類</span><span class="sxs-lookup"><span data-stu-id="09211-131">Type</span></span>|<span data-ttu-id="09211-132">説明</span><span class="sxs-lookup"><span data-stu-id="09211-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="09211-133">ID</span><span class="sxs-lookup"><span data-stu-id="09211-133">id</span></span>|<span data-ttu-id="09211-134">String</span><span class="sxs-lookup"><span data-stu-id="09211-134">String</span></span>|<span data-ttu-id="09211-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="09211-135">Key of the entity.</span></span> <span data-ttu-id="09211-136">これは読み取り専用で、自動生成されます。</span><span class="sxs-lookup"><span data-stu-id="09211-136">This is read-only and automatically generated.</span></span> <span data-ttu-id="09211-137">[roleAssignment](../resources/intune-rbac-roleassignment.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="09211-137">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="09211-138">displayName</span><span class="sxs-lookup"><span data-stu-id="09211-138">displayName</span></span>|<span data-ttu-id="09211-139">String</span><span class="sxs-lookup"><span data-stu-id="09211-139">String</span></span>|<span data-ttu-id="09211-140">ロール割り当ての表示名またはフレンドリ名。</span><span class="sxs-lookup"><span data-stu-id="09211-140">The display or friendly name of the role Assignment.</span></span> <span data-ttu-id="09211-141">[roleAssignment](../resources/intune-rbac-roleassignment.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="09211-141">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="09211-142">説明</span><span class="sxs-lookup"><span data-stu-id="09211-142">description</span></span>|<span data-ttu-id="09211-143">String</span><span class="sxs-lookup"><span data-stu-id="09211-143">String</span></span>|<span data-ttu-id="09211-144">ロール割り当ての説明。</span><span class="sxs-lookup"><span data-stu-id="09211-144">Description of the Role Assignment.</span></span> <span data-ttu-id="09211-145">[roleAssignment](../resources/intune-rbac-roleassignment.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="09211-145">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="09211-146">scopeMembers</span><span class="sxs-lookup"><span data-stu-id="09211-146">scopeMembers</span></span>|<span data-ttu-id="09211-147">String コレクション</span><span class="sxs-lookup"><span data-stu-id="09211-147">String collection</span></span>|<span data-ttu-id="09211-148">役割のスコープ メンバーのセキュリティ グループの ID リスト。</span><span class="sxs-lookup"><span data-stu-id="09211-148">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="09211-149">Azure Active Directory の ID。</span><span class="sxs-lookup"><span data-stu-id="09211-149">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="09211-150">[roleAssignment](../resources/intune-rbac-roleassignment.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="09211-150">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="09211-151">scopeType</span><span class="sxs-lookup"><span data-stu-id="09211-151">scopeType</span></span>|[<span data-ttu-id="09211-152">roleAssignmentScopeType</span><span class="sxs-lookup"><span data-stu-id="09211-152">roleAssignmentScopeType</span></span>](../resources/intune-rbac-roleassignmentscopetype.md)|<span data-ttu-id="09211-153">役割の割り当てのスコープの種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="09211-153">Specifies the type of scope for a Role Assignment.</span></span> <span data-ttu-id="09211-154">'ResourceScope' の既定の種類は、ResourceScopes の割り当てを使用できます。</span><span class="sxs-lookup"><span data-stu-id="09211-154">Default type 'ResourceScope' allows assignment of ResourceScopes.</span></span> <span data-ttu-id="09211-155">'している'、'AllLicensedUsers'、および 'AllDevicesAndLicensedUsers' の ResourceScopes プロパティは空欄のままです。</span><span class="sxs-lookup"><span data-stu-id="09211-155">For 'AllDevices', 'AllLicensedUsers', and 'AllDevicesAndLicensedUsers', the ResourceScopes property should be left empty.</span></span> <span data-ttu-id="09211-156">[RoleAssignment](../resources/intune-rbac-roleassignment.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="09211-156">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span> <span data-ttu-id="09211-157">可能な値は、`resourceScope`、`allDevices`、`allLicensedUsers`、`allDevicesAndLicensedUsers` です。</span><span class="sxs-lookup"><span data-stu-id="09211-157">Possible values are: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span></span>|
|<span data-ttu-id="09211-158">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="09211-158">resourceScopes</span></span>|<span data-ttu-id="09211-159">String コレクション</span><span class="sxs-lookup"><span data-stu-id="09211-159">String collection</span></span>|<span data-ttu-id="09211-160">役割のスコープ メンバーのセキュリティ グループの ID リスト。</span><span class="sxs-lookup"><span data-stu-id="09211-160">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="09211-161">Azure Active Directory の ID。</span><span class="sxs-lookup"><span data-stu-id="09211-161">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="09211-162">[roleAssignment](../resources/intune-rbac-roleassignment.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="09211-162">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="09211-163">members</span><span class="sxs-lookup"><span data-stu-id="09211-163">members</span></span>|<span data-ttu-id="09211-164">String コレクション</span><span class="sxs-lookup"><span data-stu-id="09211-164">String collection</span></span>|<span data-ttu-id="09211-165">ロール メンバーのセキュリティ グループの ID リスト。</span><span class="sxs-lookup"><span data-stu-id="09211-165">The list of ids of role member security groups.</span></span> <span data-ttu-id="09211-166">Azure Active Directory の ID。</span><span class="sxs-lookup"><span data-stu-id="09211-166">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="09211-167">応答</span><span class="sxs-lookup"><span data-stu-id="09211-167">Response</span></span>
<span data-ttu-id="09211-168">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で、更新された [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="09211-168">If successful, this method returns a `200 OK` response code and an updated [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="09211-169">例</span><span class="sxs-lookup"><span data-stu-id="09211-169">Example</span></span>
### <a name="request"></a><span data-ttu-id="09211-170">要求</span><span class="sxs-lookup"><span data-stu-id="09211-170">Request</span></span>
<span data-ttu-id="09211-171">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="09211-171">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/roleAssignments/{deviceAndAppManagementRoleAssignmentId}
Content-type: application/json
Content-length: 267

{
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

### <a name="response"></a><span data-ttu-id="09211-172">応答</span><span class="sxs-lookup"><span data-stu-id="09211-172">Response</span></span>
<span data-ttu-id="09211-p110">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="09211-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





