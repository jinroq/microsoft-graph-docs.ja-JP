---
title: getAssignedRoleDetails 関数
description: 現在認証されているユーザーの割り当て済みのロール定義と役割の割り当てを取得します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0f3b3f843fe521e0a9cc94fa33ba94a4f76a3514
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "35002274"
---
# <a name="getassignedroledetails-function"></a><span data-ttu-id="60a57-103">getAssignedRoleDetails 関数</span><span class="sxs-lookup"><span data-stu-id="60a57-103">getAssignedRoleDetails function</span></span>

> <span data-ttu-id="60a57-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="60a57-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="60a57-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="60a57-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="60a57-106">現在認証されているユーザーの割り当て済みのロール定義と役割の割り当てを取得します。</span><span class="sxs-lookup"><span data-stu-id="60a57-106">Retrieves the assigned role definitions and role assignments of the currently authenticated user.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="60a57-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="60a57-107">Prerequisites</span></span>
<span data-ttu-id="60a57-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="60a57-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="60a57-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="60a57-110">Permission type</span></span>|<span data-ttu-id="60a57-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="60a57-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="60a57-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="60a57-112">Delegated (work or school account)</span></span>|<span data-ttu-id="60a57-113">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="60a57-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="60a57-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="60a57-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="60a57-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="60a57-115">Not supported.</span></span>|
|<span data-ttu-id="60a57-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="60a57-116">Application</span></span>|<span data-ttu-id="60a57-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="60a57-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="60a57-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="60a57-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getAssignedRoleDetails
```

## <a name="request-headers"></a><span data-ttu-id="60a57-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="60a57-119">Request headers</span></span>
|<span data-ttu-id="60a57-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="60a57-120">Header</span></span>|<span data-ttu-id="60a57-121">値</span><span class="sxs-lookup"><span data-stu-id="60a57-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="60a57-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="60a57-122">Authorization</span></span>|<span data-ttu-id="60a57-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="60a57-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="60a57-124">承諾</span><span class="sxs-lookup"><span data-stu-id="60a57-124">Accept</span></span>|<span data-ttu-id="60a57-125">application/json</span><span class="sxs-lookup"><span data-stu-id="60a57-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="60a57-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="60a57-126">Request body</span></span>
<span data-ttu-id="60a57-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="60a57-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="60a57-128">応答</span><span class="sxs-lookup"><span data-stu-id="60a57-128">Response</span></span>
<span data-ttu-id="60a57-129">成功した場合、この関数`200 OK`は応答コードと、応答本文で[deviceAndAppManagementAssignedRoleDetails](../resources/intune-rbac-deviceandappmanagementassignedroledetails.md)を返します。</span><span class="sxs-lookup"><span data-stu-id="60a57-129">If successful, this function returns a `200 OK` response code and a [deviceAndAppManagementAssignedRoleDetails](../resources/intune-rbac-deviceandappmanagementassignedroledetails.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="60a57-130">例</span><span class="sxs-lookup"><span data-stu-id="60a57-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="60a57-131">要求</span><span class="sxs-lookup"><span data-stu-id="60a57-131">Request</span></span>
<span data-ttu-id="60a57-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="60a57-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/getAssignedRoleDetails
```

### <a name="response"></a><span data-ttu-id="60a57-133">応答</span><span class="sxs-lookup"><span data-stu-id="60a57-133">Response</span></span>
<span data-ttu-id="60a57-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="60a57-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 245

{
  "value": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignedRoleDetails",
    "roleDefinitionIds": [
      "Role Definition Ids value"
    ],
    "roleAssignmentIds": [
      "Role Assignment Ids value"
    ]
  }
}
```




