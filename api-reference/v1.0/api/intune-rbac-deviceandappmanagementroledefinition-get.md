---
title: Get deviceAndAppManagementRoleDefinition
description: deviceAndAppManagementRoleDefinition オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 026b69fc58bc4cb466ad69ac2542eac13a44dadd
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32557041"
---
# <a name="get-deviceandappmanagementroledefinition"></a><span data-ttu-id="90288-103">Get deviceAndAppManagementRoleDefinition</span><span class="sxs-lookup"><span data-stu-id="90288-103">Get deviceAndAppManagementRoleDefinition</span></span>

> <span data-ttu-id="90288-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="90288-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="90288-105">[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="90288-105">Read properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="90288-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="90288-106">Prerequisites</span></span>
<span data-ttu-id="90288-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="90288-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="90288-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="90288-109">Permission type</span></span>|<span data-ttu-id="90288-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="90288-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="90288-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="90288-111">Delegated (work or school account)</span></span>|<span data-ttu-id="90288-112">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="90288-112">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="90288-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="90288-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="90288-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="90288-114">Not supported.</span></span>|
|<span data-ttu-id="90288-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="90288-115">Application</span></span>|<span data-ttu-id="90288-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="90288-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="90288-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="90288-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleDefinitions/{roleDefinitionId}
GET /deviceManagement/roleDefinitions/{roleDefinitionId}/roleAssignments/{roleAssignmentId}/roleDefinition
```

## <a name="optional-query-parameters"></a><span data-ttu-id="90288-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="90288-118">Optional query parameters</span></span>
<span data-ttu-id="90288-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="90288-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="90288-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="90288-120">Request headers</span></span>
|<span data-ttu-id="90288-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="90288-121">Header</span></span>|<span data-ttu-id="90288-122">値</span><span class="sxs-lookup"><span data-stu-id="90288-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="90288-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="90288-123">Authorization</span></span>|<span data-ttu-id="90288-124">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="90288-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="90288-125">承諾</span><span class="sxs-lookup"><span data-stu-id="90288-125">Accept</span></span>|<span data-ttu-id="90288-126">application/json</span><span class="sxs-lookup"><span data-stu-id="90288-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="90288-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="90288-127">Request body</span></span>
<span data-ttu-id="90288-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="90288-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="90288-129">応答</span><span class="sxs-lookup"><span data-stu-id="90288-129">Response</span></span>
<span data-ttu-id="90288-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="90288-130">If successful, this method returns a `200 OK` response code and [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="90288-131">例</span><span class="sxs-lookup"><span data-stu-id="90288-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="90288-132">要求</span><span class="sxs-lookup"><span data-stu-id="90288-132">Request</span></span>
<span data-ttu-id="90288-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="90288-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/roleDefinitions/{roleDefinitionId}
```

### <a name="response"></a><span data-ttu-id="90288-134">応答</span><span class="sxs-lookup"><span data-stu-id="90288-134">Response</span></span>
<span data-ttu-id="90288-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="90288-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



