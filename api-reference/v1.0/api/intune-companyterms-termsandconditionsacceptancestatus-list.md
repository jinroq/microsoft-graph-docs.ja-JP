---
title: termsAndConditionsAcceptanceStatuses のリスト
description: termsAndConditionsAcceptanceStatus オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a5c1da79f59c1d12e6703906acc24eab06c63175
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36019850"
---
# <a name="list-termsandconditionsacceptancestatuses"></a><span data-ttu-id="1288a-103">termsAndConditionsAcceptanceStatuses のリスト</span><span class="sxs-lookup"><span data-stu-id="1288a-103">List termsAndConditionsAcceptanceStatuses</span></span>

> <span data-ttu-id="1288a-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="1288a-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1288a-105">[termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="1288a-105">List properties and relationships of the [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1288a-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="1288a-106">Prerequisites</span></span>
<span data-ttu-id="1288a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1288a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1288a-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1288a-109">Permission type</span></span>|<span data-ttu-id="1288a-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="1288a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1288a-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1288a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1288a-112">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="1288a-112">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="1288a-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1288a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1288a-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1288a-114">Not supported.</span></span>|
|<span data-ttu-id="1288a-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1288a-115">Application</span></span>|<span data-ttu-id="1288a-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1288a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1288a-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1288a-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses
```

## <a name="request-headers"></a><span data-ttu-id="1288a-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1288a-118">Request headers</span></span>
|<span data-ttu-id="1288a-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1288a-119">Header</span></span>|<span data-ttu-id="1288a-120">値</span><span class="sxs-lookup"><span data-stu-id="1288a-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1288a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1288a-121">Authorization</span></span>|<span data-ttu-id="1288a-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="1288a-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1288a-123">承諾</span><span class="sxs-lookup"><span data-stu-id="1288a-123">Accept</span></span>|<span data-ttu-id="1288a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="1288a-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1288a-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="1288a-125">Request body</span></span>
<span data-ttu-id="1288a-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="1288a-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1288a-127">応答</span><span class="sxs-lookup"><span data-stu-id="1288a-127">Response</span></span>
<span data-ttu-id="1288a-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="1288a-128">If successful, this method returns a `200 OK` response code and a collection of [termsAndConditionsAcceptanceStatus](../resources/intune-companyterms-termsandconditionsacceptancestatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1288a-129">例</span><span class="sxs-lookup"><span data-stu-id="1288a-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="1288a-130">要求</span><span class="sxs-lookup"><span data-stu-id="1288a-130">Request</span></span>
<span data-ttu-id="1288a-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1288a-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/termsAndConditions/{termsAndConditionsId}/acceptanceStatuses
```

### <a name="response"></a><span data-ttu-id="1288a-132">応答</span><span class="sxs-lookup"><span data-stu-id="1288a-132">Response</span></span>
<span data-ttu-id="1288a-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1288a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



