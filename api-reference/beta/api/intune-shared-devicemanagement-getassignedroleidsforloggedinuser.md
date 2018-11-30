---
title: getAssignedRoleIdsForLoggedInUser 関数
description: 現在認証されているユーザーのロールの割り当てと割り当てられているロールの定義を取得します。
ms.openlocfilehash: c97e701bfd35961d9fb15022500bb06727c7e89a
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069026"
---
# <a name="getassignedroleidsforloggedinuser-function"></a><span data-ttu-id="df3fb-103">getAssignedRoleIdsForLoggedInUser 関数</span><span class="sxs-lookup"><span data-stu-id="df3fb-103">getAssignedRoleIdsForLoggedInUser function</span></span>

> <span data-ttu-id="df3fb-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="df3fb-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="df3fb-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="df3fb-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="df3fb-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="df3fb-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="df3fb-107">現在認証されているユーザーのロールの割り当てと割り当てられているロールの定義を取得します。</span><span class="sxs-lookup"><span data-stu-id="df3fb-107">Retrieves the assigned role definitions and role assignments of the currently authenticated user.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="df3fb-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="df3fb-108">Prerequisites</span></span>
<span data-ttu-id="df3fb-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="df3fb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="df3fb-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="df3fb-111">Permission type</span></span>|<span data-ttu-id="df3fb-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="df3fb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="df3fb-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="df3fb-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="df3fb-114">&nbsp;&nbsp; **ロール ベースのアクセス制御 (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="df3fb-114">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="df3fb-115">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="df3fb-115">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="df3fb-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="df3fb-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="df3fb-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="df3fb-117">Not supported.</span></span>|
|<span data-ttu-id="df3fb-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="df3fb-118">Application</span></span>|<span data-ttu-id="df3fb-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="df3fb-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="df3fb-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="df3fb-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getAssignedRoleIdsForLoggedInUser
```

## <a name="request-headers"></a><span data-ttu-id="df3fb-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="df3fb-121">Request headers</span></span>
|<span data-ttu-id="df3fb-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="df3fb-122">Header</span></span>|<span data-ttu-id="df3fb-123">値</span><span class="sxs-lookup"><span data-stu-id="df3fb-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="df3fb-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="df3fb-124">Authorization</span></span>|<span data-ttu-id="df3fb-125">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="df3fb-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="df3fb-126">Accept</span><span class="sxs-lookup"><span data-stu-id="df3fb-126">Accept</span></span>|<span data-ttu-id="df3fb-127">application/json</span><span class="sxs-lookup"><span data-stu-id="df3fb-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="df3fb-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="df3fb-128">Request body</span></span>
<span data-ttu-id="df3fb-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="df3fb-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="df3fb-130">応答</span><span class="sxs-lookup"><span data-stu-id="df3fb-130">Response</span></span>
<span data-ttu-id="df3fb-131">かどうかは成功すると、この関数を返します、`200 OK`応答コードおよび応答の本文には[deviceAndAppManagementAssignedRoleIds](../resources/intune-rbac-deviceandappmanagementassignedroleids.md)です。</span><span class="sxs-lookup"><span data-stu-id="df3fb-131">If successful, this function returns a `200 OK` response code and a [deviceAndAppManagementAssignedRoleIds](../resources/intune-rbac-deviceandappmanagementassignedroleids.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="df3fb-132">例</span><span class="sxs-lookup"><span data-stu-id="df3fb-132">Example</span></span>
### <a name="request"></a><span data-ttu-id="df3fb-133">要求</span><span class="sxs-lookup"><span data-stu-id="df3fb-133">Request</span></span>
<span data-ttu-id="df3fb-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="df3fb-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/getAssignedRoleIdsForLoggedInUser
```

### <a name="response"></a><span data-ttu-id="df3fb-135">応答</span><span class="sxs-lookup"><span data-stu-id="df3fb-135">Response</span></span>
<span data-ttu-id="df3fb-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="df3fb-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





