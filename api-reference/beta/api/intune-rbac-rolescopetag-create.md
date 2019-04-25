---
title: ロール copetag の作成
description: 新しいロール copetag オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9c542d62ffb4f05de37569e45aae8bbcc90a1ac7
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32527309"
---
# <a name="create-rolescopetag"></a><span data-ttu-id="884be-103">ロール copetag の作成</span><span class="sxs-lookup"><span data-stu-id="884be-103">Create roleScopeTag</span></span>

> <span data-ttu-id="884be-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="884be-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="884be-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="884be-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="884be-106">新しい[ロール copetag](../resources/intune-rbac-rolescopetag.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="884be-106">Create a new [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="884be-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="884be-107">Prerequisites</span></span>
<span data-ttu-id="884be-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="884be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="884be-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="884be-110">Permission type</span></span>|<span data-ttu-id="884be-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="884be-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="884be-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="884be-112">Delegated (work or school account)</span></span>|<span data-ttu-id="884be-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="884be-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="884be-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="884be-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="884be-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="884be-115">Not supported.</span></span>|
|<span data-ttu-id="884be-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="884be-116">Application</span></span>|<span data-ttu-id="884be-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="884be-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="884be-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="884be-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleScopeTags
POST /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags
```

## <a name="request-headers"></a><span data-ttu-id="884be-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="884be-119">Request headers</span></span>
|<span data-ttu-id="884be-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="884be-120">Header</span></span>|<span data-ttu-id="884be-121">値</span><span class="sxs-lookup"><span data-stu-id="884be-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="884be-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="884be-122">Authorization</span></span>|<span data-ttu-id="884be-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="884be-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="884be-124">承諾</span><span class="sxs-lookup"><span data-stu-id="884be-124">Accept</span></span>|<span data-ttu-id="884be-125">application/json</span><span class="sxs-lookup"><span data-stu-id="884be-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="884be-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="884be-126">Request body</span></span>
<span data-ttu-id="884be-127">要求本文で、ロール copetag オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="884be-127">In the request body, supply a JSON representation for the roleScopeTag object.</span></span>

<span data-ttu-id="884be-128">次の表に、ロール copetag の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="884be-128">The following table shows the properties that are required when you create the roleScopeTag.</span></span>

|<span data-ttu-id="884be-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="884be-129">Property</span></span>|<span data-ttu-id="884be-130">型</span><span class="sxs-lookup"><span data-stu-id="884be-130">Type</span></span>|<span data-ttu-id="884be-131">説明</span><span class="sxs-lookup"><span data-stu-id="884be-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="884be-132">id</span><span class="sxs-lookup"><span data-stu-id="884be-132">id</span></span>|<span data-ttu-id="884be-133">String</span><span class="sxs-lookup"><span data-stu-id="884be-133">String</span></span>|<span data-ttu-id="884be-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="884be-134">Key of the entity.</span></span> <span data-ttu-id="884be-135">これは読み取り専用で、自動生成されます。</span><span class="sxs-lookup"><span data-stu-id="884be-135">This is read-only and automatically generated.</span></span>|
|<span data-ttu-id="884be-136">displayName</span><span class="sxs-lookup"><span data-stu-id="884be-136">displayName</span></span>|<span data-ttu-id="884be-137">String</span><span class="sxs-lookup"><span data-stu-id="884be-137">String</span></span>|<span data-ttu-id="884be-138">ロールスコープタグの表示名またはフレンドリ名。</span><span class="sxs-lookup"><span data-stu-id="884be-138">The display or friendly name of the Role Scope Tag.</span></span>|
|<span data-ttu-id="884be-139">description</span><span class="sxs-lookup"><span data-stu-id="884be-139">description</span></span>|<span data-ttu-id="884be-140">String</span><span class="sxs-lookup"><span data-stu-id="884be-140">String</span></span>|<span data-ttu-id="884be-141">役割の範囲タグの説明。</span><span class="sxs-lookup"><span data-stu-id="884be-141">Description of the Role Scope Tag.</span></span>|



## <a name="response"></a><span data-ttu-id="884be-142">応答</span><span class="sxs-lookup"><span data-stu-id="884be-142">Response</span></span>
<span data-ttu-id="884be-143">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[ロール copetag](../resources/intune-rbac-rolescopetag.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="884be-143">If successful, this method returns a `201 Created` response code and a [roleScopeTag](../resources/intune-rbac-rolescopetag.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="884be-144">例</span><span class="sxs-lookup"><span data-stu-id="884be-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="884be-145">要求</span><span class="sxs-lookup"><span data-stu-id="884be-145">Request</span></span>
<span data-ttu-id="884be-146">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="884be-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/roleScopeTags
Content-type: application/json
Content-length: 133

{
  "@odata.type": "#microsoft.graph.roleScopeTag",
  "displayName": "Display Name value",
  "description": "Description value"
}
```

### <a name="response"></a><span data-ttu-id="884be-147">応答</span><span class="sxs-lookup"><span data-stu-id="884be-147">Response</span></span>
<span data-ttu-id="884be-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="884be-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 182

{
  "@odata.type": "#microsoft.graph.roleScopeTag",
  "id": "9ed1e179-e179-9ed1-79e1-d19e79e1d19e",
  "displayName": "Display Name value",
  "description": "Description value"
}
```





