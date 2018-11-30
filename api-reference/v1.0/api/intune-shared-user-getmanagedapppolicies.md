---
title: getManagedAppPolicies 関数
description: 特定のユーザーのアプリ制限を取得します。
ms.openlocfilehash: 6cb9b388b8b999b298da070f592ebf7a19d851c5
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27022692"
---
# <a name="getmanagedapppolicies-function"></a><span data-ttu-id="a7c7e-103">getManagedAppPolicies 関数</span><span class="sxs-lookup"><span data-stu-id="a7c7e-103">getManagedAppPolicies function</span></span>

> <span data-ttu-id="a7c7e-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="a7c7e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a7c7e-105">特定のユーザーのアプリ制限を取得します。</span><span class="sxs-lookup"><span data-stu-id="a7c7e-105">Gets app restrictions for a given user.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a7c7e-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="a7c7e-106">Prerequisites</span></span>
<span data-ttu-id="a7c7e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a7c7e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a7c7e-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a7c7e-109">Permission type</span></span>|<span data-ttu-id="a7c7e-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a7c7e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a7c7e-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a7c7e-111">Delegated (work or school account)</span></span>| <span data-ttu-id="a7c7e-112">_コンテキストによって異なります_</span><span class="sxs-lookup"><span data-stu-id="a7c7e-112">_varies by context_</span></span>|
| <span data-ttu-id="a7c7e-113">&nbsp;&nbsp; MAM</span><span class="sxs-lookup"><span data-stu-id="a7c7e-113">&nbsp; &nbsp; MAM</span></span> | <span data-ttu-id="a7c7e-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a7c7e-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span> |
|<span data-ttu-id="a7c7e-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a7c7e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a7c7e-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a7c7e-116">Not supported.</span></span>|
|<span data-ttu-id="a7c7e-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a7c7e-117">Application</span></span>|<span data-ttu-id="a7c7e-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a7c7e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a7c7e-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a7c7e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedAppPolicies
```

## <a name="request-headers"></a><span data-ttu-id="a7c7e-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a7c7e-120">Request headers</span></span>
|<span data-ttu-id="a7c7e-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a7c7e-121">Header</span></span>|<span data-ttu-id="a7c7e-122">値</span><span class="sxs-lookup"><span data-stu-id="a7c7e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a7c7e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a7c7e-123">Authorization</span></span>|<span data-ttu-id="a7c7e-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="a7c7e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a7c7e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a7c7e-125">Accept</span></span>|<span data-ttu-id="a7c7e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a7c7e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a7c7e-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="a7c7e-127">Request body</span></span>
<span data-ttu-id="a7c7e-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="a7c7e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a7c7e-129">応答</span><span class="sxs-lookup"><span data-stu-id="a7c7e-129">Response</span></span>
<span data-ttu-id="a7c7e-130">成功した場合、この関数は `200 OK` 応答コードと、応答本文で [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) コレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="a7c7e-130">If successful, this function returns a `200 OK` response code and a [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a7c7e-131">例</span><span class="sxs-lookup"><span data-stu-id="a7c7e-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="a7c7e-132">要求</span><span class="sxs-lookup"><span data-stu-id="a7c7e-132">Request</span></span>
<span data-ttu-id="a7c7e-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a7c7e-133">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/v1.0/users/{usersId}/getManagedAppPolicies
```

### <a name="response"></a><span data-ttu-id="a7c7e-134">応答</span><span class="sxs-lookup"><span data-stu-id="a7c7e-134">Response</span></span>
<span data-ttu-id="a7c7e-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a7c7e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 401

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedAppPolicy",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "id": "3c7b9675-9675-3c7b-7596-7b3c75967b3c",
      "version": "Version value"
    }
  ]
}
```



