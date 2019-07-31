---
title: getAssignedRoleIdsForLoggedInUser 関数
description: 現在認証されているユーザーの割り当て済みのロール定義と役割の割り当てを取得します。
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0279a09b5a017a4a7ea16ba45efc2bb5f5c8a3fd
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35993621"
---
# <a name="getassignedroleidsforloggedinuser-function"></a><span data-ttu-id="8c087-103">getAssignedRoleIdsForLoggedInUser 関数</span><span class="sxs-lookup"><span data-stu-id="8c087-103">getAssignedRoleIdsForLoggedInUser function</span></span>

> <span data-ttu-id="8c087-104">**重要:** Microsoft Graph の/ベータ版の Api は変更される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="8c087-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="8c087-105">実稼働アプリケーションでは、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8c087-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="8c087-106">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8c087-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8c087-107">現在認証されているユーザーの割り当て済みのロール定義と役割の割り当てを取得します。</span><span class="sxs-lookup"><span data-stu-id="8c087-107">Retrieves the assigned role definitions and role assignments of the currently authenticated user.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8c087-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="8c087-108">Prerequisites</span></span>
<span data-ttu-id="8c087-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8c087-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8c087-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8c087-111">Permission type</span></span>|<span data-ttu-id="8c087-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="8c087-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8c087-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8c087-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="8c087-114">&nbsp; &nbsp; **役割ベースのアクセス制御 (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="8c087-114">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="8c087-115">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="8c087-115">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="8c087-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8c087-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8c087-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8c087-117">Not supported.</span></span>|
|<span data-ttu-id="8c087-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8c087-118">Application</span></span>|<span data-ttu-id="8c087-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8c087-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8c087-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8c087-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getAssignedRoleIdsForLoggedInUser
```

## <a name="request-headers"></a><span data-ttu-id="8c087-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8c087-121">Request headers</span></span>
|<span data-ttu-id="8c087-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8c087-122">Header</span></span>|<span data-ttu-id="8c087-123">値</span><span class="sxs-lookup"><span data-stu-id="8c087-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8c087-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="8c087-124">Authorization</span></span>|<span data-ttu-id="8c087-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="8c087-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8c087-126">承諾</span><span class="sxs-lookup"><span data-stu-id="8c087-126">Accept</span></span>|<span data-ttu-id="8c087-127">application/json</span><span class="sxs-lookup"><span data-stu-id="8c087-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8c087-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="8c087-128">Request body</span></span>
<span data-ttu-id="8c087-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="8c087-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8c087-130">応答</span><span class="sxs-lookup"><span data-stu-id="8c087-130">Response</span></span>
<span data-ttu-id="8c087-131">成功した場合、この関数`200 OK`は応答コードと、応答本文で**deviceAndAppManagementAssignedRoleId**を返します。</span><span class="sxs-lookup"><span data-stu-id="8c087-131">If successful, this function returns a `200 OK` response code and a **deviceAndAppManagementAssignedRoleId** in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8c087-132">例</span><span class="sxs-lookup"><span data-stu-id="8c087-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="8c087-133">要求</span><span class="sxs-lookup"><span data-stu-id="8c087-133">Request</span></span>
<span data-ttu-id="8c087-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8c087-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/getAssignedRoleIdsForLoggedInUser
```

### <a name="response"></a><span data-ttu-id="8c087-135">応答</span><span class="sxs-lookup"><span data-stu-id="8c087-135">Response</span></span>
<span data-ttu-id="8c087-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8c087-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 263

{
  "value": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignedRoleIds",
    "roleDefinitionIds": [
      "df52f163-f163-df52-63f1-52df63f152df"
    ],
    "roleAssignmentIds": [
      "1f35d53d-d53d-1f35-3dd5-351f3dd5351f"
    ]
  }
}
```





