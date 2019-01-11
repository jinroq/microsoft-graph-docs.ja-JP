---
title: getEffectivePermissions 関数
description: 現在の認証ユーザーの有効なアクセス許可を取得します
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5c887aebdba69048ded387371ad2534ce4173668
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27850779"
---
# <a name="geteffectivepermissions-function"></a><span data-ttu-id="e2800-103">getEffectivePermissions 関数</span><span class="sxs-lookup"><span data-stu-id="e2800-103">getEffectivePermissions function</span></span>

> <span data-ttu-id="e2800-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e2800-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e2800-105">現在の認証ユーザーの有効なアクセス許可を取得します</span><span class="sxs-lookup"><span data-stu-id="e2800-105">Retrieves the effective permissions of the currently authenticated user</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e2800-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="e2800-106">Prerequisites</span></span>
<span data-ttu-id="e2800-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e2800-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2800-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e2800-109">Permission type</span></span>|<span data-ttu-id="e2800-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="e2800-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e2800-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e2800-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="e2800-112">&nbsp;&nbsp;ロール ベースのアクセス制御</span><span class="sxs-lookup"><span data-stu-id="e2800-112">&nbsp; &nbsp; Role-based access control</span></span> | <span data-ttu-id="e2800-113">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="e2800-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="e2800-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e2800-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e2800-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e2800-115">Not supported.</span></span>|
|<span data-ttu-id="e2800-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e2800-116">Application</span></span>|<span data-ttu-id="e2800-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e2800-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e2800-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e2800-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getEffectivePermissions
```

## <a name="request-headers"></a><span data-ttu-id="e2800-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e2800-119">Request headers</span></span>
|<span data-ttu-id="e2800-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e2800-120">Header</span></span>|<span data-ttu-id="e2800-121">値</span><span class="sxs-lookup"><span data-stu-id="e2800-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e2800-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e2800-122">Authorization</span></span>|<span data-ttu-id="e2800-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="e2800-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e2800-124">Accept</span><span class="sxs-lookup"><span data-stu-id="e2800-124">Accept</span></span>|<span data-ttu-id="e2800-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e2800-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e2800-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="e2800-126">Request body</span></span>
<span data-ttu-id="e2800-127">要求 URL で、次のクエリ パラメーターに値を指定します。</span><span class="sxs-lookup"><span data-stu-id="e2800-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="e2800-128">次の表に、この関数で使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="e2800-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="e2800-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e2800-129">Property</span></span>|<span data-ttu-id="e2800-130">種類</span><span class="sxs-lookup"><span data-stu-id="e2800-130">Type</span></span>|<span data-ttu-id="e2800-131">説明</span><span class="sxs-lookup"><span data-stu-id="e2800-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e2800-132">scope</span><span class="sxs-lookup"><span data-stu-id="e2800-132">scope</span></span>|<span data-ttu-id="e2800-133">String</span><span class="sxs-lookup"><span data-stu-id="e2800-133">String</span></span>|<span data-ttu-id="e2800-134">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="e2800-134">Not yet documented</span></span>|


## <a name="response"></a><span data-ttu-id="e2800-135">応答</span><span class="sxs-lookup"><span data-stu-id="e2800-135">Response</span></span>
<span data-ttu-id="e2800-136">成功した場合、この関数は `200 OK` 応答コードと、応答本文で [rolePermission](../resources/intune-rbac-rolepermission.md) コレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="e2800-136">If successful, this function returns a `200 OK` response code and a [rolePermission](../resources/intune-rbac-rolepermission.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e2800-137">例</span><span class="sxs-lookup"><span data-stu-id="e2800-137">Example</span></span>
### <a name="request"></a><span data-ttu-id="e2800-138">要求</span><span class="sxs-lookup"><span data-stu-id="e2800-138">Request</span></span>
<span data-ttu-id="e2800-139">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e2800-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/getEffectivePermissions(scope='parameterValue')
```

### <a name="response"></a><span data-ttu-id="e2800-140">応答</span><span class="sxs-lookup"><span data-stu-id="e2800-140">Response</span></span>
<span data-ttu-id="e2800-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e2800-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



