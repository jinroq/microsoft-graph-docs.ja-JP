---
title: getManagedAppPolicies 関数
description: 特定のユーザーのアプリ制限を取得します。
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 29c57b953b7d3966261c5089508a3ea9fc5a717e
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36350658"
---
# <a name="getmanagedapppolicies-function"></a><span data-ttu-id="0a167-103">getManagedAppPolicies 関数</span><span class="sxs-lookup"><span data-stu-id="0a167-103">getManagedAppPolicies function</span></span>

> <span data-ttu-id="0a167-104">**重要:** Microsoft Graph の/ベータ版の Api は変更される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="0a167-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="0a167-105">実稼働アプリケーションでは、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0a167-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0a167-106">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="0a167-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0a167-107">特定のユーザーのアプリ制限を取得します。</span><span class="sxs-lookup"><span data-stu-id="0a167-107">Gets app restrictions for a given user.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0a167-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="0a167-108">Prerequisites</span></span>

<span data-ttu-id="0a167-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0a167-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0a167-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="0a167-111">Permission type</span></span>|<span data-ttu-id="0a167-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="0a167-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0a167-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="0a167-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="0a167-114">&nbsp;&nbsp; **MAM**</span><span class="sxs-lookup"><span data-stu-id="0a167-114">&nbsp; &nbsp; **MAM**</span></span> | <span data-ttu-id="0a167-115">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="0a167-115">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="0a167-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="0a167-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0a167-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0a167-117">Not supported.</span></span>|
|<span data-ttu-id="0a167-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="0a167-118">Application</span></span>|<span data-ttu-id="0a167-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="0a167-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0a167-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="0a167-120">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getManagedAppPolicies
```

## <a name="request-headers"></a><span data-ttu-id="0a167-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0a167-121">Request headers</span></span>

|<span data-ttu-id="0a167-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0a167-122">Header</span></span>|<span data-ttu-id="0a167-123">値</span><span class="sxs-lookup"><span data-stu-id="0a167-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0a167-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="0a167-124">Authorization</span></span>|<span data-ttu-id="0a167-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="0a167-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0a167-126">承諾</span><span class="sxs-lookup"><span data-stu-id="0a167-126">Accept</span></span>|<span data-ttu-id="0a167-127">application/json</span><span class="sxs-lookup"><span data-stu-id="0a167-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0a167-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="0a167-128">Request body</span></span>

<span data-ttu-id="0a167-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="0a167-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0a167-130">応答</span><span class="sxs-lookup"><span data-stu-id="0a167-130">Response</span></span>

<span data-ttu-id="0a167-131">成功した場合、この関数は `200 OK` 応答コードと、応答本文で [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) コレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="0a167-131">If successful, this function returns a `200 OK` response code and a [managedAppPolicy](../resources/intune-mam-managedapppolicy.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0a167-132">例</span><span class="sxs-lookup"><span data-stu-id="0a167-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="0a167-133">要求</span><span class="sxs-lookup"><span data-stu-id="0a167-133">Request</span></span>

<span data-ttu-id="0a167-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="0a167-134">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/users/{usersId}/getManagedAppPolicies
```

### <a name="response"></a><span data-ttu-id="0a167-135">応答</span><span class="sxs-lookup"><span data-stu-id="0a167-135">Response</span></span>

<span data-ttu-id="0a167-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="0a167-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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









