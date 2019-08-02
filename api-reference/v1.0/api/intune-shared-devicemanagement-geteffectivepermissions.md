---
title: getEffectivePermissions 関数
description: 現在の認証ユーザーの有効なアクセス許可を取得します
author: tfitzmac
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3609bb419b9fc7bf39074827915717428224443b
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36025887"
---
# <a name="geteffectivepermissions-function"></a><span data-ttu-id="fffee-103">getEffectivePermissions 関数</span><span class="sxs-lookup"><span data-stu-id="fffee-103">getEffectivePermissions function</span></span>

> <span data-ttu-id="fffee-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="fffee-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fffee-105">現在の認証ユーザーの有効なアクセス許可を取得します</span><span class="sxs-lookup"><span data-stu-id="fffee-105">Retrieves the effective permissions of the currently authenticated user</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fffee-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="fffee-106">Prerequisites</span></span>
<span data-ttu-id="fffee-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fffee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fffee-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fffee-109">Permission type</span></span>|<span data-ttu-id="fffee-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="fffee-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fffee-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fffee-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="fffee-112">&nbsp;&nbsp;役割ベースのアクセス制御</span><span class="sxs-lookup"><span data-stu-id="fffee-112">&nbsp; &nbsp; Role-based access control</span></span> | <span data-ttu-id="fffee-113">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="fffee-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="fffee-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fffee-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fffee-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fffee-115">Not supported.</span></span>|
|<span data-ttu-id="fffee-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fffee-116">Application</span></span>|<span data-ttu-id="fffee-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fffee-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fffee-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fffee-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getEffectivePermissions
```

## <a name="request-headers"></a><span data-ttu-id="fffee-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fffee-119">Request headers</span></span>
|<span data-ttu-id="fffee-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fffee-120">Header</span></span>|<span data-ttu-id="fffee-121">値</span><span class="sxs-lookup"><span data-stu-id="fffee-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fffee-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="fffee-122">Authorization</span></span>|<span data-ttu-id="fffee-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="fffee-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fffee-124">承諾</span><span class="sxs-lookup"><span data-stu-id="fffee-124">Accept</span></span>|<span data-ttu-id="fffee-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fffee-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fffee-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="fffee-126">Request body</span></span>
<span data-ttu-id="fffee-127">要求 URL で、次のクエリ パラメーターに値を指定します。</span><span class="sxs-lookup"><span data-stu-id="fffee-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="fffee-128">次の表に、この関数で使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="fffee-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="fffee-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fffee-129">Property</span></span>|<span data-ttu-id="fffee-130">型</span><span class="sxs-lookup"><span data-stu-id="fffee-130">Type</span></span>|<span data-ttu-id="fffee-131">説明</span><span class="sxs-lookup"><span data-stu-id="fffee-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fffee-132">scope</span><span class="sxs-lookup"><span data-stu-id="fffee-132">scope</span></span>|<span data-ttu-id="fffee-133">String</span><span class="sxs-lookup"><span data-stu-id="fffee-133">String</span></span>|<span data-ttu-id="fffee-134">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="fffee-134">Not yet documented</span></span>|


## <a name="response"></a><span data-ttu-id="fffee-135">応答</span><span class="sxs-lookup"><span data-stu-id="fffee-135">Response</span></span>
<span data-ttu-id="fffee-136">成功した場合、この関数は `200 OK` 応答コードと、応答本文で [rolePermission](../resources/intune-rbac-rolepermission.md) コレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="fffee-136">If successful, this function returns a `200 OK` response code and a [rolePermission](../resources/intune-rbac-rolepermission.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fffee-137">例</span><span class="sxs-lookup"><span data-stu-id="fffee-137">Example</span></span>
### <a name="request"></a><span data-ttu-id="fffee-138">要求</span><span class="sxs-lookup"><span data-stu-id="fffee-138">Request</span></span>
<span data-ttu-id="fffee-139">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="fffee-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/getEffectivePermissions(scope='parameterValue')
```

### <a name="response"></a><span data-ttu-id="fffee-140">応答</span><span class="sxs-lookup"><span data-stu-id="fffee-140">Response</span></span>
<span data-ttu-id="fffee-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="fffee-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



