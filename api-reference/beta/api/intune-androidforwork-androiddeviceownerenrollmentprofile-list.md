---
title: リスト androidDeviceOwnerEnrollmentProfiles
description: AndroidDeviceOwnerEnrollmentProfile オブジェクトのプロパティとリレーションシップをリストします。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 42607d093d12758d4e86aaa9697b1575ef548f97
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35952927"
---
# <a name="list-androiddeviceownerenrollmentprofiles"></a><span data-ttu-id="60a03-103">リスト androidDeviceOwnerEnrollmentProfiles</span><span class="sxs-lookup"><span data-stu-id="60a03-103">List androidDeviceOwnerEnrollmentProfiles</span></span>

> <span data-ttu-id="60a03-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="60a03-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="60a03-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="60a03-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="60a03-106">[AndroidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="60a03-106">List properties and relationships of the [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="60a03-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="60a03-107">Prerequisites</span></span>
<span data-ttu-id="60a03-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="60a03-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="60a03-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="60a03-110">Permission type</span></span>|<span data-ttu-id="60a03-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="60a03-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="60a03-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="60a03-112">Delegated (work or school account)</span></span>|<span data-ttu-id="60a03-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="60a03-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="60a03-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="60a03-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="60a03-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="60a03-115">Not supported.</span></span>|
|<span data-ttu-id="60a03-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="60a03-116">Application</span></span>|<span data-ttu-id="60a03-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="60a03-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="60a03-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="60a03-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/androidDeviceOwnerEnrollmentProfiles
```

## <a name="request-headers"></a><span data-ttu-id="60a03-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="60a03-119">Request headers</span></span>
|<span data-ttu-id="60a03-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="60a03-120">Header</span></span>|<span data-ttu-id="60a03-121">値</span><span class="sxs-lookup"><span data-stu-id="60a03-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="60a03-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="60a03-122">Authorization</span></span>|<span data-ttu-id="60a03-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="60a03-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="60a03-124">承諾</span><span class="sxs-lookup"><span data-stu-id="60a03-124">Accept</span></span>|<span data-ttu-id="60a03-125">application/json</span><span class="sxs-lookup"><span data-stu-id="60a03-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="60a03-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="60a03-126">Request body</span></span>
<span data-ttu-id="60a03-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="60a03-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="60a03-128">応答</span><span class="sxs-lookup"><span data-stu-id="60a03-128">Response</span></span>
<span data-ttu-id="60a03-129">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="60a03-129">If successful, this method returns a `200 OK` response code and a collection of [androidDeviceOwnerEnrollmentProfile](../resources/intune-androidforwork-androiddeviceownerenrollmentprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="60a03-130">例</span><span class="sxs-lookup"><span data-stu-id="60a03-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="60a03-131">要求</span><span class="sxs-lookup"><span data-stu-id="60a03-131">Request</span></span>
<span data-ttu-id="60a03-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="60a03-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/androidDeviceOwnerEnrollmentProfiles
```

### <a name="response"></a><span data-ttu-id="60a03-133">応答</span><span class="sxs-lookup"><span data-stu-id="60a03-133">Response</span></span>
<span data-ttu-id="60a03-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="60a03-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 898

{
  "value": [
    {
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
      "scopeTags": [
        "Scope Tags value"
      ]
    }
  ]
}
```





