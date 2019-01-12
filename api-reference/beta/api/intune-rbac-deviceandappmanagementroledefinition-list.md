---
title: deviceAndAppManagementRoleDefinitions のリスト
description: deviceAndAppManagementRoleDefinition オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: e6fbd7f8734a9b6b01771cadf9e1e6126e7b8193
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27990937"
---
# <a name="list-deviceandappmanagementroledefinitions"></a><span data-ttu-id="99a67-103">deviceAndAppManagementRoleDefinitions のリスト</span><span class="sxs-lookup"><span data-stu-id="99a67-103">List deviceAndAppManagementRoleDefinitions</span></span>

> <span data-ttu-id="99a67-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="99a67-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="99a67-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="99a67-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="99a67-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="99a67-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="99a67-107">[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="99a67-107">List properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="99a67-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="99a67-108">Prerequisites</span></span>
<span data-ttu-id="99a67-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="99a67-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="99a67-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="99a67-111">Permission type</span></span>|<span data-ttu-id="99a67-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="99a67-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="99a67-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="99a67-113">Delegated (work or school account)</span></span>|<span data-ttu-id="99a67-114">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="99a67-114">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="99a67-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="99a67-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="99a67-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="99a67-116">Not supported.</span></span>|
|<span data-ttu-id="99a67-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="99a67-117">Application</span></span>|<span data-ttu-id="99a67-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="99a67-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="99a67-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="99a67-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="99a67-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="99a67-120">Request headers</span></span>
|<span data-ttu-id="99a67-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="99a67-121">Header</span></span>|<span data-ttu-id="99a67-122">値</span><span class="sxs-lookup"><span data-stu-id="99a67-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="99a67-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="99a67-123">Authorization</span></span>|<span data-ttu-id="99a67-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="99a67-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="99a67-125">Accept</span><span class="sxs-lookup"><span data-stu-id="99a67-125">Accept</span></span>|<span data-ttu-id="99a67-126">application/json</span><span class="sxs-lookup"><span data-stu-id="99a67-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="99a67-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="99a67-127">Request body</span></span>
<span data-ttu-id="99a67-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="99a67-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="99a67-129">応答</span><span class="sxs-lookup"><span data-stu-id="99a67-129">Response</span></span>
<span data-ttu-id="99a67-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="99a67-130">If successful, this method returns a `200 OK` response code and a collection of [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="99a67-131">例</span><span class="sxs-lookup"><span data-stu-id="99a67-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="99a67-132">要求</span><span class="sxs-lookup"><span data-stu-id="99a67-132">Request</span></span>
<span data-ttu-id="99a67-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="99a67-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/roleDefinitions
```

### <a name="response"></a><span data-ttu-id="99a67-134">応答</span><span class="sxs-lookup"><span data-stu-id="99a67-134">Response</span></span>
<span data-ttu-id="99a67-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="99a67-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1425

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleDefinition",
      "id": "bca1dfb5-dfb5-bca1-b5df-a1bcb5dfa1bc",
      "displayName": "Display Name value",
      "description": "Description value",
      "permissions": [
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
      ],
      "rolePermissions": [
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
      ],
      "isBuiltInRoleDefinition": true,
      "isBuiltIn": true
    }
  ]
}
```





