---
title: getEffectivePermissions 関数
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 04988c6ab4163021098da609782d7ac8e755af83
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29408440"
---
# <a name="geteffectivepermissions-function"></a><span data-ttu-id="a2ae1-103">getEffectivePermissions 関数</span><span class="sxs-lookup"><span data-stu-id="a2ae1-103">getEffectivePermissions function</span></span>

> <span data-ttu-id="a2ae1-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a2ae1-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a2ae1-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a2ae1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a2ae1-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a2ae1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a2ae1-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="a2ae1-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a2ae1-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="a2ae1-108">Prerequisites</span></span>
<span data-ttu-id="a2ae1-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a2ae1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a2ae1-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a2ae1-111">Permission type</span></span>|<span data-ttu-id="a2ae1-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a2ae1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a2ae1-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a2ae1-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="a2ae1-114">&nbsp;&nbsp; **ロール ベースのアクセス制御 (RBAC)**</span><span class="sxs-lookup"><span data-stu-id="a2ae1-114">&nbsp; &nbsp; **Role-based access control (RBAC)**</span></span> | <span data-ttu-id="a2ae1-115">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="a2ae1-115">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="a2ae1-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a2ae1-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a2ae1-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a2ae1-117">Not supported.</span></span>|
|<span data-ttu-id="a2ae1-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a2ae1-118">Application</span></span>|<span data-ttu-id="a2ae1-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a2ae1-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a2ae1-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a2ae1-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getEffectivePermissions
```

## <a name="request-headers"></a><span data-ttu-id="a2ae1-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a2ae1-121">Request headers</span></span>
|<span data-ttu-id="a2ae1-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a2ae1-122">Header</span></span>|<span data-ttu-id="a2ae1-123">値</span><span class="sxs-lookup"><span data-stu-id="a2ae1-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a2ae1-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="a2ae1-124">Authorization</span></span>|<span data-ttu-id="a2ae1-125">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="a2ae1-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a2ae1-126">Accept</span><span class="sxs-lookup"><span data-stu-id="a2ae1-126">Accept</span></span>|<span data-ttu-id="a2ae1-127">application/json</span><span class="sxs-lookup"><span data-stu-id="a2ae1-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a2ae1-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="a2ae1-128">Request body</span></span>
<span data-ttu-id="a2ae1-129">要求 URL で、次のクエリ パラメーターに値を指定します。</span><span class="sxs-lookup"><span data-stu-id="a2ae1-129">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="a2ae1-130">次の表に、この関数で使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="a2ae1-130">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="a2ae1-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a2ae1-131">Property</span></span>|<span data-ttu-id="a2ae1-132">型</span><span class="sxs-lookup"><span data-stu-id="a2ae1-132">Type</span></span>|<span data-ttu-id="a2ae1-133">説明</span><span class="sxs-lookup"><span data-stu-id="a2ae1-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2ae1-134">scope</span><span class="sxs-lookup"><span data-stu-id="a2ae1-134">scope</span></span>|<span data-ttu-id="a2ae1-135">String</span><span class="sxs-lookup"><span data-stu-id="a2ae1-135">String</span></span>|<span data-ttu-id="a2ae1-136">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="a2ae1-136">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="a2ae1-137">応答</span><span class="sxs-lookup"><span data-stu-id="a2ae1-137">Response</span></span>
<span data-ttu-id="a2ae1-138">成功した場合、この関数は `200 OK` 応答コードと、応答本文で [rolePermission](../resources/intune-rbac-rolepermission.md) コレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="a2ae1-138">If successful, this function returns a `200 OK` response code and a [rolePermission](../resources/intune-rbac-rolepermission.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a2ae1-139">例</span><span class="sxs-lookup"><span data-stu-id="a2ae1-139">Example</span></span>
### <a name="request"></a><span data-ttu-id="a2ae1-140">要求</span><span class="sxs-lookup"><span data-stu-id="a2ae1-140">Request</span></span>
<span data-ttu-id="a2ae1-141">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a2ae1-141">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/getEffectivePermissions(scope='parameterValue')
```

### <a name="response"></a><span data-ttu-id="a2ae1-142">応答</span><span class="sxs-lookup"><span data-stu-id="a2ae1-142">Response</span></span>
<span data-ttu-id="a2ae1-p104">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a2ae1-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



