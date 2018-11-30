---
title: auditEvents のリスト
description: auditEvent オブジェクトのプロパティとリレーションシップをリストします。
ms.openlocfilehash: 8b684ca2c70d7875c218d38d32f359313fa02ee3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071734"
---
# <a name="list-auditevents"></a><span data-ttu-id="fa054-103">auditEvents のリスト</span><span class="sxs-lookup"><span data-stu-id="fa054-103">List auditEvents</span></span>

> <span data-ttu-id="fa054-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="fa054-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fa054-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fa054-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fa054-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="fa054-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fa054-107">[auditEvent](../resources/intune-auditing-auditevent.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="fa054-107">List properties and relationships of the [auditEvent](../resources/intune-auditing-auditevent.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fa054-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="fa054-108">Prerequisites</span></span>
<span data-ttu-id="fa054-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fa054-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa054-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fa054-111">Permission type</span></span>|<span data-ttu-id="fa054-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="fa054-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fa054-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fa054-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fa054-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="fa054-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="fa054-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fa054-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fa054-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fa054-116">Not supported.</span></span>|
|<span data-ttu-id="fa054-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fa054-117">Application</span></span>|<span data-ttu-id="fa054-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fa054-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fa054-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fa054-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents
```

## <a name="request-headers"></a><span data-ttu-id="fa054-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fa054-120">Request headers</span></span>
|<span data-ttu-id="fa054-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fa054-121">Header</span></span>|<span data-ttu-id="fa054-122">値</span><span class="sxs-lookup"><span data-stu-id="fa054-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fa054-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fa054-123">Authorization</span></span>|<span data-ttu-id="fa054-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="fa054-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fa054-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fa054-125">Accept</span></span>|<span data-ttu-id="fa054-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fa054-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fa054-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="fa054-127">Request body</span></span>
<span data-ttu-id="fa054-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="fa054-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fa054-129">応答</span><span class="sxs-lookup"><span data-stu-id="fa054-129">Response</span></span>
<span data-ttu-id="fa054-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [auditEvent](../resources/intune-auditing-auditevent.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="fa054-130">If successful, this method returns a `200 OK` response code and a collection of [auditEvent](../resources/intune-auditing-auditevent.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fa054-131">例</span><span class="sxs-lookup"><span data-stu-id="fa054-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="fa054-132">要求</span><span class="sxs-lookup"><span data-stu-id="fa054-132">Request</span></span>
<span data-ttu-id="fa054-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="fa054-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/auditEvents
```

### <a name="response"></a><span data-ttu-id="fa054-134">応答</span><span class="sxs-lookup"><span data-stu-id="fa054-134">Response</span></span>
<span data-ttu-id="fa054-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="fa054-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





