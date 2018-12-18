---
title: getEffectiveDeviceEnrollmentConfigurations 関数
description: まだ文書化されていません
author: tfitzmac
ms.openlocfilehash: b7bdf815f972f56892027a01db83539065fe9caf
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27315254"
---
# <a name="geteffectivedeviceenrollmentconfigurations-function"></a><span data-ttu-id="5da2c-103">getEffectiveDeviceEnrollmentConfigurations 関数</span><span class="sxs-lookup"><span data-stu-id="5da2c-103">getEffectiveDeviceEnrollmentConfigurations function</span></span>

> <span data-ttu-id="5da2c-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5da2c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5da2c-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5da2c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5da2c-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="5da2c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5da2c-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="5da2c-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5da2c-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="5da2c-108">Prerequisites</span></span>

<span data-ttu-id="5da2c-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5da2c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5da2c-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5da2c-111">Permission type</span></span>|<span data-ttu-id="5da2c-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="5da2c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5da2c-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5da2c-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="5da2c-114">&nbsp;&nbsp; **契約時**</span><span class="sxs-lookup"><span data-stu-id="5da2c-114">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="5da2c-115">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5da2c-115">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="5da2c-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5da2c-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5da2c-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5da2c-117">Not supported.</span></span>|
|<span data-ttu-id="5da2c-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5da2c-118">Application</span></span>|<span data-ttu-id="5da2c-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5da2c-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5da2c-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5da2c-120">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getEffectiveDeviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="5da2c-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5da2c-121">Request headers</span></span>

|<span data-ttu-id="5da2c-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5da2c-122">Header</span></span>|<span data-ttu-id="5da2c-123">値</span><span class="sxs-lookup"><span data-stu-id="5da2c-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5da2c-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="5da2c-124">Authorization</span></span>|<span data-ttu-id="5da2c-125">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="5da2c-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5da2c-126">Accept</span><span class="sxs-lookup"><span data-stu-id="5da2c-126">Accept</span></span>|<span data-ttu-id="5da2c-127">application/json</span><span class="sxs-lookup"><span data-stu-id="5da2c-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5da2c-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="5da2c-128">Request body</span></span>

<span data-ttu-id="5da2c-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="5da2c-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5da2c-130">応答</span><span class="sxs-lookup"><span data-stu-id="5da2c-130">Response</span></span>

<span data-ttu-id="5da2c-131">かどうかは成功すると、この関数を返します、`200 OK`応答コードおよび応答の本文に[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="5da2c-131">If successful, this function returns a `200 OK` response code and a [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5da2c-132">例</span><span class="sxs-lookup"><span data-stu-id="5da2c-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="5da2c-133">要求</span><span class="sxs-lookup"><span data-stu-id="5da2c-133">Request</span></span>

<span data-ttu-id="5da2c-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5da2c-134">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/users/{usersId}/getEffectiveDeviceEnrollmentConfigurations
```

### <a name="response"></a><span data-ttu-id="5da2c-135">応答</span><span class="sxs-lookup"><span data-stu-id="5da2c-135">Response</span></span>

<span data-ttu-id="5da2c-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="5da2c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 422

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceEnrollmentConfiguration",
      "id": "df13d8b9-d8b9-df13-b9d8-13dfb9d813df",
      "displayName": "Display Name value",
      "description": "Description value",
      "priority": 8,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "version": 7
    }
  ]
}
```



