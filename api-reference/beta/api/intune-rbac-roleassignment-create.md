---
title: roleAssignment の作成
description: 新しい roleAssignment オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 95986bbf38aef82cd04cd7fa8d58aebea9f443b2
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32527540"
---
# <a name="create-roleassignment"></a><span data-ttu-id="74384-103">roleAssignment の作成</span><span class="sxs-lookup"><span data-stu-id="74384-103">Create roleAssignment</span></span>

> <span data-ttu-id="74384-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="74384-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="74384-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="74384-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="74384-106">新しい [roleAssignment](../resources/intune-rbac-roleassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="74384-106">Create a new [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="74384-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="74384-107">Prerequisites</span></span>
<span data-ttu-id="74384-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="74384-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="74384-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="74384-110">Permission type</span></span>|<span data-ttu-id="74384-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="74384-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="74384-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="74384-112">Delegated (work or school account)</span></span>|<span data-ttu-id="74384-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="74384-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="74384-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="74384-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="74384-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="74384-115">Not supported.</span></span>|
|<span data-ttu-id="74384-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="74384-116">Application</span></span>|<span data-ttu-id="74384-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="74384-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="74384-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="74384-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="74384-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="74384-119">Request headers</span></span>
|<span data-ttu-id="74384-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="74384-120">Header</span></span>|<span data-ttu-id="74384-121">値</span><span class="sxs-lookup"><span data-stu-id="74384-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="74384-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="74384-122">Authorization</span></span>|<span data-ttu-id="74384-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="74384-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="74384-124">承諾</span><span class="sxs-lookup"><span data-stu-id="74384-124">Accept</span></span>|<span data-ttu-id="74384-125">application/json</span><span class="sxs-lookup"><span data-stu-id="74384-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="74384-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="74384-126">Request body</span></span>
<span data-ttu-id="74384-127">要求本文で、roleAssignment オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="74384-127">In the request body, supply a JSON representation for the roleAssignment object.</span></span>

<span data-ttu-id="74384-128">次の表に、roleAssignment の作成時に必要になるプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="74384-128">The following table shows the properties that are required when you create the roleAssignment.</span></span>

|<span data-ttu-id="74384-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="74384-129">Property</span></span>|<span data-ttu-id="74384-130">型</span><span class="sxs-lookup"><span data-stu-id="74384-130">Type</span></span>|<span data-ttu-id="74384-131">説明</span><span class="sxs-lookup"><span data-stu-id="74384-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="74384-132">id</span><span class="sxs-lookup"><span data-stu-id="74384-132">id</span></span>|<span data-ttu-id="74384-133">String</span><span class="sxs-lookup"><span data-stu-id="74384-133">String</span></span>|<span data-ttu-id="74384-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="74384-134">Key of the entity.</span></span> <span data-ttu-id="74384-135">これは読み取り専用で、自動生成されます。</span><span class="sxs-lookup"><span data-stu-id="74384-135">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="74384-136">displayName</span><span class="sxs-lookup"><span data-stu-id="74384-136">displayName</span></span>|<span data-ttu-id="74384-137">String</span><span class="sxs-lookup"><span data-stu-id="74384-137">String</span></span>|<span data-ttu-id="74384-138">ロール割り当ての表示名またはフレンドリ名。</span><span class="sxs-lookup"><span data-stu-id="74384-138">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="74384-139">description</span><span class="sxs-lookup"><span data-stu-id="74384-139">description</span></span>|<span data-ttu-id="74384-140">String</span><span class="sxs-lookup"><span data-stu-id="74384-140">String</span></span>|<span data-ttu-id="74384-141">ロール割り当ての説明。</span><span class="sxs-lookup"><span data-stu-id="74384-141">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="74384-142">scopeMembers</span><span class="sxs-lookup"><span data-stu-id="74384-142">scopeMembers</span></span>|<span data-ttu-id="74384-143">String コレクション</span><span class="sxs-lookup"><span data-stu-id="74384-143">String collection</span></span>|<span data-ttu-id="74384-144">役割のスコープ メンバーのセキュリティ グループの ID リスト。</span><span class="sxs-lookup"><span data-stu-id="74384-144">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="74384-145">Azure Active Directory の ID。</span><span class="sxs-lookup"><span data-stu-id="74384-145">These are IDs from Azure Active Directory.</span></span>|
|<span data-ttu-id="74384-146">scopeType</span><span class="sxs-lookup"><span data-stu-id="74384-146">scopeType</span></span>|[<span data-ttu-id="74384-147">roleAssignmentScopeType</span><span class="sxs-lookup"><span data-stu-id="74384-147">roleAssignmentScopeType</span></span>](../resources/intune-rbac-roleassignmentscopetype.md)|<span data-ttu-id="74384-148">役割の割り当てのスコープの種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="74384-148">Specifies the type of scope for a Role Assignment.</span></span> <span data-ttu-id="74384-149">既定の種類 ' resourcescope ' では、を割り当てることができます。</span><span class="sxs-lookup"><span data-stu-id="74384-149">Default type 'ResourceScope' allows assignment of ResourceScopes.</span></span> <span data-ttu-id="74384-150">' alldevices '、' AllLicensedUsers '、および ' AllDevicesAndLicensedUsers ' の場合、ResourceScopes プロパティは空のままにする必要があります。</span><span class="sxs-lookup"><span data-stu-id="74384-150">For 'AllDevices', 'AllLicensedUsers', and 'AllDevicesAndLicensedUsers', the ResourceScopes property should be left empty.</span></span> <span data-ttu-id="74384-151">可能な値は、`resourceScope`、`allDevices`、`allLicensedUsers`、`allDevicesAndLicensedUsers` です。</span><span class="sxs-lookup"><span data-stu-id="74384-151">Possible values are: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span></span>|
|<span data-ttu-id="74384-152">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="74384-152">resourceScopes</span></span>|<span data-ttu-id="74384-153">String コレクション</span><span class="sxs-lookup"><span data-stu-id="74384-153">String collection</span></span>|<span data-ttu-id="74384-154">役割のスコープ メンバーのセキュリティ グループの ID リスト。</span><span class="sxs-lookup"><span data-stu-id="74384-154">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="74384-155">Azure Active Directory の ID。</span><span class="sxs-lookup"><span data-stu-id="74384-155">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="74384-156">応答</span><span class="sxs-lookup"><span data-stu-id="74384-156">Response</span></span>
<span data-ttu-id="74384-157">成功した場合、このメソッドは `201 Created` 応答コードと応答本文で [roleAssignment](../resources/intune-rbac-roleassignment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="74384-157">If successful, this method returns a `201 Created` response code and a [roleAssignment](../resources/intune-rbac-roleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="74384-158">例</span><span class="sxs-lookup"><span data-stu-id="74384-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="74384-159">要求</span><span class="sxs-lookup"><span data-stu-id="74384-159">Request</span></span>
<span data-ttu-id="74384-160">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="74384-160">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="74384-161">応答</span><span class="sxs-lookup"><span data-stu-id="74384-161">Response</span></span>
<span data-ttu-id="74384-p106">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="74384-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





