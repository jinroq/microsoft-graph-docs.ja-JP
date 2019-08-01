---
title: roleDefinitions のリスト
description: roleDefinition オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f546f100551b93749adc7625bb37f6e297e89dc3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36023700"
---
# <a name="list-roledefinitions"></a><span data-ttu-id="7f78e-103">roleDefinitions のリスト</span><span class="sxs-lookup"><span data-stu-id="7f78e-103">List roleDefinitions</span></span>

> <span data-ttu-id="7f78e-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="7f78e-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7f78e-105">[roleDefinition](../resources/intune-rbac-roledefinition.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="7f78e-105">List properties and relationships of the [roleDefinition](../resources/intune-rbac-roledefinition.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7f78e-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="7f78e-106">Prerequisites</span></span>
<span data-ttu-id="7f78e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7f78e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f78e-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7f78e-109">Permission type</span></span>|<span data-ttu-id="7f78e-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="7f78e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7f78e-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7f78e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7f78e-112">DeviceManagementRBAC.ReadWrite.All、DeviceManagementRBAC.Read.All</span><span class="sxs-lookup"><span data-stu-id="7f78e-112">DeviceManagementRBAC.ReadWrite.All, DeviceManagementRBAC.Read.All</span></span>|
|<span data-ttu-id="7f78e-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7f78e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7f78e-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7f78e-114">Not supported.</span></span>|
|<span data-ttu-id="7f78e-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7f78e-115">Application</span></span>|<span data-ttu-id="7f78e-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7f78e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7f78e-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7f78e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/roleDefinitions
```

## <a name="request-headers"></a><span data-ttu-id="7f78e-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7f78e-118">Request headers</span></span>
|<span data-ttu-id="7f78e-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7f78e-119">Header</span></span>|<span data-ttu-id="7f78e-120">値</span><span class="sxs-lookup"><span data-stu-id="7f78e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7f78e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7f78e-121">Authorization</span></span>|<span data-ttu-id="7f78e-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="7f78e-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7f78e-123">承諾</span><span class="sxs-lookup"><span data-stu-id="7f78e-123">Accept</span></span>|<span data-ttu-id="7f78e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="7f78e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7f78e-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="7f78e-125">Request body</span></span>
<span data-ttu-id="7f78e-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="7f78e-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7f78e-127">応答</span><span class="sxs-lookup"><span data-stu-id="7f78e-127">Response</span></span>
<span data-ttu-id="7f78e-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [roleDefinition](../resources/intune-rbac-roledefinition.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="7f78e-128">If successful, this method returns a `200 OK` response code and a collection of [roleDefinition](../resources/intune-rbac-roledefinition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7f78e-129">例</span><span class="sxs-lookup"><span data-stu-id="7f78e-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="7f78e-130">要求</span><span class="sxs-lookup"><span data-stu-id="7f78e-130">Request</span></span>
<span data-ttu-id="7f78e-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7f78e-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/roleDefinitions
```

### <a name="response"></a><span data-ttu-id="7f78e-132">応答</span><span class="sxs-lookup"><span data-stu-id="7f78e-132">Response</span></span>
<span data-ttu-id="7f78e-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7f78e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



