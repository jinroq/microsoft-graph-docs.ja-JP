---
title: getEffectiveDeviceEnrollmentConfigurations 関数
description: まだ文書化されていません
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 6eb34d4fc1f2855afeaf93fa5fd8878f6896cd0f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35980283"
---
# <a name="geteffectivedeviceenrollmentconfigurations-function"></a><span data-ttu-id="41bc5-103">getEffectiveDeviceEnrollmentConfigurations 関数</span><span class="sxs-lookup"><span data-stu-id="41bc5-103">getEffectiveDeviceEnrollmentConfigurations function</span></span>

> <span data-ttu-id="41bc5-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="41bc5-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="41bc5-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="41bc5-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="41bc5-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="41bc5-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="41bc5-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="41bc5-107">Prerequisites</span></span>
<span data-ttu-id="41bc5-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="41bc5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41bc5-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="41bc5-110">Permission type</span></span>|<span data-ttu-id="41bc5-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="41bc5-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="41bc5-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="41bc5-112">Delegated (work or school account)</span></span>|<span data-ttu-id="41bc5-113">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="41bc5-113">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="41bc5-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="41bc5-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="41bc5-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="41bc5-115">Not supported.</span></span>|
|<span data-ttu-id="41bc5-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="41bc5-116">Application</span></span>|<span data-ttu-id="41bc5-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="41bc5-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="41bc5-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="41bc5-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/getEffectiveDeviceEnrollmentConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="41bc5-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="41bc5-119">Request headers</span></span>
|<span data-ttu-id="41bc5-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="41bc5-120">Header</span></span>|<span data-ttu-id="41bc5-121">値</span><span class="sxs-lookup"><span data-stu-id="41bc5-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="41bc5-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="41bc5-122">Authorization</span></span>|<span data-ttu-id="41bc5-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="41bc5-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="41bc5-124">承諾</span><span class="sxs-lookup"><span data-stu-id="41bc5-124">Accept</span></span>|<span data-ttu-id="41bc5-125">application/json</span><span class="sxs-lookup"><span data-stu-id="41bc5-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="41bc5-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="41bc5-126">Request body</span></span>
<span data-ttu-id="41bc5-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="41bc5-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="41bc5-128">応答</span><span class="sxs-lookup"><span data-stu-id="41bc5-128">Response</span></span>
<span data-ttu-id="41bc5-129">成功した場合、この関数`200 OK`は応答コードと、応答本文で[deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md)コレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="41bc5-129">If successful, this function returns a `200 OK` response code and a [deviceEnrollmentConfiguration](../resources/intune-onboarding-deviceenrollmentconfiguration.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="41bc5-130">例</span><span class="sxs-lookup"><span data-stu-id="41bc5-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="41bc5-131">要求</span><span class="sxs-lookup"><span data-stu-id="41bc5-131">Request</span></span>
<span data-ttu-id="41bc5-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="41bc5-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/getEffectiveDeviceEnrollmentConfigurations
```

### <a name="response"></a><span data-ttu-id="41bc5-133">応答</span><span class="sxs-lookup"><span data-stu-id="41bc5-133">Response</span></span>
<span data-ttu-id="41bc5-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="41bc5-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





