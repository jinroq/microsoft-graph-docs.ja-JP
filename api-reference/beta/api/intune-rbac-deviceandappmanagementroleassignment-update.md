---
title: deviceAndAppManagementRoleAssignment の更新
description: deviceAndAppManagementRoleAssignment オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1cbdc5b74b0143189872f9117e619a827741d7eb
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29416497"
---
# <a name="update-deviceandappmanagementroleassignment"></a><span data-ttu-id="46774-103">deviceAndAppManagementRoleAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="46774-103">Update deviceAndAppManagementRoleAssignment</span></span>

> <span data-ttu-id="46774-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="46774-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="46774-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="46774-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="46774-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="46774-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="46774-107">[deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="46774-107">Update the properties of a [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="46774-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="46774-108">Prerequisites</span></span>
<span data-ttu-id="46774-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="46774-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="46774-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="46774-111">Permission type</span></span>|<span data-ttu-id="46774-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="46774-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="46774-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="46774-113">Delegated (work or school account)</span></span>|<span data-ttu-id="46774-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="46774-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="46774-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="46774-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="46774-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="46774-116">Not supported.</span></span>|
|<span data-ttu-id="46774-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="46774-117">Application</span></span>|<span data-ttu-id="46774-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="46774-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="46774-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="46774-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleAssignments/{deviceAndAppManagementRoleAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="46774-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="46774-120">Request headers</span></span>
|<span data-ttu-id="46774-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="46774-121">Header</span></span>|<span data-ttu-id="46774-122">値</span><span class="sxs-lookup"><span data-stu-id="46774-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="46774-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="46774-123">Authorization</span></span>|<span data-ttu-id="46774-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="46774-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="46774-125">Accept</span><span class="sxs-lookup"><span data-stu-id="46774-125">Accept</span></span>|<span data-ttu-id="46774-126">application/json</span><span class="sxs-lookup"><span data-stu-id="46774-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="46774-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="46774-127">Request body</span></span>
<span data-ttu-id="46774-128">要求本文で、[deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="46774-128">In the request body, supply a JSON representation for the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object.</span></span>

<span data-ttu-id="46774-129">次の表に、[deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="46774-129">The following table shows the properties that are required when you create the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md).</span></span>

|<span data-ttu-id="46774-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="46774-130">Property</span></span>|<span data-ttu-id="46774-131">型</span><span class="sxs-lookup"><span data-stu-id="46774-131">Type</span></span>|<span data-ttu-id="46774-132">説明</span><span class="sxs-lookup"><span data-stu-id="46774-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="46774-133">id</span><span class="sxs-lookup"><span data-stu-id="46774-133">id</span></span>|<span data-ttu-id="46774-134">String</span><span class="sxs-lookup"><span data-stu-id="46774-134">String</span></span>|<span data-ttu-id="46774-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="46774-135">Key of the entity.</span></span> <span data-ttu-id="46774-136">これは読み取り専用で、自動生成されます。</span><span class="sxs-lookup"><span data-stu-id="46774-136">This is read-only and automatically generated.</span></span> <span data-ttu-id="46774-137">[roleAssignment](../resources/intune-rbac-roleassignment.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="46774-137">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="46774-138">displayName</span><span class="sxs-lookup"><span data-stu-id="46774-138">displayName</span></span>|<span data-ttu-id="46774-139">String</span><span class="sxs-lookup"><span data-stu-id="46774-139">String</span></span>|<span data-ttu-id="46774-140">ロール割り当ての表示名またはフレンドリ名。</span><span class="sxs-lookup"><span data-stu-id="46774-140">The display or friendly name of the role Assignment.</span></span> <span data-ttu-id="46774-141">[roleAssignment](../resources/intune-rbac-roleassignment.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="46774-141">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="46774-142">説明</span><span class="sxs-lookup"><span data-stu-id="46774-142">description</span></span>|<span data-ttu-id="46774-143">String</span><span class="sxs-lookup"><span data-stu-id="46774-143">String</span></span>|<span data-ttu-id="46774-144">ロール割り当ての説明。</span><span class="sxs-lookup"><span data-stu-id="46774-144">Description of the Role Assignment.</span></span> <span data-ttu-id="46774-145">[roleAssignment](../resources/intune-rbac-roleassignment.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="46774-145">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="46774-146">scopeMembers</span><span class="sxs-lookup"><span data-stu-id="46774-146">scopeMembers</span></span>|<span data-ttu-id="46774-147">String コレクション</span><span class="sxs-lookup"><span data-stu-id="46774-147">String collection</span></span>|<span data-ttu-id="46774-148">役割のスコープ メンバーのセキュリティ グループの ID リスト。</span><span class="sxs-lookup"><span data-stu-id="46774-148">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="46774-149">Azure Active Directory の ID。</span><span class="sxs-lookup"><span data-stu-id="46774-149">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="46774-150">[roleAssignment](../resources/intune-rbac-roleassignment.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="46774-150">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="46774-151">scopeType</span><span class="sxs-lookup"><span data-stu-id="46774-151">scopeType</span></span>|[<span data-ttu-id="46774-152">roleAssignmentScopeType</span><span class="sxs-lookup"><span data-stu-id="46774-152">roleAssignmentScopeType</span></span>](../resources/intune-rbac-roleassignmentscopetype.md)|<span data-ttu-id="46774-153">役割の割り当てのスコープの種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="46774-153">Specifies the type of scope for a Role Assignment.</span></span> <span data-ttu-id="46774-154">'ResourceScope' の既定の種類は、ResourceScopes の割り当てを使用できます。</span><span class="sxs-lookup"><span data-stu-id="46774-154">Default type 'ResourceScope' allows assignment of ResourceScopes.</span></span> <span data-ttu-id="46774-155">'している'、'AllLicensedUsers'、および 'AllDevicesAndLicensedUsers' の ResourceScopes プロパティは空欄のままです。</span><span class="sxs-lookup"><span data-stu-id="46774-155">For 'AllDevices', 'AllLicensedUsers', and 'AllDevicesAndLicensedUsers', the ResourceScopes property should be left empty.</span></span> <span data-ttu-id="46774-156">[RoleAssignment](../resources/intune-rbac-roleassignment.md)から継承されます。</span><span class="sxs-lookup"><span data-stu-id="46774-156">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span> <span data-ttu-id="46774-157">可能な値は、`resourceScope`、`allDevices`、`allLicensedUsers`、`allDevicesAndLicensedUsers` です。</span><span class="sxs-lookup"><span data-stu-id="46774-157">Possible values are: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span></span>|
|<span data-ttu-id="46774-158">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="46774-158">resourceScopes</span></span>|<span data-ttu-id="46774-159">String コレクション</span><span class="sxs-lookup"><span data-stu-id="46774-159">String collection</span></span>|<span data-ttu-id="46774-160">役割のスコープ メンバーのセキュリティ グループの ID リスト。</span><span class="sxs-lookup"><span data-stu-id="46774-160">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="46774-161">Azure Active Directory の ID。</span><span class="sxs-lookup"><span data-stu-id="46774-161">These are IDs from Azure Active Directory.</span></span> <span data-ttu-id="46774-162">[roleAssignment](../resources/intune-rbac-roleassignment.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="46774-162">Inherited from [roleAssignment](../resources/intune-rbac-roleassignment.md)</span></span>|
|<span data-ttu-id="46774-163">members</span><span class="sxs-lookup"><span data-stu-id="46774-163">members</span></span>|<span data-ttu-id="46774-164">String コレクション</span><span class="sxs-lookup"><span data-stu-id="46774-164">String collection</span></span>|<span data-ttu-id="46774-165">ロール メンバーのセキュリティ グループの ID リスト。</span><span class="sxs-lookup"><span data-stu-id="46774-165">The list of ids of role member security groups.</span></span> <span data-ttu-id="46774-166">Azure Active Directory の ID。</span><span class="sxs-lookup"><span data-stu-id="46774-166">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="46774-167">応答</span><span class="sxs-lookup"><span data-stu-id="46774-167">Response</span></span>
<span data-ttu-id="46774-168">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で、更新された [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="46774-168">If successful, this method returns a `200 OK` response code and an updated [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="46774-169">例</span><span class="sxs-lookup"><span data-stu-id="46774-169">Example</span></span>

### <a name="request"></a><span data-ttu-id="46774-170">要求</span><span class="sxs-lookup"><span data-stu-id="46774-170">Request</span></span>
<span data-ttu-id="46774-171">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="46774-171">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/roleAssignments/{deviceAndAppManagementRoleAssignmentId}
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

### <a name="response"></a><span data-ttu-id="46774-172">応答</span><span class="sxs-lookup"><span data-stu-id="46774-172">Response</span></span>
<span data-ttu-id="46774-p110">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="46774-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




