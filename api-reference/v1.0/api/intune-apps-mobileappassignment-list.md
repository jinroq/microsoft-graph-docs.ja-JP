---
title: mobileAppAssignments のリスト
description: mobileAppAssignment オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: fa626e56cea6bae1cb43a8e607ecc3701a17946e
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27811278"
---
# <a name="list-mobileappassignments"></a><span data-ttu-id="dafea-103">mobileAppAssignments のリスト</span><span class="sxs-lookup"><span data-stu-id="dafea-103">List mobileAppAssignments</span></span>

> <span data-ttu-id="dafea-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="dafea-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="dafea-105">[mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="dafea-105">List properties and relationships of the [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="dafea-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="dafea-106">Prerequisites</span></span>
<span data-ttu-id="dafea-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="dafea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dafea-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="dafea-109">Permission type</span></span>|<span data-ttu-id="dafea-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="dafea-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dafea-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="dafea-111">Delegated (work or school account)</span></span>|<span data-ttu-id="dafea-112">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="dafea-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="dafea-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="dafea-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dafea-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dafea-114">Not supported.</span></span>|
|<span data-ttu-id="dafea-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="dafea-115">Application</span></span>|<span data-ttu-id="dafea-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="dafea-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dafea-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="dafea-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="dafea-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="dafea-118">Request headers</span></span>
|<span data-ttu-id="dafea-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="dafea-119">Header</span></span>|<span data-ttu-id="dafea-120">値</span><span class="sxs-lookup"><span data-stu-id="dafea-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dafea-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="dafea-121">Authorization</span></span>|<span data-ttu-id="dafea-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="dafea-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dafea-123">Accept</span><span class="sxs-lookup"><span data-stu-id="dafea-123">Accept</span></span>|<span data-ttu-id="dafea-124">application/json</span><span class="sxs-lookup"><span data-stu-id="dafea-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dafea-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="dafea-125">Request body</span></span>
<span data-ttu-id="dafea-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="dafea-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="dafea-127">応答</span><span class="sxs-lookup"><span data-stu-id="dafea-127">Response</span></span>
<span data-ttu-id="dafea-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="dafea-128">If successful, this method returns a `200 OK` response code and a collection of [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dafea-129">例</span><span class="sxs-lookup"><span data-stu-id="dafea-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="dafea-130">要求</span><span class="sxs-lookup"><span data-stu-id="dafea-130">Request</span></span>
<span data-ttu-id="dafea-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="dafea-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/assignments
```

### <a name="response"></a><span data-ttu-id="dafea-132">応答</span><span class="sxs-lookup"><span data-stu-id="dafea-132">Response</span></span>
<span data-ttu-id="dafea-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="dafea-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 391

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileAppAssignment",
      "id": "591620b7-20b7-5916-b720-1659b7201659",
      "intent": "required",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      },
      "settings": {
        "@odata.type": "microsoft.graph.mobileAppAssignmentSettings"
      }
    }
  ]
}
```



