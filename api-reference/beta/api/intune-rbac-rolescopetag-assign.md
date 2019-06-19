---
title: assign アクション
description: まだ文書化されていません
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a259fd1f36fc61ce918a7082e03c6af97a61e002
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "35002057"
---
# <a name="assign-action"></a><span data-ttu-id="4c243-103">アクションの割り当て</span><span class="sxs-lookup"><span data-stu-id="4c243-103">assign action</span></span>

> <span data-ttu-id="4c243-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4c243-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4c243-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4c243-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4c243-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="4c243-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4c243-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="4c243-107">Prerequisites</span></span>
<span data-ttu-id="4c243-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4c243-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4c243-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4c243-110">Permission type</span></span>|<span data-ttu-id="4c243-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="4c243-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4c243-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4c243-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4c243-113">DeviceManagementRBAC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c243-113">DeviceManagementRBAC.ReadWrite.All</span></span>|
|<span data-ttu-id="4c243-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4c243-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4c243-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4c243-115">Not supported.</span></span>|
|<span data-ttu-id="4c243-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4c243-116">Application</span></span>|<span data-ttu-id="4c243-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4c243-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4c243-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4c243-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/roleScopeTags/{roleScopeTagId}/assign
POST /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/{roleScopeTagId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="4c243-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4c243-119">Request headers</span></span>
|<span data-ttu-id="4c243-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4c243-120">Header</span></span>|<span data-ttu-id="4c243-121">値</span><span class="sxs-lookup"><span data-stu-id="4c243-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4c243-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4c243-122">Authorization</span></span>|<span data-ttu-id="4c243-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="4c243-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4c243-124">承諾</span><span class="sxs-lookup"><span data-stu-id="4c243-124">Accept</span></span>|<span data-ttu-id="4c243-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4c243-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4c243-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="4c243-126">Request body</span></span>
<span data-ttu-id="4c243-127">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="4c243-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="4c243-128">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="4c243-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="4c243-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4c243-129">Property</span></span>|<span data-ttu-id="4c243-130">型</span><span class="sxs-lookup"><span data-stu-id="4c243-130">Type</span></span>|<span data-ttu-id="4c243-131">説明</span><span class="sxs-lookup"><span data-stu-id="4c243-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4c243-132">assignments</span><span class="sxs-lookup"><span data-stu-id="4c243-132">assignments</span></span>|<span data-ttu-id="4c243-133">[ロール Copetagautoassignment](../resources/intune-rbac-rolescopetagautoassignment.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="4c243-133">[roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) collection</span></span>|<span data-ttu-id="4c243-134">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="4c243-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="4c243-135">応答</span><span class="sxs-lookup"><span data-stu-id="4c243-135">Response</span></span>
<span data-ttu-id="4c243-136">成功した場合、このアクション`200 OK`は応答コードと、応答本文で、[ロール Copetagautoassignment](../resources/intune-rbac-rolescopetagautoassignment.md)コレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="4c243-136">If successful, this action returns a `200 OK` response code and a [roleScopeTagAutoAssignment](../resources/intune-rbac-rolescopetagautoassignment.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4c243-137">例</span><span class="sxs-lookup"><span data-stu-id="4c243-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="4c243-138">要求</span><span class="sxs-lookup"><span data-stu-id="4c243-138">Request</span></span>
<span data-ttu-id="4c243-139">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4c243-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/roleScopeTags/{roleScopeTagId}/assign

Content-type: application/json
Content-length: 274

{
  "assignments": [
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

### <a name="response"></a><span data-ttu-id="4c243-140">応答</span><span class="sxs-lookup"><span data-stu-id="4c243-140">Response</span></span>
<span data-ttu-id="4c243-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4c243-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




