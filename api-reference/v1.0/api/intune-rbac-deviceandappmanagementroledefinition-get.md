---
title: Get deviceAndAppManagementRoleDefinition
description: deviceAndAppManagementRoleDefinition オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
ms.openlocfilehash: 85038215c39321de1bcc497c3f53f6c99d06dd53
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27327868"
---
# <a name="get-deviceandappmanagementroledefinition"></a><span data-ttu-id="f4401-103">Get deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="f4401-103">Get deviceAndAppManagementRoleDefinition</span></span>

> <span data-ttu-id="f4401-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f4401-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f4401-105">[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="f4401-105">Read properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f4401-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="f4401-106">Prerequisites</span></span>
<span data-ttu-id="f4401-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f4401-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f4401-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f4401-109">Permission type</span></span>|<span data-ttu-id="f4401-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f4401-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f4401-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f4401-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f4401-112">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="f4401-112">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="f4401-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f4401-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f4401-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f4401-114">Not supported.</span></span>|
|<span data-ttu-id="f4401-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f4401-115">Application</span></span>|<span data-ttu-id="f4401-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f4401-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f4401-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f4401-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleDefinitions/{roleDefinitionId}
GET /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/roleDefinition
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f4401-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="f4401-118">Optional query parameters</span></span>
<span data-ttu-id="f4401-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="f4401-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="f4401-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f4401-120">Request headers</span></span>
|<span data-ttu-id="f4401-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f4401-121">Header</span></span>|<span data-ttu-id="f4401-122">値</span><span class="sxs-lookup"><span data-stu-id="f4401-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f4401-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f4401-123">Authorization</span></span>|<span data-ttu-id="f4401-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="f4401-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f4401-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f4401-125">Accept</span></span>|<span data-ttu-id="f4401-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f4401-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f4401-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="f4401-127">Request body</span></span>
<span data-ttu-id="f4401-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="f4401-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f4401-129">応答</span><span class="sxs-lookup"><span data-stu-id="f4401-129">Response</span></span>
<span data-ttu-id="f4401-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f4401-130">If successful, this method returns a `200 OK` response code and [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f4401-131">例</span><span class="sxs-lookup"><span data-stu-id="f4401-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="f4401-132">要求</span><span class="sxs-lookup"><span data-stu-id="f4401-132">Request</span></span>
<span data-ttu-id="f4401-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f4401-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/roleDefinitions/{roleDefinitionId}
```

### <a name="response"></a><span data-ttu-id="f4401-134">応答</span><span class="sxs-lookup"><span data-stu-id="f4401-134">Response</span></span>
<span data-ttu-id="f4401-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f4401-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 712

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceAndAppManagementRoleDefinition",
    "id": "bca1dfb5-dfb5-bca1-b5df-a1bcb5dfa1bc",
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
}
```



