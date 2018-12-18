---
title: Get auditEvent
description: auditEvent オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
ms.openlocfilehash: e4bcc13b5cce4e90e2a1b0ce31311723252d07c4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27339257"
---
# <a name="get-auditevent"></a><span data-ttu-id="e3783-103">Get auditEvent</span><span class="sxs-lookup"><span data-stu-id="e3783-103">Get auditEvent</span></span>

> <span data-ttu-id="e3783-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e3783-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e3783-105">[auditEvent](../resources/intune-auditing-auditevent.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="e3783-105">Read properties and relationships of the [auditEvent](../resources/intune-auditing-auditevent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e3783-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="e3783-106">Prerequisites</span></span>
<span data-ttu-id="e3783-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e3783-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e3783-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e3783-109">Permission type</span></span>|<span data-ttu-id="e3783-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="e3783-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e3783-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e3783-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e3783-112">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="e3783-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="e3783-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e3783-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e3783-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e3783-114">Not supported.</span></span>|
|<span data-ttu-id="e3783-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e3783-115">Application</span></span>|<span data-ttu-id="e3783-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e3783-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e3783-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e3783-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents/{auditEventId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e3783-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="e3783-118">Optional query parameters</span></span>
<span data-ttu-id="e3783-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="e3783-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="e3783-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e3783-120">Request headers</span></span>
|<span data-ttu-id="e3783-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e3783-121">Header</span></span>|<span data-ttu-id="e3783-122">値</span><span class="sxs-lookup"><span data-stu-id="e3783-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e3783-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e3783-123">Authorization</span></span>|<span data-ttu-id="e3783-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="e3783-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e3783-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e3783-125">Accept</span></span>|<span data-ttu-id="e3783-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e3783-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e3783-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="e3783-127">Request body</span></span>
<span data-ttu-id="e3783-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="e3783-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e3783-129">応答</span><span class="sxs-lookup"><span data-stu-id="e3783-129">Response</span></span>
<span data-ttu-id="e3783-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [auditEvent](../resources/intune-auditing-auditevent.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e3783-130">If successful, this method returns a `200 OK` response code and [auditEvent](../resources/intune-auditing-auditevent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e3783-131">例</span><span class="sxs-lookup"><span data-stu-id="e3783-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="e3783-132">要求</span><span class="sxs-lookup"><span data-stu-id="e3783-132">Request</span></span>
<span data-ttu-id="e3783-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e3783-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/auditEvents/{auditEventId}
```

### <a name="response"></a><span data-ttu-id="e3783-134">応答</span><span class="sxs-lookup"><span data-stu-id="e3783-134">Response</span></span>
<span data-ttu-id="e3783-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e3783-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1538

{
  "value": {
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
}
```



