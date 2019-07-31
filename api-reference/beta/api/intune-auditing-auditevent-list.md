---
title: auditEvents のリスト
description: auditEvent オブジェクトのプロパティとリレーションシップをリストします。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 24d362fe3b6316f291eecef2f511509859977a99
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35959482"
---
# <a name="list-auditevents"></a><span data-ttu-id="92a99-103">auditEvents のリスト</span><span class="sxs-lookup"><span data-stu-id="92a99-103">List auditEvents</span></span>

> <span data-ttu-id="92a99-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="92a99-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="92a99-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="92a99-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="92a99-106">[auditEvent](../resources/intune-auditing-auditevent.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="92a99-106">List properties and relationships of the [auditEvent](../resources/intune-auditing-auditevent.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="92a99-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="92a99-107">Prerequisites</span></span>
<span data-ttu-id="92a99-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="92a99-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="92a99-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="92a99-110">Permission type</span></span>|<span data-ttu-id="92a99-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="92a99-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="92a99-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="92a99-112">Delegated (work or school account)</span></span>|<span data-ttu-id="92a99-113">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="92a99-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="92a99-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="92a99-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="92a99-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="92a99-115">Not supported.</span></span>|
|<span data-ttu-id="92a99-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="92a99-116">Application</span></span>|<span data-ttu-id="92a99-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="92a99-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="92a99-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="92a99-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents
```

## <a name="request-headers"></a><span data-ttu-id="92a99-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="92a99-119">Request headers</span></span>
|<span data-ttu-id="92a99-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="92a99-120">Header</span></span>|<span data-ttu-id="92a99-121">値</span><span class="sxs-lookup"><span data-stu-id="92a99-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="92a99-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="92a99-122">Authorization</span></span>|<span data-ttu-id="92a99-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="92a99-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="92a99-124">承諾</span><span class="sxs-lookup"><span data-stu-id="92a99-124">Accept</span></span>|<span data-ttu-id="92a99-125">application/json</span><span class="sxs-lookup"><span data-stu-id="92a99-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="92a99-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="92a99-126">Request body</span></span>
<span data-ttu-id="92a99-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="92a99-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="92a99-128">応答</span><span class="sxs-lookup"><span data-stu-id="92a99-128">Response</span></span>
<span data-ttu-id="92a99-129">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [auditEvent](../resources/intune-auditing-auditevent.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="92a99-129">If successful, this method returns a `200 OK` response code and a collection of [auditEvent](../resources/intune-auditing-auditevent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="92a99-130">例</span><span class="sxs-lookup"><span data-stu-id="92a99-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="92a99-131">要求</span><span class="sxs-lookup"><span data-stu-id="92a99-131">Request</span></span>
<span data-ttu-id="92a99-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="92a99-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/auditEvents
```

### <a name="response"></a><span data-ttu-id="92a99-133">応答</span><span class="sxs-lookup"><span data-stu-id="92a99-133">Response</span></span>
<span data-ttu-id="92a99-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="92a99-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1632

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.auditEvent",
      "id": "59653ce8-3ce8-5965-e83c-6559e83c6559",
      "displayName": "Display Name value",
      "componentName": "Component Name value",
      "actor": {
        "@odata.type": "microsoft.graph.auditActor",
        "type": "Type value",
        "userPermissions": [
          "User Permissions value"
        ],
        "applicationId": "Application Id value",
        "applicationDisplayName": "Application Display Name value",
        "userPrincipalName": "User Principal Name value",
        "servicePrincipalName": "Service Principal Name value",
        "ipAddress": "Ip Address value",
        "userId": "User Id value"
      },
      "activity": "Activity value",
      "activityDateTime": "2016-12-31T23:59:51.6363086-08:00",
      "activityType": "Activity Type value",
      "activityOperationType": "Activity Operation Type value",
      "activityResult": "Activity Result value",
      "correlationId": "52effe71-fe71-52ef-71fe-ef5271feef52",
      "resources": [
        {
          "@odata.type": "microsoft.graph.auditResource",
          "displayName": "Display Name value",
          "modifiedProperties": [
            {
              "@odata.type": "microsoft.graph.auditProperty",
              "displayName": "Display Name value",
              "oldValue": "Old Value value",
              "newValue": "New Value value"
            }
          ],
          "type": "Type value",
          "resourceId": "Resource Id value"
        }
      ],
      "category": "Category value"
    }
  ]
}
```





