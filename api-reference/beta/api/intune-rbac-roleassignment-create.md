---
title: roleAssignment の作成
description: 新しい roleAssignment オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0fea340156edda5f697d7dd5210c8bde85165a88
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36351351"
---
# <a name="create-roleassignment"></a><span data-ttu-id="4fc46-103">roleAssignment の作成</span><span class="sxs-lookup"><span data-stu-id="4fc46-103">Create roleAssignment</span></span>

> <span data-ttu-id="4fc46-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4fc46-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4fc46-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4fc46-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4fc46-106">新しい [roleAssignment](../resources/intune-rbac-roleassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="4fc46-106">Create a new [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4fc46-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="4fc46-107">Prerequisites</span></span>
<span data-ttu-id="4fc46-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4fc46-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4fc46-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4fc46-110">Permission type</span></span>|<span data-ttu-id="4fc46-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="4fc46-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4fc46-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4fc46-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4fc46-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4fc46-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="4fc46-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4fc46-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4fc46-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4fc46-115">Not supported.</span></span>|
|<span data-ttu-id="4fc46-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4fc46-116">Application</span></span>|<span data-ttu-id="4fc46-117">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4fc46-117">DeviceManagementRBAC.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4fc46-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4fc46-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="4fc46-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4fc46-119">Request headers</span></span>
|<span data-ttu-id="4fc46-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4fc46-120">Header</span></span>|<span data-ttu-id="4fc46-121">値</span><span class="sxs-lookup"><span data-stu-id="4fc46-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4fc46-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4fc46-122">Authorization</span></span>|<span data-ttu-id="4fc46-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="4fc46-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4fc46-124">承諾</span><span class="sxs-lookup"><span data-stu-id="4fc46-124">Accept</span></span>|<span data-ttu-id="4fc46-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4fc46-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4fc46-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="4fc46-126">Request body</span></span>
<span data-ttu-id="4fc46-127">要求本文で、roleAssignment オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="4fc46-127">In the request body, supply a JSON representation for the roleAssignment object.</span></span>

<span data-ttu-id="4fc46-128">次の表に、roleAssignment の作成時に必要になるプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="4fc46-128">The following table shows the properties that are required when you create the roleAssignment.</span></span>

|<span data-ttu-id="4fc46-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4fc46-129">Property</span></span>|<span data-ttu-id="4fc46-130">型</span><span class="sxs-lookup"><span data-stu-id="4fc46-130">Type</span></span>|<span data-ttu-id="4fc46-131">説明</span><span class="sxs-lookup"><span data-stu-id="4fc46-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4fc46-132">id</span><span class="sxs-lookup"><span data-stu-id="4fc46-132">id</span></span>|<span data-ttu-id="4fc46-133">文字列</span><span class="sxs-lookup"><span data-stu-id="4fc46-133">String</span></span>|<span data-ttu-id="4fc46-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="4fc46-134">Key of the entity.</span></span> <span data-ttu-id="4fc46-135">これは読み取り専用で、自動生成されます。</span><span class="sxs-lookup"><span data-stu-id="4fc46-135">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="4fc46-136">displayName</span><span class="sxs-lookup"><span data-stu-id="4fc46-136">displayName</span></span>|<span data-ttu-id="4fc46-137">String</span><span class="sxs-lookup"><span data-stu-id="4fc46-137">String</span></span>|<span data-ttu-id="4fc46-138">ロール割り当ての表示名またはフレンドリ名。</span><span class="sxs-lookup"><span data-stu-id="4fc46-138">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="4fc46-139">description</span><span class="sxs-lookup"><span data-stu-id="4fc46-139">description</span></span>|<span data-ttu-id="4fc46-140">String</span><span class="sxs-lookup"><span data-stu-id="4fc46-140">String</span></span>|<span data-ttu-id="4fc46-141">ロール割り当ての説明。</span><span class="sxs-lookup"><span data-stu-id="4fc46-141">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="4fc46-142">scopeMembers</span><span class="sxs-lookup"><span data-stu-id="4fc46-142">scopeMembers</span></span>|<span data-ttu-id="4fc46-143">String コレクション</span><span class="sxs-lookup"><span data-stu-id="4fc46-143">String collection</span></span>|<span data-ttu-id="4fc46-144">役割のスコープ メンバーのセキュリティ グループの ID リスト。</span><span class="sxs-lookup"><span data-stu-id="4fc46-144">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="4fc46-145">Azure Active Directory の ID。</span><span class="sxs-lookup"><span data-stu-id="4fc46-145">These are IDs from Azure Active Directory.</span></span>|
|<span data-ttu-id="4fc46-146">scopeType</span><span class="sxs-lookup"><span data-stu-id="4fc46-146">scopeType</span></span>|[<span data-ttu-id="4fc46-147">roleAssignmentScopeType</span><span class="sxs-lookup"><span data-stu-id="4fc46-147">roleAssignmentScopeType</span></span>](../resources/intune-rbac-roleassignmentscopetype.md)|<span data-ttu-id="4fc46-148">役割の割り当てのスコープの種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="4fc46-148">Specifies the type of scope for a Role Assignment.</span></span> <span data-ttu-id="4fc46-149">既定の種類 ' ResourceScope ' では、を割り当てることができます。</span><span class="sxs-lookup"><span data-stu-id="4fc46-149">Default type 'ResourceScope' allows assignment of ResourceScopes.</span></span> <span data-ttu-id="4fc46-150">' AllDevices '、' AllLicensedUsers '、および ' AllDevicesAndLicensedUsers ' の場合、ResourceScopes プロパティは空のままにする必要があります。</span><span class="sxs-lookup"><span data-stu-id="4fc46-150">For 'AllDevices', 'AllLicensedUsers', and 'AllDevicesAndLicensedUsers', the ResourceScopes property should be left empty.</span></span> <span data-ttu-id="4fc46-151">使用可能な値は、`resourceScope`、`allDevices`、`allLicensedUsers`、`allDevicesAndLicensedUsers` です。</span><span class="sxs-lookup"><span data-stu-id="4fc46-151">Possible values are: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span></span>|
|<span data-ttu-id="4fc46-152">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="4fc46-152">resourceScopes</span></span>|<span data-ttu-id="4fc46-153">String コレクション</span><span class="sxs-lookup"><span data-stu-id="4fc46-153">String collection</span></span>|<span data-ttu-id="4fc46-154">役割のスコープ メンバーのセキュリティ グループの ID リスト。</span><span class="sxs-lookup"><span data-stu-id="4fc46-154">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="4fc46-155">Azure Active Directory の ID。</span><span class="sxs-lookup"><span data-stu-id="4fc46-155">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="4fc46-156">応答</span><span class="sxs-lookup"><span data-stu-id="4fc46-156">Response</span></span>
<span data-ttu-id="4fc46-157">成功した場合、このメソッドは `201 Created` 応答コードと応答本文で [roleAssignment](../resources/intune-rbac-roleassignment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="4fc46-157">If successful, this method returns a `201 Created` response code and a [roleAssignment](../resources/intune-rbac-roleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4fc46-158">例</span><span class="sxs-lookup"><span data-stu-id="4fc46-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="4fc46-159">要求</span><span class="sxs-lookup"><span data-stu-id="4fc46-159">Request</span></span>
<span data-ttu-id="4fc46-160">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4fc46-160">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments
Content-type: application/json
Content-length: 277

{
  "@odata.type": "#microsoft.graph.roleAssignment",
  "displayName": "Display Name value",
  "description": "Description value",
  "scopeMembers": [
    "Scope Members value"
  ],
  "scopeType": "allDevices",
  "resourceScopes": [
    "Resource Scopes value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="4fc46-161">応答</span><span class="sxs-lookup"><span data-stu-id="4fc46-161">Response</span></span>
<span data-ttu-id="4fc46-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4fc46-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 326

{
  "@odata.type": "#microsoft.graph.roleAssignment",
  "id": "b3234d24-4d24-b323-244d-23b3244d23b3",
  "displayName": "Display Name value",
  "description": "Description value",
  "scopeMembers": [
    "Scope Members value"
  ],
  "scopeType": "allDevices",
  "resourceScopes": [
    "Resource Scopes value"
  ]
}
```






