---
title: deviceAndAppManagementRoleAssignments のリスト
description: deviceAndAppManagementRoleAssignment オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 13c8a3550c48bc1afa8b9bfcb686f27d5d445f55
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/11/2019
ms.locfileid: "31790131"
---
# <a name="list-deviceandappmanagementroleassignments"></a><span data-ttu-id="ba39a-103">deviceAndAppManagementRoleAssignments のリスト</span><span class="sxs-lookup"><span data-stu-id="ba39a-103">List deviceAndAppManagementRoleAssignments</span></span>

> <span data-ttu-id="ba39a-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ba39a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ba39a-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ba39a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ba39a-106">[deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="ba39a-106">List properties and relationships of the [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ba39a-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="ba39a-107">Prerequisites</span></span>
<span data-ttu-id="ba39a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ba39a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ba39a-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ba39a-110">Permission type</span></span>|<span data-ttu-id="ba39a-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ba39a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ba39a-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ba39a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ba39a-113">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="ba39a-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="ba39a-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ba39a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ba39a-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ba39a-115">Not supported.</span></span>|
|<span data-ttu-id="ba39a-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ba39a-116">Application</span></span>|<span data-ttu-id="ba39a-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ba39a-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ba39a-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ba39a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleAssignments
```

## <a name="request-headers"></a><span data-ttu-id="ba39a-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ba39a-119">Request headers</span></span>
|<span data-ttu-id="ba39a-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ba39a-120">Header</span></span>|<span data-ttu-id="ba39a-121">値</span><span class="sxs-lookup"><span data-stu-id="ba39a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ba39a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ba39a-122">Authorization</span></span>|<span data-ttu-id="ba39a-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="ba39a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ba39a-124">承諾</span><span class="sxs-lookup"><span data-stu-id="ba39a-124">Accept</span></span>|<span data-ttu-id="ba39a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ba39a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ba39a-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="ba39a-126">Request body</span></span>
<span data-ttu-id="ba39a-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ba39a-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ba39a-128">応答</span><span class="sxs-lookup"><span data-stu-id="ba39a-128">Response</span></span>
<span data-ttu-id="ba39a-129">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="ba39a-129">If successful, this method returns a `200 OK` response code and a collection of [deviceAndAppManagementRoleAssignment](../resources/intune-rbac-deviceandappmanagementroleassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ba39a-130">例</span><span class="sxs-lookup"><span data-stu-id="ba39a-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="ba39a-131">要求</span><span class="sxs-lookup"><span data-stu-id="ba39a-131">Request</span></span>
<span data-ttu-id="ba39a-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ba39a-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/roleAssignments
```

### <a name="response"></a><span data-ttu-id="ba39a-133">応答</span><span class="sxs-lookup"><span data-stu-id="ba39a-133">Response</span></span>
<span data-ttu-id="ba39a-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ba39a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





