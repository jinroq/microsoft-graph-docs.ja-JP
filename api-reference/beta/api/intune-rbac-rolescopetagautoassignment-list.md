---
title: ロールの Copetagautoassignments を一覧表示する
description: ロール Copetagautoassignment オブジェクトのプロパティとリレーションシップをリストします。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 57c26411158bc9b7ae147f31fedaa3fadded175c
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36347633"
---
# <a name="list-rolescopetagautoassignments"></a><span data-ttu-id="97944-103">ロールの Copetagautoassignments を一覧表示する</span><span class="sxs-lookup"><span data-stu-id="97944-103">List roleScopeTagAutoAssignments</span></span>

> <span data-ttu-id="97944-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="97944-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="97944-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="97944-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="97944-106">[ロール Copetagautoassignment](../resources/intune-rbac-rolescopetagautoassignment.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="97944-106">List properties and relationships of the [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="97944-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="97944-107">Prerequisites</span></span>
<span data-ttu-id="97944-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="97944-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="97944-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="97944-110">Permission type</span></span>|<span data-ttu-id="97944-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="97944-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="97944-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="97944-112">Delegated (work or school account)</span></span>|<span data-ttu-id="97944-113">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="97944-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="97944-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="97944-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="97944-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="97944-115">Not supported.</span></span>|
|<span data-ttu-id="97944-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="97944-116">Application</span></span>|<span data-ttu-id="97944-117">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="97944-117">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="97944-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="97944-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/{roleScopeTagId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="97944-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="97944-119">Request headers</span></span>
|<span data-ttu-id="97944-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="97944-120">Header</span></span>|<span data-ttu-id="97944-121">値</span><span class="sxs-lookup"><span data-stu-id="97944-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="97944-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="97944-122">Authorization</span></span>|<span data-ttu-id="97944-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="97944-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="97944-124">承諾</span><span class="sxs-lookup"><span data-stu-id="97944-124">Accept</span></span>|<span data-ttu-id="97944-125">application/json</span><span class="sxs-lookup"><span data-stu-id="97944-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="97944-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="97944-126">Request body</span></span>
<span data-ttu-id="97944-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="97944-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="97944-128">応答</span><span class="sxs-lookup"><span data-stu-id="97944-128">Response</span></span>
<span data-ttu-id="97944-129">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で、[ロール Copetagautoassignment](../resources/intune-rbac-rolescopetagautoassignment.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="97944-129">If successful, this method returns a `200 OK` response code and a collection of [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="97944-130">例</span><span class="sxs-lookup"><span data-stu-id="97944-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="97944-131">要求</span><span class="sxs-lookup"><span data-stu-id="97944-131">Request</span></span>
<span data-ttu-id="97944-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="97944-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/{roleScopeTagId}/assignments
```

### <a name="response"></a><span data-ttu-id="97944-133">応答</span><span class="sxs-lookup"><span data-stu-id="97944-133">Response</span></span>
<span data-ttu-id="97944-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="97944-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 268

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.roleScopeTagAutoAssignment",
      "id": "256e6375-6375-256e-7563-6e2575636e25",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```






