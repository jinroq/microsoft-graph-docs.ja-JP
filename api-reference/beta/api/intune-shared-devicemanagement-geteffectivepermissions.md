---
title: getEffectivePermissions 関数
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: f0eca9494d98ca1e572d80eac6957c49f07ea702
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27868027"
---
# <a name="geteffectivepermissions-function"></a><span data-ttu-id="9e1bf-103">getEffectivePermissions 関数</span><span class="sxs-lookup"><span data-stu-id="9e1bf-103">getEffectivePermissions function</span></span>

> <span data-ttu-id="9e1bf-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="9e1bf-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="9e1bf-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9e1bf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="9e1bf-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="9e1bf-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9e1bf-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="9e1bf-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9e1bf-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="9e1bf-108">Prerequisites</span></span>
<span data-ttu-id="9e1bf-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="9e1bf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9e1bf-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="9e1bf-111">Permission type</span></span>|<span data-ttu-id="9e1bf-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="9e1bf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9e1bf-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="9e1bf-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="9e1bf-114">&nbsp;&nbsp; **ロール ベースのアクセス制御 (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="9e1bf-114">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="9e1bf-115">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="9e1bf-115">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="9e1bf-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="9e1bf-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9e1bf-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9e1bf-117">Not supported.</span></span>|
|<span data-ttu-id="9e1bf-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="9e1bf-118">Application</span></span>|<span data-ttu-id="9e1bf-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="9e1bf-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9e1bf-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="9e1bf-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getEffectivePermissions
```

## <a name="request-headers"></a><span data-ttu-id="9e1bf-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9e1bf-121">Request headers</span></span>
|<span data-ttu-id="9e1bf-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9e1bf-122">Header</span></span>|<span data-ttu-id="9e1bf-123">値</span><span class="sxs-lookup"><span data-stu-id="9e1bf-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9e1bf-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="9e1bf-124">Authorization</span></span>|<span data-ttu-id="9e1bf-125">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="9e1bf-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9e1bf-126">Accept</span><span class="sxs-lookup"><span data-stu-id="9e1bf-126">Accept</span></span>|<span data-ttu-id="9e1bf-127">application/json</span><span class="sxs-lookup"><span data-stu-id="9e1bf-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9e1bf-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="9e1bf-128">Request body</span></span>
<span data-ttu-id="9e1bf-129">要求 URL で、次のクエリ パラメーターに値を指定します。</span><span class="sxs-lookup"><span data-stu-id="9e1bf-129">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="9e1bf-130">次の表に、この関数で使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="9e1bf-130">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="9e1bf-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9e1bf-131">Property</span></span>|<span data-ttu-id="9e1bf-132">種類</span><span class="sxs-lookup"><span data-stu-id="9e1bf-132">Type</span></span>|<span data-ttu-id="9e1bf-133">説明</span><span class="sxs-lookup"><span data-stu-id="9e1bf-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9e1bf-134">scope</span><span class="sxs-lookup"><span data-stu-id="9e1bf-134">scope</span></span>|<span data-ttu-id="9e1bf-135">String</span><span class="sxs-lookup"><span data-stu-id="9e1bf-135">String</span></span>|<span data-ttu-id="9e1bf-136">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="9e1bf-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="9e1bf-137">応答</span><span class="sxs-lookup"><span data-stu-id="9e1bf-137">Response</span></span>
<span data-ttu-id="9e1bf-138">成功した場合、この関数は `200 OK` 応答コードと、応答本文で [rolePermission](../resources/intune-rbac-rolepermission.md) コレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="9e1bf-138">If successful, this function returns a `200 OK` response code and a [rolePermission](../resources/intune-rbac-rolepermission.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9e1bf-139">例</span><span class="sxs-lookup"><span data-stu-id="9e1bf-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="9e1bf-140">要求</span><span class="sxs-lookup"><span data-stu-id="9e1bf-140">Request</span></span>
<span data-ttu-id="9e1bf-141">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="9e1bf-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/getEffectivePermissions(scope='parameterValue')
```

### <a name="response"></a><span data-ttu-id="9e1bf-142">応答</span><span class="sxs-lookup"><span data-stu-id="9e1bf-142">Response</span></span>
<span data-ttu-id="9e1bf-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="9e1bf-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 471

{
  "value": [
    {
      "@odata.type": "microsoft.graph.rolePermission",
      "actions": [
        "Actions value"
      ],
      "resourceActions": [
        {
          "@odata.type": "microsoft.graph.resourceAction",
          "allowedResourceActions": [
            "Allowed Resource Actions value"
          ],
          "notAllowedResourceActions": [
            "Not Allowed Resource Actions value"
          ]
        }
      ]
    }
  ]
}
```



