---
title: roleDefinitions のリスト
description: roleDefinition オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 117ee436ad63d0d28654935ab0271ff3700821b6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27837703"
---
# <a name="list-roledefinitions"></a><span data-ttu-id="7cb95-103">roleDefinitions のリスト</span><span class="sxs-lookup"><span data-stu-id="7cb95-103">List roleDefinitions</span></span>

> <span data-ttu-id="7cb95-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="7cb95-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7cb95-105">[roleDefinition](../resources/intune-rbac-roledefinition.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="7cb95-105">List properties and relationships of the [roleDefinition](../resources/intune-rbac-roledefinition.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7cb95-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="7cb95-106">Prerequisites</span></span>
<span data-ttu-id="7cb95-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7cb95-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7cb95-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7cb95-109">Permission type</span></span>|<span data-ttu-id="7cb95-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="7cb95-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7cb95-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7cb95-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7cb95-112">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="7cb95-112">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="7cb95-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7cb95-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7cb95-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7cb95-114">Not supported.</span></span>|
|<span data-ttu-id="7cb95-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7cb95-115">Application</span></span>|<span data-ttu-id="7cb95-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7cb95-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7cb95-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7cb95-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="7cb95-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7cb95-118">Request headers</span></span>
|<span data-ttu-id="7cb95-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7cb95-119">Header</span></span>|<span data-ttu-id="7cb95-120">値</span><span class="sxs-lookup"><span data-stu-id="7cb95-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7cb95-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7cb95-121">Authorization</span></span>|<span data-ttu-id="7cb95-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="7cb95-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7cb95-123">Accept</span><span class="sxs-lookup"><span data-stu-id="7cb95-123">Accept</span></span>|<span data-ttu-id="7cb95-124">application/json</span><span class="sxs-lookup"><span data-stu-id="7cb95-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7cb95-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="7cb95-125">Request body</span></span>
<span data-ttu-id="7cb95-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="7cb95-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7cb95-127">応答</span><span class="sxs-lookup"><span data-stu-id="7cb95-127">Response</span></span>
<span data-ttu-id="7cb95-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [roleDefinition](../resources/intune-rbac-roledefinition.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="7cb95-128">If successful, this method returns a `200 OK` response code and a collection of [roleDefinition](../resources/intune-rbac-roledefinition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7cb95-129">例</span><span class="sxs-lookup"><span data-stu-id="7cb95-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="7cb95-130">要求</span><span class="sxs-lookup"><span data-stu-id="7cb95-130">Request</span></span>
<span data-ttu-id="7cb95-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7cb95-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/roleDefinitions
```

### <a name="response"></a><span data-ttu-id="7cb95-132">応答</span><span class="sxs-lookup"><span data-stu-id="7cb95-132">Response</span></span>
<span data-ttu-id="7cb95-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7cb95-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



