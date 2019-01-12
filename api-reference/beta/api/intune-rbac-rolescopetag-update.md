---
title: RoleScopeTag を更新します。
description: RoleScopeTag オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ec006889750999bf2a61aaefd6fba7bc5b747999
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27933521"
---
# <a name="update-rolescopetag"></a><span data-ttu-id="c0846-103">RoleScopeTag を更新します。</span><span class="sxs-lookup"><span data-stu-id="c0846-103">Update roleScopeTag</span></span>

> <span data-ttu-id="c0846-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c0846-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c0846-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c0846-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c0846-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c0846-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c0846-107">[RoleScopeTag](../resources/intune-rbac-rolescopetag.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="c0846-107">Update the properties of a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c0846-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="c0846-108">Prerequisites</span></span>
<span data-ttu-id="c0846-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c0846-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c0846-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c0846-111">Permission type</span></span>|<span data-ttu-id="c0846-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="c0846-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c0846-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c0846-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c0846-114">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c0846-114">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="c0846-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c0846-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c0846-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c0846-116">Not supported.</span></span>|
|<span data-ttu-id="c0846-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c0846-117">Application</span></span>|<span data-ttu-id="c0846-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c0846-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c0846-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c0846-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/roleScopeTags/{roleScopeTagId}
PATCH /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/{roleScopeTagId}
```

## <a name="request-headers"></a><span data-ttu-id="c0846-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c0846-120">Request headers</span></span>
|<span data-ttu-id="c0846-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c0846-121">Header</span></span>|<span data-ttu-id="c0846-122">値</span><span class="sxs-lookup"><span data-stu-id="c0846-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c0846-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c0846-123">Authorization</span></span>|<span data-ttu-id="c0846-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="c0846-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c0846-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c0846-125">Accept</span></span>|<span data-ttu-id="c0846-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c0846-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c0846-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="c0846-127">Request body</span></span>
<span data-ttu-id="c0846-128">要求の本文に[roleScopeTag](../resources/intune-rbac-rolescopetag.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="c0846-128">In the request body, supply a JSON representation for the [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>

<span data-ttu-id="c0846-129">[RoleScopeTag](../resources/intune-rbac-rolescopetag.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="c0846-129">The following table shows the properties that are required when you create the [roleScopeTag](../resources/intune-rbac-rolescopetag.md).</span></span>

|<span data-ttu-id="c0846-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c0846-130">Property</span></span>|<span data-ttu-id="c0846-131">種類</span><span class="sxs-lookup"><span data-stu-id="c0846-131">Type</span></span>|<span data-ttu-id="c0846-132">説明</span><span class="sxs-lookup"><span data-stu-id="c0846-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c0846-133">ID</span><span class="sxs-lookup"><span data-stu-id="c0846-133">id</span></span>|<span data-ttu-id="c0846-134">String</span><span class="sxs-lookup"><span data-stu-id="c0846-134">String</span></span>|<span data-ttu-id="c0846-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="c0846-135">Key of the entity.</span></span> <span data-ttu-id="c0846-136">これは読み取り専用で、自動生成されます。</span><span class="sxs-lookup"><span data-stu-id="c0846-136">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="c0846-137">displayName</span><span class="sxs-lookup"><span data-stu-id="c0846-137">displayName</span></span>|<span data-ttu-id="c0846-138">String</span><span class="sxs-lookup"><span data-stu-id="c0846-138">String</span></span>|<span data-ttu-id="c0846-139">表示する、またはロールのスコープのタグの表示名。</span><span class="sxs-lookup"><span data-stu-id="c0846-139">The display or friendly name of the Role Scope Tag.</span></span>|
|<span data-ttu-id="c0846-140">説明</span><span class="sxs-lookup"><span data-stu-id="c0846-140">description</span></span>|<span data-ttu-id="c0846-141">String</span><span class="sxs-lookup"><span data-stu-id="c0846-141">String</span></span>|<span data-ttu-id="c0846-142">ロールのスコープのタグの説明です。</span><span class="sxs-lookup"><span data-stu-id="c0846-142">Description of the Role Scope Tag.</span></span>|



## <a name="response"></a><span data-ttu-id="c0846-143">応答</span><span class="sxs-lookup"><span data-stu-id="c0846-143">Response</span></span>
<span data-ttu-id="c0846-144">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[roleScopeTag](../resources/intune-rbac-rolescopetag.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="c0846-144">If successful, this method returns a `200 OK` response code and an updated [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c0846-145">例</span><span class="sxs-lookup"><span data-stu-id="c0846-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="c0846-146">要求</span><span class="sxs-lookup"><span data-stu-id="c0846-146">Request</span></span>
<span data-ttu-id="c0846-147">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c0846-147">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/roleScopeTags/{roleScopeTagId}
Content-type: application/json
Content-length: 82

{
  "displayName": "Display Name value",
  "description": "Description value"
}
```

### <a name="response"></a><span data-ttu-id="c0846-148">応答</span><span class="sxs-lookup"><span data-stu-id="c0846-148">Response</span></span>
<span data-ttu-id="c0846-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c0846-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 182

{
  "@odata.type": "#microsoft.graph.roleScopeTag",
  "id": "9ed1e179-e179-9ed1-79e1-d19e79e1d19e",
  "displayName": "Display Name value",
  "description": "Description value"
}
```





