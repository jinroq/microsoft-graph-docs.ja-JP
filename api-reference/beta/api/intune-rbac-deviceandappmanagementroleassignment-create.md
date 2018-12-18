---
title: deviceAndAppManagementRoleAssignment の作成
description: 新しい deviceAndAppManagementRoleAssignment オブジェクトを作成します。
author: tfitzmac
ms.openlocfilehash: 4ed81fdc58a2675be6d5f0b991507914d5c92e89
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27323990"
---
# <a name="create-deviceandappmanagementroleassignment"></a><span data-ttu-id="0c842-103">deviceAndAppManagementRoleAssignment の作成</span><span class="sxs-lookup"><span data-stu-id="0c842-103">Create deviceAndAppManagementRoleAssignment</span></span>

> <span data-ttu-id="0c842-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0c842-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0c842-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0c842-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0c842-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="0c842-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0c842-107">新しい [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="0c842-107">Create a new [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0c842-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="0c842-108">Prerequisites</span></span>
<span data-ttu-id="0c842-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0c842-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c842-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0c842-111">Permission type</span></span>|<span data-ttu-id="0c842-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="0c842-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0c842-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0c842-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0c842-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c842-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="0c842-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0c842-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0c842-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0c842-116">Not supported.</span></span>|
|<span data-ttu-id="0c842-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0c842-117">Application</span></span>|<span data-ttu-id="0c842-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0c842-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0c842-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0c842-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="0c842-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0c842-120">Request headers</span></span>
|<span data-ttu-id="0c842-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0c842-121">Header</span></span>|<span data-ttu-id="0c842-122">値</span><span class="sxs-lookup"><span data-stu-id="0c842-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0c842-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0c842-123">Authorization</span></span>|<span data-ttu-id="0c842-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="0c842-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0c842-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0c842-125">Accept</span></span>|<span data-ttu-id="0c842-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0c842-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0c842-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="0c842-127">Request body</span></span>
<span data-ttu-id="0c842-128">要求本文で、deviceAndAppManagementRoleAssignment オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="0c842-128">In the request body, supply a JSON representation for the deviceAndAppManagementRoleAssignment object.</span></span>

<span data-ttu-id="0c842-129">次の表に、deviceAndAppManagementRoleAssignment の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="0c842-129">The following table shows the properties that are required when you create the deviceAndAppManagementRoleAssignment.</span></span>

|<span data-ttu-id="0c842-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="0c842-130">Property</span></span>|<span data-ttu-id="0c842-131">種類</span><span class="sxs-lookup"><span data-stu-id="0c842-131">Type</span></span>|<span data-ttu-id="0c842-132">説明</span><span class="sxs-lookup"><span data-stu-id="0c842-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c842-133">ID</span><span class="sxs-lookup"><span data-stu-id="0c842-133">id</span></span>|<span data-ttu-id="0c842-134">String</span><span class="sxs-lookup"><span data-stu-id="0c842-134">String</span></span>|<span data-ttu-id="0c842-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="0c842-135">Key of the entity.</span></span> <span data-ttu-id="0c842-136">これは読み取り専用で、自動生成されます。</span><span class="sxs-lookup"><span data-stu-id="0c842-136">This is read-only and automatically generated.</span></span> <span data-ttu-id="0c842-137">[roleAssignment](../resources/intune-rbac-roleassignment.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0c842-137">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="0c842-138">displayName</span><span class="sxs-lookup"><span data-stu-id="0c842-138">displayName</span></span>|<span data-ttu-id="0c842-139">String</span><span class="sxs-lookup"><span data-stu-id="0c842-139">String</span></span>|<span data-ttu-id="0c842-140">ロール割り当ての表示名またはフレンドリ名。</span><span class="sxs-lookup"><span data-stu-id="0c842-140">The display or friendly name of the role Assignment.</span></span> <span data-ttu-id="0c842-141">[roleAssignment](../resources/intune-rbac-roleassignment.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0c842-141">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="0c842-142">説明</span><span class="sxs-lookup"><span data-stu-id="0c842-142">description</span></span>|<span data-ttu-id="0c842-143">String</span><span class="sxs-lookup"><span data-stu-id="0c842-143">String</span></span>|<span data-ttu-id="0c842-144">ロール割り当ての説明。</span><span class="sxs-lookup"><span data-stu-id="0c842-144">Description of the Role Assignment.</span></span> <span data-ttu-id="0c842-145">[roleAssignment](../resources/intune-rbac-roleassignment.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0c842-145">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="0c842-146">scopeMembers</span><span class="sxs-lookup"><span data-stu-id="0c842-146">scopeMembers</span></span>|<span data-ttu-id="0c842-147">String コレクション</span><span class="sxs-lookup"><span data-stu-id="0c842-147">String collection</span></span>|<span data-ttu-id="0c842-148">役割のスコープ メンバーのセキュリティ グループの ID リスト。</span><span class="sxs-lookup"><span data-stu-id="0c842-148">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="0c842-149">Azure Active Directory の ID。</span><span class="sxs-lookup"><span data-stu-id="0c842-149">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="0c842-150">[roleAssignment](../resources/intune-rbac-roleassignment.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0c842-150">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="0c842-151">scopeType</span><span class="sxs-lookup"><span data-stu-id="0c842-151">scopeType</span></span>|[<span data-ttu-id="0c842-152">roleAssignmentScopeType</span><span class="sxs-lookup"><span data-stu-id="0c842-152">roleAssignmentScopeType</span></span>](../resources/intune-rbac-roleassignmentscopetype.md)|<span data-ttu-id="0c842-153">役割の割り当てのスコープの種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="0c842-153">Specifies the type of scope for a Role Assignment.</span></span> <span data-ttu-id="0c842-154">'ResourceScope' の既定の種類は、ResourceScopes の割り当てを使用できます。</span><span class="sxs-lookup"><span data-stu-id="0c842-154">Default type 'ResourceScope' allows assignment of ResourceScopes.</span></span> <span data-ttu-id="0c842-155">'している'、'AllLicensedUsers'、および 'AllDevicesAndLicensedUsers' の ResourceScopes プロパティは空欄のままです。</span><span class="sxs-lookup"><span data-stu-id="0c842-155">For 'AllDevices', 'AllLicensedUsers', and 'AllDevicesAndLicensedUsers', the ResourceScopes property should be left empty.</span></span> <span data-ttu-id="0c842-156">[RoleAssignment](../resources/intune-rbac-roleassignment.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="0c842-156">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span> <span data-ttu-id="0c842-157">可能な値は、`resourceScope`、`allDevices`、`allLicensedUsers`、`allDevicesAndLicensedUsers` です。</span><span class="sxs-lookup"><span data-stu-id="0c842-157">Possible values are: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span></span>|
|<span data-ttu-id="0c842-158">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="0c842-158">resourceScopes</span></span>|<span data-ttu-id="0c842-159">String コレクション</span><span class="sxs-lookup"><span data-stu-id="0c842-159">String collection</span></span>|<span data-ttu-id="0c842-160">役割のスコープ メンバーのセキュリティ グループの ID リスト。</span><span class="sxs-lookup"><span data-stu-id="0c842-160">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="0c842-161">Azure Active Directory の ID。</span><span class="sxs-lookup"><span data-stu-id="0c842-161">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="0c842-162">[roleAssignment](../resources/intune-rbac-roleassignment.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="0c842-162">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="0c842-163">members</span><span class="sxs-lookup"><span data-stu-id="0c842-163">members</span></span>|<span data-ttu-id="0c842-164">String コレクション</span><span class="sxs-lookup"><span data-stu-id="0c842-164">String collection</span></span>|<span data-ttu-id="0c842-165">ロール メンバーのセキュリティ グループの ID リスト。</span><span class="sxs-lookup"><span data-stu-id="0c842-165">The list of ids of role member security groups.</span></span> <span data-ttu-id="0c842-166">Azure Active Directory の ID。</span><span class="sxs-lookup"><span data-stu-id="0c842-166">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="0c842-167">応答</span><span class="sxs-lookup"><span data-stu-id="0c842-167">Response</span></span>
<span data-ttu-id="0c842-168">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="0c842-168">If successful, this method returns a `201 Created` response code and a [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0c842-169">例</span><span class="sxs-lookup"><span data-stu-id="0c842-169">Example</span></span>
### <a name="request"></a><span data-ttu-id="0c842-170">要求</span><span class="sxs-lookup"><span data-stu-id="0c842-170">Request</span></span>
<span data-ttu-id="0c842-171">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0c842-171">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0c842-172">応答</span><span class="sxs-lookup"><span data-stu-id="0c842-172">Response</span></span>
<span data-ttu-id="0c842-p110">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0c842-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





