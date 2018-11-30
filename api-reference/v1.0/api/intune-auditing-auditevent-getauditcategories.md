---
title: getAuditCategories function
description: まだ文書化されていません
ms.openlocfilehash: 4e54768c6381f947ea9b65751986f756422a46fa
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023572"
---
# <a name="getauditcategories-function"></a><span data-ttu-id="cbdf1-103">getAuditCategories function</span><span class="sxs-lookup"><span data-stu-id="cbdf1-103">getAuditCategories function</span></span>

> <span data-ttu-id="cbdf1-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="cbdf1-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cbdf1-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="cbdf1-105">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cbdf1-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="cbdf1-106">Prerequisites</span></span>
<span data-ttu-id="cbdf1-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cbdf1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cbdf1-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="cbdf1-109">Permission type</span></span>|<span data-ttu-id="cbdf1-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="cbdf1-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cbdf1-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="cbdf1-111">Delegated (work or school account)</span></span>|<span data-ttu-id="cbdf1-112">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="cbdf1-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="cbdf1-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="cbdf1-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cbdf1-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cbdf1-114">Not supported.</span></span>|
|<span data-ttu-id="cbdf1-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="cbdf1-115">Application</span></span>|<span data-ttu-id="cbdf1-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="cbdf1-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cbdf1-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="cbdf1-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/auditEvents/getAuditCategories
```

## <a name="request-headers"></a><span data-ttu-id="cbdf1-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cbdf1-118">Request headers</span></span>
|<span data-ttu-id="cbdf1-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cbdf1-119">Header</span></span>|<span data-ttu-id="cbdf1-120">値</span><span class="sxs-lookup"><span data-stu-id="cbdf1-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cbdf1-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="cbdf1-121">Authorization</span></span>|<span data-ttu-id="cbdf1-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="cbdf1-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cbdf1-123">Accept</span><span class="sxs-lookup"><span data-stu-id="cbdf1-123">Accept</span></span>|<span data-ttu-id="cbdf1-124">application/json</span><span class="sxs-lookup"><span data-stu-id="cbdf1-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cbdf1-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="cbdf1-125">Request body</span></span>
<span data-ttu-id="cbdf1-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="cbdf1-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cbdf1-127">応答</span><span class="sxs-lookup"><span data-stu-id="cbdf1-127">Response</span></span>
<span data-ttu-id="cbdf1-128">成功した場合、この関数は `200 OK` 応答コードと、応答本文で String コレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="cbdf1-128">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cbdf1-129">例</span><span class="sxs-lookup"><span data-stu-id="cbdf1-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="cbdf1-130">要求</span><span class="sxs-lookup"><span data-stu-id="cbdf1-130">Request</span></span>
<span data-ttu-id="cbdf1-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="cbdf1-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/auditEvents/getAuditCategories
```

### <a name="response"></a><span data-ttu-id="cbdf1-132">応答</span><span class="sxs-lookup"><span data-stu-id="cbdf1-132">Response</span></span>
<span data-ttu-id="cbdf1-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="cbdf1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 57

{
  "value": [
    "Get Audit Categories value"
  ]
}
```


