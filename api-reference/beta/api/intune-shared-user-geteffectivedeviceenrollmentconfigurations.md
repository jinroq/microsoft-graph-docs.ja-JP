---
title: getEffectiveDeviceEnrollmentConfigurations 関数
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5ede65e91303cd939648abbe9a23bd026fd778b5
ms.sourcegitcommit: f58ff560fa02ac95e296375c143b0922fb6a425c
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/19/2019
ms.locfileid: "30572230"
---
# <a name="geteffectivedeviceenrollmentconfigurations-function"></a><span data-ttu-id="22835-103">getEffectiveDeviceEnrollmentConfigurations 関数</span><span class="sxs-lookup"><span data-stu-id="22835-103">getEffectiveDeviceEnrollmentConfigurations function</span></span>

> <span data-ttu-id="22835-104">**重要:** Microsoft Graph の/ベータ版の api は変更される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="22835-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="22835-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="22835-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="22835-106">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="22835-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="22835-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="22835-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="22835-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="22835-108">Prerequisites</span></span>

<span data-ttu-id="22835-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="22835-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="22835-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="22835-111">Permission type</span></span>|<span data-ttu-id="22835-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="22835-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="22835-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="22835-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="22835-114">&nbsp; &nbsp; **オンボーディング**</span><span class="sxs-lookup"><span data-stu-id="22835-114">&nbsp; &nbsp; **Onboarding**</span></span> | <span data-ttu-id="22835-115">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22835-115">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="22835-116">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="22835-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="22835-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="22835-117">Not supported.</span></span>|
|<span data-ttu-id="22835-118">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="22835-118">Application</span></span>|<span data-ttu-id="22835-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="22835-119">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="22835-120">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="22835-120">HTTP Request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getEffectiveDeviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="22835-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="22835-121">Request headers</span></span>

|<span data-ttu-id="22835-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="22835-122">Header</span></span>|<span data-ttu-id="22835-123">値</span><span class="sxs-lookup"><span data-stu-id="22835-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="22835-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="22835-124">Authorization</span></span>|<span data-ttu-id="22835-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="22835-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="22835-126">承諾</span><span class="sxs-lookup"><span data-stu-id="22835-126">Accept</span></span>|<span data-ttu-id="22835-127">application/json</span><span class="sxs-lookup"><span data-stu-id="22835-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="22835-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="22835-128">Request body</span></span>

<span data-ttu-id="22835-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="22835-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="22835-130">応答</span><span class="sxs-lookup"><span data-stu-id="22835-130">Response</span></span>

<span data-ttu-id="22835-131">成功した場合、この関数`200 OK`は応答コードと、応答本文で[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)コレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="22835-131">If successful, this function returns a `200 OK` response code and a [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="22835-132">例</span><span class="sxs-lookup"><span data-stu-id="22835-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="22835-133">要求</span><span class="sxs-lookup"><span data-stu-id="22835-133">Request</span></span>

<span data-ttu-id="22835-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="22835-134">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/users/{usersId}/getEffectiveDeviceEnrollmentConfigurations
```

### <a name="response"></a><span data-ttu-id="22835-135">応答</span><span class="sxs-lookup"><span data-stu-id="22835-135">Response</span></span>

<span data-ttu-id="22835-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="22835-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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



