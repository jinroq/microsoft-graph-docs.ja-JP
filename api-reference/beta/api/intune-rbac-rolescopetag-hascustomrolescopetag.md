---
title: Hascustomロール Copetag 関数
description: まだ文書化されていません
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a77030ba3da40378e8ad1c18bc4e170767da8fbc
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35741431"
---
# <a name="hascustomrolescopetag-function"></a><span data-ttu-id="d0b73-103">Hascustomロール Copetag 関数</span><span class="sxs-lookup"><span data-stu-id="d0b73-103">hasCustomRoleScopeTag function</span></span>

> <span data-ttu-id="d0b73-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d0b73-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d0b73-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d0b73-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d0b73-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="d0b73-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d0b73-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="d0b73-107">Prerequisites</span></span>
<span data-ttu-id="d0b73-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d0b73-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d0b73-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d0b73-110">Permission type</span></span>|<span data-ttu-id="d0b73-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="d0b73-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d0b73-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d0b73-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d0b73-113">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="d0b73-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="d0b73-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d0b73-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d0b73-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d0b73-115">Not supported.</span></span>|
|<span data-ttu-id="d0b73-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d0b73-116">Application</span></span>|<span data-ttu-id="d0b73-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d0b73-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d0b73-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d0b73-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleScopeTags/hasCustomRoleScopeTag
GET /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/microsoft.graph.deviceAndAppManagementRoleAssignment/roleScopeTags/hasCustomRoleScopeTag
```

## <a name="request-headers"></a><span data-ttu-id="d0b73-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d0b73-119">Request headers</span></span>
|<span data-ttu-id="d0b73-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d0b73-120">Header</span></span>|<span data-ttu-id="d0b73-121">値</span><span class="sxs-lookup"><span data-stu-id="d0b73-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d0b73-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d0b73-122">Authorization</span></span>|<span data-ttu-id="d0b73-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="d0b73-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d0b73-124">承諾</span><span class="sxs-lookup"><span data-stu-id="d0b73-124">Accept</span></span>|<span data-ttu-id="d0b73-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d0b73-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d0b73-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="d0b73-126">Request body</span></span>
<span data-ttu-id="d0b73-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="d0b73-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d0b73-128">応答</span><span class="sxs-lookup"><span data-stu-id="d0b73-128">Response</span></span>
<span data-ttu-id="d0b73-129">成功した場合、この関数は `200 OK` 応答コードと、応答本文でブール値を返します。</span><span class="sxs-lookup"><span data-stu-id="d0b73-129">If successful, this function returns a `200 OK` response code and a Boolean in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d0b73-130">例</span><span class="sxs-lookup"><span data-stu-id="d0b73-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="d0b73-131">要求</span><span class="sxs-lookup"><span data-stu-id="d0b73-131">Request</span></span>
<span data-ttu-id="d0b73-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d0b73-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/roleScopeTags/hasCustomRoleScopeTag
```

### <a name="response"></a><span data-ttu-id="d0b73-133">応答</span><span class="sxs-lookup"><span data-stu-id="d0b73-133">Response</span></span>
<span data-ttu-id="d0b73-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d0b73-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 21

{
  "value": true
}
```





