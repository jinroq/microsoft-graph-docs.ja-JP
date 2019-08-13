---
title: AndroidDeviceOwnerEnrollmentProfile を取得する
description: AndroidDeviceOwnerEnrollmentProfile オブジェクトのプロパティとリレーションシップを読み取ります。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b69e5b3a4b9c726a73ee2dc152054c86d7520e0d
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36325181"
---
# <a name="get-androiddeviceownerenrollmentprofile"></a><span data-ttu-id="5bb0b-103">AndroidDeviceOwnerEnrollmentProfile を取得する</span><span class="sxs-lookup"><span data-stu-id="5bb0b-103">Get androidDeviceOwnerEnrollmentProfile</span></span>

> <span data-ttu-id="5bb0b-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5bb0b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5bb0b-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="5bb0b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5bb0b-106">[AndroidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="5bb0b-106">Read properties and relationships of the [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5bb0b-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="5bb0b-107">Prerequisites</span></span>
<span data-ttu-id="5bb0b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5bb0b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5bb0b-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5bb0b-110">Permission type</span></span>|<span data-ttu-id="5bb0b-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="5bb0b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5bb0b-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5bb0b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="5bb0b-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5bb0b-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="5bb0b-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5bb0b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5bb0b-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5bb0b-115">Not supported.</span></span>|
|<span data-ttu-id="5bb0b-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5bb0b-116">Application</span></span>|<span data-ttu-id="5bb0b-117">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5bb0b-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5bb0b-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5bb0b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/androidDeviceOwnerEnrollmentProfiles/{androidDeviceOwnerEnrollmentProfileId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5bb0b-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="5bb0b-119">Optional query parameters</span></span>
<span data-ttu-id="5bb0b-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="5bb0b-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5bb0b-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5bb0b-121">Request headers</span></span>
|<span data-ttu-id="5bb0b-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5bb0b-122">Header</span></span>|<span data-ttu-id="5bb0b-123">値</span><span class="sxs-lookup"><span data-stu-id="5bb0b-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5bb0b-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="5bb0b-124">Authorization</span></span>|<span data-ttu-id="5bb0b-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="5bb0b-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5bb0b-126">承諾</span><span class="sxs-lookup"><span data-stu-id="5bb0b-126">Accept</span></span>|<span data-ttu-id="5bb0b-127">application/json</span><span class="sxs-lookup"><span data-stu-id="5bb0b-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5bb0b-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="5bb0b-128">Request body</span></span>
<span data-ttu-id="5bb0b-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="5bb0b-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5bb0b-130">応答</span><span class="sxs-lookup"><span data-stu-id="5bb0b-130">Response</span></span>
<span data-ttu-id="5bb0b-131">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="5bb0b-131">If successful, this method returns a `200 OK` response code and [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5bb0b-132">例</span><span class="sxs-lookup"><span data-stu-id="5bb0b-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="5bb0b-133">要求</span><span class="sxs-lookup"><span data-stu-id="5bb0b-133">Request</span></span>
<span data-ttu-id="5bb0b-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5bb0b-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/androidDeviceOwnerEnrollmentProfiles/{androidDeviceOwnerEnrollmentProfileId}
```

### <a name="response"></a><span data-ttu-id="5bb0b-135">応答</span><span class="sxs-lookup"><span data-stu-id="5bb0b-135">Response</span></span>
<span data-ttu-id="5bb0b-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="5bb0b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 858

{
  "value": {
    "@odata.type": "#microsoft.graph.androidDeviceOwnerEnrollmentProfile",
    "accountId": "Account Id value",
    "id": "a8d0245e-245e-a8d0-5e24-d0a85e24d0a8",
    "displayName": "Display Name value",
    "description": "Description value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "tokenValue": "Token Value value",
    "tokenCreationDateTime": "2017-01-01T00:01:38.5314127-08:00",
    "tokenExpirationDateTime": "2016-12-31T23:59:54.0590989-08:00",
    "enrolledDeviceCount": 3,
    "qrCodeContent": "Qr Code Content value",
    "qrCodeImage": {
      "@odata.type": "microsoft.graph.mimeContent",
      "type": "Type value",
      "value": "dmFsdWU="
    },
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ]
  }
}
```






