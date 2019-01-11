---
title: windowsInformationProtectionNetworkLearningSummaries のリスト
description: windowsInformationProtectionNetworkLearningSummary オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 9b18e6c3a810fc2abe633ad1096ab9221cf379df
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27839194"
---
# <a name="list-windowsinformationprotectionnetworklearningsummaries"></a><span data-ttu-id="6b8a0-103">windowsInformationProtectionNetworkLearningSummaries のリスト</span><span class="sxs-lookup"><span data-stu-id="6b8a0-103">List windowsInformationProtectionNetworkLearningSummaries</span></span>

> <span data-ttu-id="6b8a0-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="6b8a0-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6b8a0-105">[windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="6b8a0-105">List properties and relationships of the [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6b8a0-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="6b8a0-106">Prerequisites</span></span>
<span data-ttu-id="6b8a0-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6b8a0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6b8a0-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6b8a0-109">Permission type</span></span>|<span data-ttu-id="6b8a0-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="6b8a0-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6b8a0-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6b8a0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6b8a0-112">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="6b8a0-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="6b8a0-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6b8a0-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6b8a0-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6b8a0-114">Not supported.</span></span>|
|<span data-ttu-id="6b8a0-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6b8a0-115">Application</span></span>|<span data-ttu-id="6b8a0-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6b8a0-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6b8a0-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6b8a0-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsInformationProtectionNetworkLearningSummaries
```

## <a name="request-headers"></a><span data-ttu-id="6b8a0-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6b8a0-118">Request headers</span></span>
|<span data-ttu-id="6b8a0-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6b8a0-119">Header</span></span>|<span data-ttu-id="6b8a0-120">値</span><span class="sxs-lookup"><span data-stu-id="6b8a0-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6b8a0-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6b8a0-121">Authorization</span></span>|<span data-ttu-id="6b8a0-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="6b8a0-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6b8a0-123">Accept</span><span class="sxs-lookup"><span data-stu-id="6b8a0-123">Accept</span></span>|<span data-ttu-id="6b8a0-124">application/json</span><span class="sxs-lookup"><span data-stu-id="6b8a0-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6b8a0-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="6b8a0-125">Request body</span></span>
<span data-ttu-id="6b8a0-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="6b8a0-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6b8a0-127">応答</span><span class="sxs-lookup"><span data-stu-id="6b8a0-127">Response</span></span>
<span data-ttu-id="6b8a0-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="6b8a0-128">If successful, this method returns a `200 OK` response code and a collection of [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6b8a0-129">例</span><span class="sxs-lookup"><span data-stu-id="6b8a0-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="6b8a0-130">要求</span><span class="sxs-lookup"><span data-stu-id="6b8a0-130">Request</span></span>
<span data-ttu-id="6b8a0-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6b8a0-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/windowsInformationProtectionNetworkLearningSummaries
```

### <a name="response"></a><span data-ttu-id="6b8a0-132">応答</span><span class="sxs-lookup"><span data-stu-id="6b8a0-132">Response</span></span>
<span data-ttu-id="6b8a0-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="6b8a0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 235

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsInformationProtectionNetworkLearningSummary",
      "id": "242108f7-08f7-2421-f708-2124f7082124",
      "url": "Url value",
      "deviceCount": 11
    }
  ]
}
```



