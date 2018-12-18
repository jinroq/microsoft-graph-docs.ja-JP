---
title: termsAndConditionsAcceptanceStatuses のリスト
description: termsAndConditionsAcceptanceStatus オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
ms.openlocfilehash: 6c538d331dfaedde5c2cabe483f5860a1c53e56d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27343254"
---
# <a name="list-termsandconditionsacceptancestatuses"></a><span data-ttu-id="6b945-103">termsAndConditionsAcceptanceStatuses のリスト</span><span class="sxs-lookup"><span data-stu-id="6b945-103">List termsAndConditionsAcceptanceStatuses</span></span>

> <span data-ttu-id="6b945-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6b945-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6b945-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6b945-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6b945-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="6b945-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6b945-107">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="6b945-107">List properties and relationships of the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6b945-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="6b945-108">Prerequisites</span></span>
<span data-ttu-id="6b945-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6b945-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6b945-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6b945-111">Permission type</span></span>|<span data-ttu-id="6b945-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="6b945-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6b945-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6b945-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6b945-114">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="6b945-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="6b945-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6b945-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6b945-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6b945-116">Not supported.</span></span>|
|<span data-ttu-id="6b945-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6b945-117">Application</span></span>|<span data-ttu-id="6b945-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6b945-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6b945-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6b945-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="6b945-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6b945-120">Request headers</span></span>
|<span data-ttu-id="6b945-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6b945-121">Header</span></span>|<span data-ttu-id="6b945-122">値</span><span class="sxs-lookup"><span data-stu-id="6b945-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6b945-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6b945-123">Authorization</span></span>|<span data-ttu-id="6b945-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="6b945-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6b945-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6b945-125">Accept</span></span>|<span data-ttu-id="6b945-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6b945-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6b945-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="6b945-127">Request body</span></span>
<span data-ttu-id="6b945-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="6b945-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6b945-129">応答</span><span class="sxs-lookup"><span data-stu-id="6b945-129">Response</span></span>
<span data-ttu-id="6b945-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="6b945-130">If successful, this method returns a `200 OK` response code and a collection of [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6b945-131">例</span><span class="sxs-lookup"><span data-stu-id="6b945-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="6b945-132">要求</span><span class="sxs-lookup"><span data-stu-id="6b945-132">Request</span></span>
<span data-ttu-id="6b945-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6b945-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses
```

### <a name="response"></a><span data-ttu-id="6b945-134">応答</span><span class="sxs-lookup"><span data-stu-id="6b945-134">Response</span></span>
<span data-ttu-id="6b945-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="6b945-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 313

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.termsAndConditionsAcceptanceStatus",
      "id": "a045ce1a-ce1a-a045-1ace-45a01ace45a0",
      "userDisplayName": "User Display Name value",
      "acceptedVersion": 15,
      "acceptedDateTime": "2016-12-31T23:57:43.6165506-08:00"
    }
  ]
}
```





