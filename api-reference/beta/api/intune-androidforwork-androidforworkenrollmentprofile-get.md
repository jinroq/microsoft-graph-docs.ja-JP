---
title: androidForWorkEnrollmentProfile の取得
description: androidForWorkEnrollmentProfile オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9e1fb1987c8cc6dfadf8ec0e510ecb89d6b7cb31
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32498845"
---
# <a name="get-androidforworkenrollmentprofile"></a><span data-ttu-id="c9fb4-103">androidForWorkEnrollmentProfile の取得</span><span class="sxs-lookup"><span data-stu-id="c9fb4-103">Get androidForWorkEnrollmentProfile</span></span>

> <span data-ttu-id="c9fb4-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c9fb4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c9fb4-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="c9fb4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c9fb4-106">[androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="c9fb4-106">Read properties and relationships of the [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c9fb4-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="c9fb4-107">Prerequisites</span></span>
<span data-ttu-id="c9fb4-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c9fb4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c9fb4-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c9fb4-110">Permission type</span></span>|<span data-ttu-id="c9fb4-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="c9fb4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c9fb4-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c9fb4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c9fb4-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="c9fb4-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="c9fb4-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c9fb4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c9fb4-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c9fb4-115">Not supported.</span></span>|
|<span data-ttu-id="c9fb4-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c9fb4-116">Application</span></span>|<span data-ttu-id="c9fb4-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c9fb4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c9fb4-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c9fb4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/androidForWorkEnrollmentProfiles/{androidForWorkEnrollmentProfileId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c9fb4-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="c9fb4-119">Optional query parameters</span></span>
<span data-ttu-id="c9fb4-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="c9fb4-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c9fb4-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c9fb4-121">Request headers</span></span>
|<span data-ttu-id="c9fb4-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c9fb4-122">Header</span></span>|<span data-ttu-id="c9fb4-123">値</span><span class="sxs-lookup"><span data-stu-id="c9fb4-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c9fb4-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="c9fb4-124">Authorization</span></span>|<span data-ttu-id="c9fb4-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="c9fb4-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c9fb4-126">承諾</span><span class="sxs-lookup"><span data-stu-id="c9fb4-126">Accept</span></span>|<span data-ttu-id="c9fb4-127">application/json</span><span class="sxs-lookup"><span data-stu-id="c9fb4-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c9fb4-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="c9fb4-128">Request body</span></span>
<span data-ttu-id="c9fb4-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="c9fb4-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c9fb4-130">応答</span><span class="sxs-lookup"><span data-stu-id="c9fb4-130">Response</span></span>
<span data-ttu-id="c9fb4-131">このメソッドが成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="c9fb4-131">If successful, this method returns a `200 OK` response code and [androidForWorkEnrollmentProfile](../resources/intune-androidforwork-androidforworkenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c9fb4-132">例</span><span class="sxs-lookup"><span data-stu-id="c9fb4-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="c9fb4-133">要求</span><span class="sxs-lookup"><span data-stu-id="c9fb4-133">Request</span></span>
<span data-ttu-id="c9fb4-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c9fb4-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/androidForWorkEnrollmentProfiles/{androidForWorkEnrollmentProfileId}
```

### <a name="response"></a><span data-ttu-id="c9fb4-135">応答</span><span class="sxs-lookup"><span data-stu-id="c9fb4-135">Response</span></span>
<span data-ttu-id="c9fb4-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c9fb4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 719

{
  "value": {
    "@odata.type": "#microsoft.graph.androidForWorkEnrollmentProfile",
    "accountId": "Account Id value",
    "id": "e6742553-2553-e674-5325-74e6532574e6",
    "displayName": "Display Name value",
    "description": "Description value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "tokenValue": "Token Value value",
    "tokenExpirationDateTime": "2016-12-31T23:59:54.0590989-08:00",
    "enrolledDeviceCount": 3,
    "qrCodeContent": "Qr Code Content value",
    "qrCodeImage": {
      "@odata.type": "microsoft.graph.mimeContent",
      "type": "Type value",
      "value": "dmFsdWU="
    }
  }
}
```





