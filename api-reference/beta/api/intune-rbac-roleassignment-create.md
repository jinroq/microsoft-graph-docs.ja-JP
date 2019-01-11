---
title: roleAssignment の作成
description: 新しい roleAssignment オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 486aaf7a47631f99c86150e08c8672f513e04337
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27806679"
---
# <a name="create-roleassignment"></a><span data-ttu-id="fba06-103">roleAssignment の作成</span><span class="sxs-lookup"><span data-stu-id="fba06-103">Create roleAssignment</span></span>

> <span data-ttu-id="fba06-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="fba06-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fba06-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fba06-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fba06-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="fba06-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fba06-107">新しい [roleAssignment](../resources/intune-rbac-roleassignment.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="fba06-107">Create a new [roleAssignment](../resources/intune-rbac-roleassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fba06-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="fba06-108">Prerequisites</span></span>
<span data-ttu-id="fba06-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fba06-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fba06-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fba06-111">Permission type</span></span>|<span data-ttu-id="fba06-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="fba06-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fba06-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fba06-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fba06-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fba06-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="fba06-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fba06-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fba06-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fba06-116">Not supported.</span></span>|
|<span data-ttu-id="fba06-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fba06-117">Application</span></span>|<span data-ttu-id="fba06-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fba06-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fba06-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fba06-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="fba06-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fba06-120">Request headers</span></span>
|<span data-ttu-id="fba06-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fba06-121">Header</span></span>|<span data-ttu-id="fba06-122">値</span><span class="sxs-lookup"><span data-stu-id="fba06-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fba06-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fba06-123">Authorization</span></span>|<span data-ttu-id="fba06-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="fba06-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fba06-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fba06-125">Accept</span></span>|<span data-ttu-id="fba06-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fba06-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fba06-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="fba06-127">Request body</span></span>
<span data-ttu-id="fba06-128">要求本文で、roleAssignment オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="fba06-128">In the request body, supply a JSON representation for the roleAssignment object.</span></span>

<span data-ttu-id="fba06-129">次の表に、roleAssignment の作成時に必要になるプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="fba06-129">The following table shows the properties that are required when you create the roleAssignment.</span></span>

|<span data-ttu-id="fba06-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fba06-130">Property</span></span>|<span data-ttu-id="fba06-131">種類</span><span class="sxs-lookup"><span data-stu-id="fba06-131">Type</span></span>|<span data-ttu-id="fba06-132">説明</span><span class="sxs-lookup"><span data-stu-id="fba06-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fba06-133">ID</span><span class="sxs-lookup"><span data-stu-id="fba06-133">id</span></span>|<span data-ttu-id="fba06-134">String</span><span class="sxs-lookup"><span data-stu-id="fba06-134">String</span></span>|<span data-ttu-id="fba06-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="fba06-135">Key of the entity.</span></span> <span data-ttu-id="fba06-136">これは読み取り専用で、自動生成されます。</span><span class="sxs-lookup"><span data-stu-id="fba06-136">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="fba06-137">displayName</span><span class="sxs-lookup"><span data-stu-id="fba06-137">displayName</span></span>|<span data-ttu-id="fba06-138">String</span><span class="sxs-lookup"><span data-stu-id="fba06-138">String</span></span>|<span data-ttu-id="fba06-139">ロール割り当ての表示名またはフレンドリ名。</span><span class="sxs-lookup"><span data-stu-id="fba06-139">The display or friendly name of the role Assignment.</span></span>|
|<span data-ttu-id="fba06-140">説明</span><span class="sxs-lookup"><span data-stu-id="fba06-140">description</span></span>|<span data-ttu-id="fba06-141">String</span><span class="sxs-lookup"><span data-stu-id="fba06-141">String</span></span>|<span data-ttu-id="fba06-142">ロール割り当ての説明。</span><span class="sxs-lookup"><span data-stu-id="fba06-142">Description of the Role Assignment.</span></span>|
|<span data-ttu-id="fba06-143">scopeMembers</span><span class="sxs-lookup"><span data-stu-id="fba06-143">scopeMembers</span></span>|<span data-ttu-id="fba06-144">String コレクション</span><span class="sxs-lookup"><span data-stu-id="fba06-144">String collection</span></span>|<span data-ttu-id="fba06-145">役割のスコープ メンバーのセキュリティ グループの ID リスト。</span><span class="sxs-lookup"><span data-stu-id="fba06-145">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="fba06-146">Azure Active Directory の ID。</span><span class="sxs-lookup"><span data-stu-id="fba06-146">These are IDs from Azure Active Directory.</span></span>|
|<span data-ttu-id="fba06-147">scopeType</span><span class="sxs-lookup"><span data-stu-id="fba06-147">scopeType</span></span>|[<span data-ttu-id="fba06-148">roleAssignmentScopeType</span><span class="sxs-lookup"><span data-stu-id="fba06-148">roleAssignmentScopeType</span></span>](../resources/intune-rbac-roleassignmentscopetype.md)|<span data-ttu-id="fba06-149">役割の割り当てのスコープの種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="fba06-149">Specifies the type of scope for a Role Assignment.</span></span> <span data-ttu-id="fba06-150">'ResourceScope' の既定の種類は、ResourceScopes の割り当てを使用できます。</span><span class="sxs-lookup"><span data-stu-id="fba06-150">Default type 'ResourceScope' allows assignment of ResourceScopes.</span></span> <span data-ttu-id="fba06-151">'している'、'AllLicensedUsers'、および 'AllDevicesAndLicensedUsers' の ResourceScopes プロパティは空欄のままです。</span><span class="sxs-lookup"><span data-stu-id="fba06-151">For 'AllDevices', 'AllLicensedUsers', and 'AllDevicesAndLicensedUsers', the ResourceScopes property should be left empty.</span></span> <span data-ttu-id="fba06-152">可能な値は、`resourceScope`、`allDevices`、`allLicensedUsers`、`allDevicesAndLicensedUsers` です。</span><span class="sxs-lookup"><span data-stu-id="fba06-152">Possible values are: `resourceScope`, `allDevices`, `allLicensedUsers`, `allDevicesAndLicensedUsers`.</span></span>|
|<span data-ttu-id="fba06-153">resourceScopes</span><span class="sxs-lookup"><span data-stu-id="fba06-153">resourceScopes</span></span>|<span data-ttu-id="fba06-154">String コレクション</span><span class="sxs-lookup"><span data-stu-id="fba06-154">String collection</span></span>|<span data-ttu-id="fba06-155">役割のスコープ メンバーのセキュリティ グループの ID リスト。</span><span class="sxs-lookup"><span data-stu-id="fba06-155">List of ids of role scope member security groups.</span></span>  <span data-ttu-id="fba06-156">Azure Active Directory の ID。</span><span class="sxs-lookup"><span data-stu-id="fba06-156">These are IDs from Azure Active Directory.</span></span>|



## <a name="response"></a><span data-ttu-id="fba06-157">応答</span><span class="sxs-lookup"><span data-stu-id="fba06-157">Response</span></span>
<span data-ttu-id="fba06-158">成功した場合、このメソッドは `201 Created` 応答コードと応答本文で [roleAssignment](../resources/intune-rbac-roleassignment.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="fba06-158">If successful, this method returns a `201 Created` response code and a [roleAssignment](../resources/intune-rbac-roleassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fba06-159">例</span><span class="sxs-lookup"><span data-stu-id="fba06-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="fba06-160">要求</span><span class="sxs-lookup"><span data-stu-id="fba06-160">Request</span></span>
<span data-ttu-id="fba06-161">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="fba06-161">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="fba06-162">応答</span><span class="sxs-lookup"><span data-stu-id="fba06-162">Response</span></span>
<span data-ttu-id="fba06-p107">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="fba06-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





