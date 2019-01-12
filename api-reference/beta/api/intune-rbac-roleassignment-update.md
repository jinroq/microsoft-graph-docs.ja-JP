---
title: roleAssignment の更新
description: roleAssignment オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: f35f7ee957250a546d721a615036f18648d28ff7
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27913877"
---
# <a name="update-roleassignment"></a><span data-ttu-id="9168e-103">roleAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="9168e-103">Update roleAssignment</span></span>

> <span data-ttu-id="9168e-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9168e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9168e-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9168e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9168e-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="9168e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9168e-107">[roleAssignment](../resources/intune-rbac-roleassignment.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="9168e-107">Update the properties of a [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9168e-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="9168e-108">Prerequisites</span></span>
<span data-ttu-id="9168e-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9168e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9168e-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9168e-111">Permission type</span></span>|<span data-ttu-id="9168e-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="9168e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9168e-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9168e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9168e-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9168e-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="9168e-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9168e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9168e-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9168e-116">Not supported.</span></span>|
|<span data-ttu-id="9168e-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9168e-117">Application</span></span>|<span data-ttu-id="9168e-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9168e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9168e-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9168e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="9168e-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9168e-120">Request headers</span></span>
|<span data-ttu-id="9168e-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9168e-121">Header</span></span>|<span data-ttu-id="9168e-122">値</span><span class="sxs-lookup"><span data-stu-id="9168e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9168e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9168e-123">Authorization</span></span>|<span data-ttu-id="9168e-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="9168e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9168e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="9168e-125">Accept</span></span>|<span data-ttu-id="9168e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9168e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9168e-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="9168e-127">Request body</span></span>
<span data-ttu-id="9168e-128">要求本文で、[roleAssignment](../resources/intune-rbac-roleassignment.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="9168e-128">In the request body, supply a JSON representation for the [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>

<span data-ttu-id="9168e-129">次の表に、[roleAssignment](../resources/intune-rbac-roleassignment.md) の作成時に必要になるプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="9168e-129">The following table shows the properties that are required when you create the [roleAssignment](../resources/intune-rbac-roleassignment.md).</span></span>

|<span data-ttu-id="9168e-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9168e-130">Property</span></span>|<span data-ttu-id="9168e-131">型</span><span class="sxs-lookup"><span data-stu-id="9168e-131">Type</span></span>|<span data-ttu-id="9168e-132">説明</span><span class="sxs-lookup"><span data-stu-id="9168e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9168e-133">ID</span><span class="sxs-lookup"><span data-stu-id="9168e-133">id</span></span>|<span data-ttu-id="9168e-134">String</span><span class="sxs-lookup"><span data-stu-id="9168e-134">String</span></span>|<span data-ttu-id="9168e-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="9168e-135">Key of the entity.</span></span> <span data-ttu-id="9168e-136">これは読み取り専用で、自動生成されます。</span><span class="sxs-lookup"><span data-stu-id="9168e-136">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="9168e-137">displayName</span><span class="sxs-lookup"><span data-stu-id="9168e-137">displayName</span></span>|<span data-ttu-id="9168e-138">String</span><span class="sxs-lookup"><span data-stu-id="9168e-138">String</span></span>|<span data-ttu-id="9168e-139">ロール割り当ての表示名またはフレンドリ名。</span><span class="sxs-lookup"><span data-stu-id="9168e-139">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="9168e-140">説明</span><span class="sxs-lookup"><span data-stu-id="9168e-140">description</span></span>|<span data-ttu-id="9168e-141">String</span><span class="sxs-lookup"><span data-stu-id="9168e-141">String</span></span>|<span data-ttu-id="9168e-142">ロール割り当ての説明。</span><span class="sxs-lookup"><span data-stu-id="9168e-142">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="9168e-143">scopeMembers</span><span class="sxs-lookup"><span data-stu-id="9168e-143">scopeMembers</span></span>|<span data-ttu-id="9168e-144">String コレクション</span><span class="sxs-lookup"><span data-stu-id="9168e-144">String collection</span></span>|<span data-ttu-id="9168e-145">役割のスコープ メンバーのセキュリティ グループの ID リスト。</span><span class="sxs-lookup"><span data-stu-id="9168e-145">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="9168e-146">Azure Active Directory の ID。</span><span class="sxs-lookup"><span data-stu-id="9168e-146">These are IDs from Azure Active Directory.</span></span>|
|<span data-ttu-id="9168e-147">scopeType</span><span class="sxs-lookup"><span data-stu-id="9168e-147">scopeType</span></span>|[<span data-ttu-id="9168e-148">roleAssignmentScopeType</span><span class="sxs-lookup"><span data-stu-id="9168e-148">roleAssignmentScopeType</span></span>](../resources/intune-rbac-roleassignmentscopetype.md)|<span data-ttu-id="9168e-149">役割の割り当てのスコープの種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="9168e-149">Specifies the type of scope for a Role Assignment.</span></span> <span data-ttu-id="9168e-150">'ResourceScope' の既定の種類は、ResourceScopes の割り当てを使用できます。</span><span class="sxs-lookup"><span data-stu-id="9168e-150">Default type 'ResourceScope' allows assignment of ResourceScopes.</span></span> <span data-ttu-id="9168e-151">'している'、'AllLicensedUsers'、および 'AllDevicesAndLicensedUsers' の ResourceScopes プロパティは空欄のままです。</span><span class="sxs-lookup"><span data-stu-id="9168e-151">For 'AllDevices', 'AllLicensedUsers', and 'AllDevicesAndLicensedUsers', the ResourceScopes property should be left empty.</span></span> <span data-ttu-id="9168e-152">可能な値は、`resourceScope`、`allDevices`、`allLicensedUsers`、`allDevicesAndLicensedUsers` です。</span><span class="sxs-lookup"><span data-stu-id="9168e-152">Possible values are: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span></span>|
|<span data-ttu-id="9168e-153">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="9168e-153">resourceScopes</span></span>|<span data-ttu-id="9168e-154">String コレクション</span><span class="sxs-lookup"><span data-stu-id="9168e-154">String collection</span></span>|<span data-ttu-id="9168e-155">役割のスコープ メンバーのセキュリティ グループの ID リスト。</span><span class="sxs-lookup"><span data-stu-id="9168e-155">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="9168e-156">Azure Active Directory の ID。</span><span class="sxs-lookup"><span data-stu-id="9168e-156">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="9168e-157">応答</span><span class="sxs-lookup"><span data-stu-id="9168e-157">Response</span></span>
<span data-ttu-id="9168e-158">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [roleAssignment](../resources/intune-rbac-roleassignment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="9168e-158">If successful, this method returns a `200 OK` response code and an updated [roleAssignment](../resources/intune-rbac-roleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9168e-159">例</span><span class="sxs-lookup"><span data-stu-id="9168e-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="9168e-160">要求</span><span class="sxs-lookup"><span data-stu-id="9168e-160">Request</span></span>
<span data-ttu-id="9168e-161">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9168e-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}
Content-type: application/json
Content-length: 224

{
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

### <a name="response"></a><span data-ttu-id="9168e-162">応答</span><span class="sxs-lookup"><span data-stu-id="9168e-162">Response</span></span>
<span data-ttu-id="9168e-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="9168e-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





