---
title: リスト iosVppAppAssignedLicenses
description: IosVppAppAssignedLicense オブジェクトのプロパティと関係を一覧表示します。
ms.openlocfilehash: c8589cea1baf58c070ec21510bd06380d5e98885
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067614"
---
# <a name="list-iosvppappassignedlicenses"></a><span data-ttu-id="83106-103">リスト iosVppAppAssignedLicenses</span><span class="sxs-lookup"><span data-stu-id="83106-103">List iosVppAppAssignedLicenses</span></span>

> <span data-ttu-id="83106-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="83106-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="83106-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="83106-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="83106-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="83106-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="83106-107">[IosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="83106-107">List properties and relationships of the [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="83106-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="83106-108">Prerequisites</span></span>
<span data-ttu-id="83106-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="83106-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="83106-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="83106-111">Permission type</span></span>|<span data-ttu-id="83106-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="83106-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="83106-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="83106-113">Delegated (work or school account)</span></span>|<span data-ttu-id="83106-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="83106-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="83106-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="83106-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="83106-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="83106-116">Not supported.</span></span>|
|<span data-ttu-id="83106-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="83106-117">Application</span></span>|<span data-ttu-id="83106-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="83106-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="83106-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="83106-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="83106-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="83106-120">Request headers</span></span>
|<span data-ttu-id="83106-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="83106-121">Header</span></span>|<span data-ttu-id="83106-122">値</span><span class="sxs-lookup"><span data-stu-id="83106-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="83106-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="83106-123">Authorization</span></span>|<span data-ttu-id="83106-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="83106-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="83106-125">Accept</span><span class="sxs-lookup"><span data-stu-id="83106-125">Accept</span></span>|<span data-ttu-id="83106-126">application/json</span><span class="sxs-lookup"><span data-stu-id="83106-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="83106-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="83106-127">Request body</span></span>
<span data-ttu-id="83106-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="83106-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="83106-129">応答</span><span class="sxs-lookup"><span data-stu-id="83106-129">Response</span></span>
<span data-ttu-id="83106-130">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)オブジェクトのコレクションです。</span><span class="sxs-lookup"><span data-stu-id="83106-130">If successful, this method returns a `200 OK` response code and a collection of [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="83106-131">例</span><span class="sxs-lookup"><span data-stu-id="83106-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="83106-132">要求</span><span class="sxs-lookup"><span data-stu-id="83106-132">Request</span></span>
<span data-ttu-id="83106-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="83106-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

### <a name="response"></a><span data-ttu-id="83106-134">応答</span><span class="sxs-lookup"><span data-stu-id="83106-134">Response</span></span>
<span data-ttu-id="83106-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="83106-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 340

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosVppAppAssignedLicense",
      "id": "090a8d2e-8d2e-090a-2e8d-0a092e8d0a09",
      "userEmailAddress": "User Email Address value",
      "userId": "User Id value",
      "userName": "User Name value",
      "userPrincipalName": "User Principal Name value"
    }
  ]
}
```





