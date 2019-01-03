---
title: getUserIdsWithFlaggedAppRegistration 関数
description: まだ文書化されていません
author: tfitzmac
ms.openlocfilehash: 7f57ab3af48ac7e815b914be3339435d6be58fc4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27329380"
---
# <a name="getuseridswithflaggedappregistration-function"></a><span data-ttu-id="0bd34-103">getUserIdsWithFlaggedAppRegistration 関数</span><span class="sxs-lookup"><span data-stu-id="0bd34-103">getUserIdsWithFlaggedAppRegistration function</span></span>

> <span data-ttu-id="0bd34-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0bd34-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0bd34-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0bd34-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0bd34-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="0bd34-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0bd34-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="0bd34-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0bd34-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="0bd34-108">Prerequisites</span></span>
<span data-ttu-id="0bd34-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0bd34-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0bd34-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0bd34-111">Permission type</span></span>|<span data-ttu-id="0bd34-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="0bd34-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0bd34-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0bd34-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0bd34-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="0bd34-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="0bd34-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0bd34-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0bd34-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0bd34-116">Not supported.</span></span>|
|<span data-ttu-id="0bd34-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0bd34-117">Application</span></span>|<span data-ttu-id="0bd34-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0bd34-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0bd34-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0bd34-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedAppRegistrations/getUserIdsWithFlaggedAppRegistration
```

## <a name="request-headers"></a><span data-ttu-id="0bd34-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0bd34-120">Request headers</span></span>
|<span data-ttu-id="0bd34-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0bd34-121">Header</span></span>|<span data-ttu-id="0bd34-122">値</span><span class="sxs-lookup"><span data-stu-id="0bd34-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0bd34-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0bd34-123">Authorization</span></span>|<span data-ttu-id="0bd34-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="0bd34-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0bd34-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0bd34-125">Accept</span></span>|<span data-ttu-id="0bd34-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0bd34-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0bd34-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="0bd34-127">Request body</span></span>
<span data-ttu-id="0bd34-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="0bd34-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0bd34-129">応答</span><span class="sxs-lookup"><span data-stu-id="0bd34-129">Response</span></span>
<span data-ttu-id="0bd34-130">成功した場合、この関数は `200 OK` 応答コードと、応答本文で String コレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="0bd34-130">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0bd34-131">例</span><span class="sxs-lookup"><span data-stu-id="0bd34-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="0bd34-132">要求</span><span class="sxs-lookup"><span data-stu-id="0bd34-132">Request</span></span>
<span data-ttu-id="0bd34-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0bd34-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/managedAppRegistrations/getUserIdsWithFlaggedAppRegistration
```

### <a name="response"></a><span data-ttu-id="0bd34-134">応答</span><span class="sxs-lookup"><span data-stu-id="0bd34-134">Response</span></span>
<span data-ttu-id="0bd34-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0bd34-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 79

{
  "value": [
    "Get User Ids With Flagged App Registration value"
  ]
}
```




