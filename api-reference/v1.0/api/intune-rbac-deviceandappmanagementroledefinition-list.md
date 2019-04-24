---
title: deviceAndAppManagementRoleDefinitions のリスト
description: deviceAndAppManagementRoleDefinition オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 6530309293c0b678416806782fa699487300ca00
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32461144"
---
# <a name="list-deviceandappmanagementroledefinitions"></a><span data-ttu-id="adcca-103">deviceAndAppManagementRoleDefinitions のリスト</span><span class="sxs-lookup"><span data-stu-id="adcca-103">List deviceAndAppManagementRoleDefinitions</span></span>

> <span data-ttu-id="adcca-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="adcca-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="adcca-105">[deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="adcca-105">List properties and relationships of the [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="adcca-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="adcca-106">Prerequisites</span></span>
<span data-ttu-id="adcca-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="adcca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="adcca-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="adcca-109">Permission type</span></span>|<span data-ttu-id="adcca-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="adcca-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="adcca-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="adcca-111">Delegated (work or school account)</span></span>|<span data-ttu-id="adcca-112">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="adcca-112">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="adcca-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="adcca-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="adcca-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="adcca-114">Not supported.</span></span>|
|<span data-ttu-id="adcca-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="adcca-115">Application</span></span>|<span data-ttu-id="adcca-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="adcca-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="adcca-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="adcca-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="adcca-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="adcca-118">Request headers</span></span>
|<span data-ttu-id="adcca-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="adcca-119">Header</span></span>|<span data-ttu-id="adcca-120">値</span><span class="sxs-lookup"><span data-stu-id="adcca-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="adcca-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="adcca-121">Authorization</span></span>|<span data-ttu-id="adcca-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="adcca-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="adcca-123">承諾</span><span class="sxs-lookup"><span data-stu-id="adcca-123">Accept</span></span>|<span data-ttu-id="adcca-124">application/json</span><span class="sxs-lookup"><span data-stu-id="adcca-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="adcca-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="adcca-125">Request body</span></span>
<span data-ttu-id="adcca-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="adcca-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="adcca-127">応答</span><span class="sxs-lookup"><span data-stu-id="adcca-127">Response</span></span>
<span data-ttu-id="adcca-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="adcca-128">If successful, this method returns a `200 OK` response code and a collection of [deviceAndAppManagementRoleDefinition](../resources/intune-rbac-deviceandappmanagementroledefinition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="adcca-129">例</span><span class="sxs-lookup"><span data-stu-id="adcca-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="adcca-130">要求</span><span class="sxs-lookup"><span data-stu-id="adcca-130">Request</span></span>
<span data-ttu-id="adcca-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="adcca-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/roleDefinitions
```

### <a name="response"></a><span data-ttu-id="adcca-132">応答</span><span class="sxs-lookup"><span data-stu-id="adcca-132">Response</span></span>
<span data-ttu-id="adcca-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="adcca-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 768

{
  "value": [
    {
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
  ]
}
```



