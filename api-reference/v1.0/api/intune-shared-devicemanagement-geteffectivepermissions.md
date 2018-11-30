---
title: getEffectivePermissions 関数
description: 現在の認証ユーザーの有効なアクセス許可を取得します
ms.openlocfilehash: 0d07045c4db64f6bb9418907cea618480d959522
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022688"
---
# <a name="geteffectivepermissions-function"></a><span data-ttu-id="4442c-103">getEffectivePermissions 関数</span><span class="sxs-lookup"><span data-stu-id="4442c-103">getEffectivePermissions function</span></span>

> <span data-ttu-id="4442c-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="4442c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4442c-105">現在の認証ユーザーの有効なアクセス許可を取得します</span><span class="sxs-lookup"><span data-stu-id="4442c-105">Retrieves the effective permissions of the currently authenticated user</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4442c-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="4442c-106">Prerequisites</span></span>
<span data-ttu-id="4442c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4442c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4442c-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4442c-109">Permission type</span></span>|<span data-ttu-id="4442c-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="4442c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4442c-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4442c-111">Delegated (work or school account)</span></span>||
| <span data-ttu-id="4442c-112">&nbsp;&nbsp;ロール ベースのアクセス制御</span><span class="sxs-lookup"><span data-stu-id="4442c-112">&nbsp; &nbsp; Role-based access control</span></span> | <span data-ttu-id="4442c-113">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="4442c-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="4442c-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4442c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4442c-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4442c-115">Not supported.</span></span>|
|<span data-ttu-id="4442c-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4442c-116">Application</span></span>|<span data-ttu-id="4442c-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4442c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4442c-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4442c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/getEffectivePermissions
```

## <a name="request-headers"></a><span data-ttu-id="4442c-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4442c-119">Request headers</span></span>
|<span data-ttu-id="4442c-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4442c-120">Header</span></span>|<span data-ttu-id="4442c-121">値</span><span class="sxs-lookup"><span data-stu-id="4442c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4442c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4442c-122">Authorization</span></span>|<span data-ttu-id="4442c-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="4442c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4442c-124">Accept</span><span class="sxs-lookup"><span data-stu-id="4442c-124">Accept</span></span>|<span data-ttu-id="4442c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4442c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4442c-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="4442c-126">Request body</span></span>
<span data-ttu-id="4442c-127">要求 URL で、次のクエリ パラメーターに値を指定します。</span><span class="sxs-lookup"><span data-stu-id="4442c-127">In the request URL, provide the following query parameters with values.</span></span>
<span data-ttu-id="4442c-128">次の表に、この関数で使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="4442c-128">The following table shows the parameters that can be used with this function.</span></span>

|<span data-ttu-id="4442c-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4442c-129">Property</span></span>|<span data-ttu-id="4442c-130">型</span><span class="sxs-lookup"><span data-stu-id="4442c-130">Type</span></span>|<span data-ttu-id="4442c-131">説明</span><span class="sxs-lookup"><span data-stu-id="4442c-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4442c-132">scope</span><span class="sxs-lookup"><span data-stu-id="4442c-132">scope</span></span>|<span data-ttu-id="4442c-133">String</span><span class="sxs-lookup"><span data-stu-id="4442c-133">String</span></span>|<span data-ttu-id="4442c-134">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="4442c-134">Not yet documented</span></span>|


## <a name="response"></a><span data-ttu-id="4442c-135">応答</span><span class="sxs-lookup"><span data-stu-id="4442c-135">Response</span></span>
<span data-ttu-id="4442c-136">成功した場合、この関数は `200 OK` 応答コードと、応答本文で [rolePermission](../resources/intune-rbac-rolepermission.md) コレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="4442c-136">If successful, this function returns a `200 OK` response code and a [rolePermission](../resources/intune-rbac-rolepermission.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4442c-137">例</span><span class="sxs-lookup"><span data-stu-id="4442c-137">Example</span></span>
### <a name="request"></a><span data-ttu-id="4442c-138">要求</span><span class="sxs-lookup"><span data-stu-id="4442c-138">Request</span></span>
<span data-ttu-id="4442c-139">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4442c-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/getEffectivePermissions(scope='parameterValue')
```

### <a name="response"></a><span data-ttu-id="4442c-140">応答</span><span class="sxs-lookup"><span data-stu-id="4442c-140">Response</span></span>
<span data-ttu-id="4442c-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4442c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



