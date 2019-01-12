---
title: deviceAndAppManagementRoleAssignments のリスト
description: deviceAndAppManagementRoleAssignment オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 4d6d583c440b73ef1fac3d84d130183116b14a21
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27991053"
---
# <a name="list-deviceandappmanagementroleassignments"></a><span data-ttu-id="5d158-103">deviceAndAppManagementRoleAssignments のリスト</span><span class="sxs-lookup"><span data-stu-id="5d158-103">List deviceAndAppManagementRoleAssignments</span></span>

> <span data-ttu-id="5d158-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5d158-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5d158-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5d158-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5d158-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="5d158-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5d158-107">[deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="5d158-107">List properties and relationships of the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5d158-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="5d158-108">Prerequisites</span></span>
<span data-ttu-id="5d158-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5d158-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5d158-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5d158-111">Permission type</span></span>|<span data-ttu-id="5d158-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="5d158-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5d158-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5d158-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5d158-114">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="5d158-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="5d158-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5d158-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5d158-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5d158-116">Not supported.</span></span>|
|<span data-ttu-id="5d158-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5d158-117">Application</span></span>|<span data-ttu-id="5d158-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5d158-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5d158-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5d158-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="5d158-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5d158-120">Request headers</span></span>
|<span data-ttu-id="5d158-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5d158-121">Header</span></span>|<span data-ttu-id="5d158-122">値</span><span class="sxs-lookup"><span data-stu-id="5d158-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5d158-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5d158-123">Authorization</span></span>|<span data-ttu-id="5d158-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="5d158-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5d158-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5d158-125">Accept</span></span>|<span data-ttu-id="5d158-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5d158-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5d158-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="5d158-127">Request body</span></span>
<span data-ttu-id="5d158-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="5d158-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5d158-129">応答</span><span class="sxs-lookup"><span data-stu-id="5d158-129">Response</span></span>
<span data-ttu-id="5d158-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="5d158-130">If successful, this method returns a `200 OK` response code and a collection of [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5d158-131">例</span><span class="sxs-lookup"><span data-stu-id="5d158-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="5d158-132">要求</span><span class="sxs-lookup"><span data-stu-id="5d158-132">Request</span></span>
<span data-ttu-id="5d158-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5d158-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/roleAssignments
```

### <a name="response"></a><span data-ttu-id="5d158-134">応答</span><span class="sxs-lookup"><span data-stu-id="5d158-134">Response</span></span>
<span data-ttu-id="5d158-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="5d158-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 480

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleAssignment",
      "id": "a12e8ebb-8ebb-a12e-bb8e-2ea1bb8e2ea1",
      "displayName": "Display Name value",
      "description": "Description value",
      "scopeMembers": [
        "Scope Members value"
      ],
      "scopeType": "allDevices",
      "resourceScopes": [
        "Resource Scopes value"
      ],
      "members": [
        "Members value"
      ]
    }
  ]
}
```





