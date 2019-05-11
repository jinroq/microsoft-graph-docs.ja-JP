---
title: getEffectivePermissions 関数
description: まだ文書化されていません
author: rolyon
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a1c2cb3ba99d89f2903fb417784cf08fdd1bd78f
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33898365"
---
# <a name="geteffectivepermissions-function"></a><span data-ttu-id="33b23-103">getEffectivePermissions 関数</span><span class="sxs-lookup"><span data-stu-id="33b23-103">getEffectivePermissions function</span></span>

> <span data-ttu-id="33b23-104">**重要:** Microsoft Graph の/ベータ版の Api は変更される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="33b23-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="33b23-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="33b23-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="33b23-106">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="33b23-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="33b23-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="33b23-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="33b23-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="33b23-108">Prerequisites</span></span>
<span data-ttu-id="33b23-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="33b23-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="33b23-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="33b23-111">Permission type</span></span>|<span data-ttu-id="33b23-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="33b23-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="33b23-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="33b23-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="33b23-114">&nbsp; &nbsp; **役割ベースのアクセス制御 (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="33b23-114">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="33b23-115">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="33b23-115">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="33b23-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="33b23-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="33b23-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="33b23-117">Not supported.</span></span>|
|<span data-ttu-id="33b23-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="33b23-118">Application</span></span>|<span data-ttu-id="33b23-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="33b23-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="33b23-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="33b23-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getEffectivePermissions
```

## <a name="request-headers"></a><span data-ttu-id="33b23-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="33b23-121">Request headers</span></span>
|<span data-ttu-id="33b23-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="33b23-122">Header</span></span>|<span data-ttu-id="33b23-123">値</span><span class="sxs-lookup"><span data-stu-id="33b23-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="33b23-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="33b23-124">Authorization</span></span>|<span data-ttu-id="33b23-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="33b23-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="33b23-126">承諾</span><span class="sxs-lookup"><span data-stu-id="33b23-126">Accept</span></span>|<span data-ttu-id="33b23-127">application/json</span><span class="sxs-lookup"><span data-stu-id="33b23-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="33b23-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="33b23-128">Request body</span></span>
<span data-ttu-id="33b23-129">要求 URL で、次のクエリ パラメーターに値を指定します。</span><span class="sxs-lookup"><span data-stu-id="33b23-129">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="33b23-130">次の表に、この関数で使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="33b23-130">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="33b23-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="33b23-131">Property</span></span>|<span data-ttu-id="33b23-132">型</span><span class="sxs-lookup"><span data-stu-id="33b23-132">Type</span></span>|<span data-ttu-id="33b23-133">説明</span><span class="sxs-lookup"><span data-stu-id="33b23-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="33b23-134">scope</span><span class="sxs-lookup"><span data-stu-id="33b23-134">scope</span></span>|<span data-ttu-id="33b23-135">String</span><span class="sxs-lookup"><span data-stu-id="33b23-135">String</span></span>|<span data-ttu-id="33b23-136">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="33b23-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="33b23-137">応答</span><span class="sxs-lookup"><span data-stu-id="33b23-137">Response</span></span>
<span data-ttu-id="33b23-138">成功した場合、この関数は `200 OK` 応答コードと、応答本文で [rolePermission](../resources/intune-rbac-rolepermission.md) コレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="33b23-138">If successful, this function returns a `200 OK` response code and a [rolePermission](../resources/intune-rbac-rolepermission.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="33b23-139">例</span><span class="sxs-lookup"><span data-stu-id="33b23-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="33b23-140">要求</span><span class="sxs-lookup"><span data-stu-id="33b23-140">Request</span></span>
<span data-ttu-id="33b23-141">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="33b23-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/getEffectivePermissions(scope='parameterValue')
```

### <a name="response"></a><span data-ttu-id="33b23-142">応答</span><span class="sxs-lookup"><span data-stu-id="33b23-142">Response</span></span>
<span data-ttu-id="33b23-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="33b23-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



