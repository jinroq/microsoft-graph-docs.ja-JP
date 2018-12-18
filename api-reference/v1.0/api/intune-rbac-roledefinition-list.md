---
title: roleDefinitions のリスト
description: roleDefinition オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
ms.openlocfilehash: 2aa23644d075c03aeb5b19551672214f15e0f4bd
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27319650"
---
# <a name="list-roledefinitions"></a><span data-ttu-id="cd657-103">roleDefinitions のリスト</span><span class="sxs-lookup"><span data-stu-id="cd657-103">List roleDefinitions</span></span>

> <span data-ttu-id="cd657-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="cd657-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cd657-105">[roleDefinition](../resources/intune-rbac-roledefinition.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="cd657-105">List properties and relationships of the [roleDefinition](../resources/intune-rbac-roledefinition.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cd657-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="cd657-106">Prerequisites</span></span>
<span data-ttu-id="cd657-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cd657-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cd657-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cd657-109">Permission type</span></span>|<span data-ttu-id="cd657-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="cd657-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cd657-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cd657-111">Delegated (work or school account)</span></span>|<span data-ttu-id="cd657-112">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="cd657-112">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="cd657-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cd657-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cd657-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cd657-114">Not supported.</span></span>|
|<span data-ttu-id="cd657-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cd657-115">Application</span></span>|<span data-ttu-id="cd657-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cd657-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cd657-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cd657-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="cd657-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cd657-118">Request headers</span></span>
|<span data-ttu-id="cd657-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cd657-119">Header</span></span>|<span data-ttu-id="cd657-120">値</span><span class="sxs-lookup"><span data-stu-id="cd657-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cd657-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="cd657-121">Authorization</span></span>|<span data-ttu-id="cd657-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="cd657-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cd657-123">Accept</span><span class="sxs-lookup"><span data-stu-id="cd657-123">Accept</span></span>|<span data-ttu-id="cd657-124">application/json</span><span class="sxs-lookup"><span data-stu-id="cd657-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cd657-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="cd657-125">Request body</span></span>
<span data-ttu-id="cd657-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="cd657-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cd657-127">応答</span><span class="sxs-lookup"><span data-stu-id="cd657-127">Response</span></span>
<span data-ttu-id="cd657-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [roleDefinition](../resources/intune-rbac-roledefinition.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="cd657-128">If successful, this method returns a `200 OK` response code and a collection of [roleDefinition](../resources/intune-rbac-roledefinition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cd657-129">例</span><span class="sxs-lookup"><span data-stu-id="cd657-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="cd657-130">要求</span><span class="sxs-lookup"><span data-stu-id="cd657-130">Request</span></span>
<span data-ttu-id="cd657-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="cd657-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/roleDefinitions
```

### <a name="response"></a><span data-ttu-id="cd657-132">応答</span><span class="sxs-lookup"><span data-stu-id="cd657-132">Response</span></span>
<span data-ttu-id="cd657-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="cd657-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 746

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.roleDefinition",
      "id": "70fdcd08-cd08-70fd-08cd-fd7008cdfd70",
      "displayName": "Display Name value",
      "description": "Description value",
      "rolePermissions": [
        {
          "@odata.type": "microsoft.graph.rolePermission",
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
      ],
      "isBuiltIn": true
    }
  ]
}
```



