---
title: syncLicenses アクション
description: 特定の appleVolumePurchaseProgramToken に関連付けられたライセンスを同期します
author: tfitzmac
ms.openlocfilehash: 541d974666988a165293f8e4241d0a15d712209a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27336604"
---
# <a name="synclicenses-action"></a><span data-ttu-id="aa986-103">syncLicenses アクション</span><span class="sxs-lookup"><span data-stu-id="aa986-103">syncLicenses action</span></span>

> <span data-ttu-id="aa986-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="aa986-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="aa986-105">特定の appleVolumePurchaseProgramToken に関連付けられたライセンスを同期します</span><span class="sxs-lookup"><span data-stu-id="aa986-105">Syncs licenses associated with a specific appleVolumePurchaseProgramToken</span></span>
## <a name="prerequisites"></a><span data-ttu-id="aa986-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="aa986-106">Prerequisites</span></span>
<span data-ttu-id="aa986-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="aa986-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aa986-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="aa986-109">Permission type</span></span>|<span data-ttu-id="aa986-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="aa986-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aa986-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="aa986-111">Delegated (work or school account)</span></span>|<span data-ttu-id="aa986-112">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aa986-112">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="aa986-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="aa986-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aa986-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="aa986-114">Not supported.</span></span>|
|<span data-ttu-id="aa986-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="aa986-115">Application</span></span>|<span data-ttu-id="aa986-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="aa986-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="aa986-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="aa986-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/vppTokens/{vppTokenId}/syncLicenses
```

## <a name="request-headers"></a><span data-ttu-id="aa986-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="aa986-118">Request headers</span></span>
|<span data-ttu-id="aa986-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="aa986-119">Header</span></span>|<span data-ttu-id="aa986-120">値</span><span class="sxs-lookup"><span data-stu-id="aa986-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aa986-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="aa986-121">Authorization</span></span>|<span data-ttu-id="aa986-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="aa986-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aa986-123">Accept</span><span class="sxs-lookup"><span data-stu-id="aa986-123">Accept</span></span>|<span data-ttu-id="aa986-124">application/json</span><span class="sxs-lookup"><span data-stu-id="aa986-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aa986-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="aa986-125">Request body</span></span>
<span data-ttu-id="aa986-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="aa986-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aa986-127">応答</span><span class="sxs-lookup"><span data-stu-id="aa986-127">Response</span></span>
<span data-ttu-id="aa986-128">成功した場合、このアクションは `200 OK` 応答コードと、応答本文で [vppToken](../resources/intune-onboarding-vpptoken.md) を返します。</span><span class="sxs-lookup"><span data-stu-id="aa986-128">If successful, this action returns a `200 OK` response code and a [vppToken](../resources/intune-onboarding-vpptoken.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aa986-129">例</span><span class="sxs-lookup"><span data-stu-id="aa986-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="aa986-130">要求</span><span class="sxs-lookup"><span data-stu-id="aa986-130">Request</span></span>
<span data-ttu-id="aa986-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="aa986-131">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/vppTokens/{vppTokenId}/syncLicenses
```

### <a name="response"></a><span data-ttu-id="aa986-132">応答</span><span class="sxs-lookup"><span data-stu-id="aa986-132">Response</span></span>
<span data-ttu-id="aa986-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="aa986-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 619

{
  "value": {
    "@odata.type": "#microsoft.graph.vppToken",
    "id": "9ceb2f92-2f92-9ceb-922f-eb9c922feb9c",
    "organizationName": "Organization Name value",
    "vppTokenAccountType": "education",
    "appleId": "Apple Id value",
    "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00",
    "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
    "token": "Token value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "state": "valid",
    "lastSyncStatus": "inProgress",
    "automaticallyUpdateApps": true,
    "countryOrRegion": "Country Or Region value"
  }
}
```


