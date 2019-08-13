---
title: deviceAndAppManagementRoleDefinitions のリスト
description: deviceAndAppManagementRoleDefinition オブジェクトのプロパティとリレーションシップをリストします。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ff3db2c2349c813bda3170f33645afc35f2230e7
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36351470"
---
# <a name="list-deviceandappmanagementroledefinitions"></a><span data-ttu-id="7e1ae-103">deviceAndAppManagementRoleDefinitions のリスト</span><span class="sxs-lookup"><span data-stu-id="7e1ae-103">List deviceAndAppManagementRoleDefinitions</span></span>

> <span data-ttu-id="7e1ae-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7e1ae-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7e1ae-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7e1ae-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7e1ae-106">[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="7e1ae-106">List properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7e1ae-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="7e1ae-107">Prerequisites</span></span>
<span data-ttu-id="7e1ae-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7e1ae-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7e1ae-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7e1ae-110">Permission type</span></span>|<span data-ttu-id="7e1ae-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="7e1ae-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7e1ae-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7e1ae-112">Delegated (work or school account)</span></span>|<span data-ttu-id="7e1ae-113">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="7e1ae-113">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="7e1ae-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7e1ae-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7e1ae-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7e1ae-115">Not supported.</span></span>|
|<span data-ttu-id="7e1ae-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7e1ae-116">Application</span></span>|<span data-ttu-id="7e1ae-117">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="7e1ae-117">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7e1ae-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7e1ae-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="7e1ae-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7e1ae-119">Request headers</span></span>
|<span data-ttu-id="7e1ae-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7e1ae-120">Header</span></span>|<span data-ttu-id="7e1ae-121">値</span><span class="sxs-lookup"><span data-stu-id="7e1ae-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7e1ae-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="7e1ae-122">Authorization</span></span>|<span data-ttu-id="7e1ae-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="7e1ae-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7e1ae-124">承諾</span><span class="sxs-lookup"><span data-stu-id="7e1ae-124">Accept</span></span>|<span data-ttu-id="7e1ae-125">application/json</span><span class="sxs-lookup"><span data-stu-id="7e1ae-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7e1ae-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="7e1ae-126">Request body</span></span>
<span data-ttu-id="7e1ae-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="7e1ae-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7e1ae-128">応答</span><span class="sxs-lookup"><span data-stu-id="7e1ae-128">Response</span></span>
<span data-ttu-id="7e1ae-129">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="7e1ae-129">If successful, this method returns a `200 OK` response code and a collection of [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7e1ae-130">例</span><span class="sxs-lookup"><span data-stu-id="7e1ae-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="7e1ae-131">要求</span><span class="sxs-lookup"><span data-stu-id="7e1ae-131">Request</span></span>
<span data-ttu-id="7e1ae-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7e1ae-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/roleDefinitions
```

### <a name="response"></a><span data-ttu-id="7e1ae-133">応答</span><span class="sxs-lookup"><span data-stu-id="7e1ae-133">Response</span></span>
<span data-ttu-id="7e1ae-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7e1ae-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1499

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
      "isBuiltIn": true,
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ]
    }
  ]
}
```






