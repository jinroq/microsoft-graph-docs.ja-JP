---
title: Get androidForWorkSettings
description: androidForWorkSettings オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 694055193f3ce66843f589637dfe95684009209b
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27946414"
---
# <a name="get-androidforworksettings"></a><span data-ttu-id="23277-103">Get androidForWorkSettings</span><span class="sxs-lookup"><span data-stu-id="23277-103">Get androidForWorkSettings</span></span>

> <span data-ttu-id="23277-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="23277-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="23277-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="23277-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="23277-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="23277-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="23277-107">[androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="23277-107">Read properties and relationships of the [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="23277-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="23277-108">Prerequisites</span></span>
<span data-ttu-id="23277-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="23277-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="23277-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="23277-111">Permission type</span></span>|<span data-ttu-id="23277-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="23277-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="23277-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="23277-113">Delegated (work or school account)</span></span>|<span data-ttu-id="23277-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="23277-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="23277-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="23277-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="23277-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="23277-116">Not supported.</span></span>|
|<span data-ttu-id="23277-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="23277-117">Application</span></span>|<span data-ttu-id="23277-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="23277-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="23277-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="23277-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/androidForWorkSettings
```

## <a name="optional-query-parameters"></a><span data-ttu-id="23277-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="23277-120">Optional query parameters</span></span>
<span data-ttu-id="23277-121">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="23277-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="23277-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="23277-122">Request headers</span></span>
|<span data-ttu-id="23277-123">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="23277-123">Header</span></span>|<span data-ttu-id="23277-124">値</span><span class="sxs-lookup"><span data-stu-id="23277-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="23277-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="23277-125">Authorization</span></span>|<span data-ttu-id="23277-126">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="23277-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="23277-127">Accept</span><span class="sxs-lookup"><span data-stu-id="23277-127">Accept</span></span>|<span data-ttu-id="23277-128">application/json</span><span class="sxs-lookup"><span data-stu-id="23277-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="23277-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="23277-129">Request body</span></span>
<span data-ttu-id="23277-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="23277-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="23277-131">応答</span><span class="sxs-lookup"><span data-stu-id="23277-131">Response</span></span>
<span data-ttu-id="23277-132">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="23277-132">If successful, this method returns a `200 OK` response code and [androidForWorkSettings](../resources/intune-androidforwork-androidforworksettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="23277-133">例</span><span class="sxs-lookup"><span data-stu-id="23277-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="23277-134">要求</span><span class="sxs-lookup"><span data-stu-id="23277-134">Request</span></span>
<span data-ttu-id="23277-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="23277-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/androidForWorkSettings
```

### <a name="response"></a><span data-ttu-id="23277-136">応答</span><span class="sxs-lookup"><span data-stu-id="23277-136">Response</span></span>
<span data-ttu-id="23277-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="23277-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 613

{
  "value": {
    "@odata.type": "#microsoft.graph.androidForWorkSettings",
    "id": "97adc169-c169-97ad-69c1-ad9769c1ad97",
    "bindStatus": "bound",
    "lastAppSyncDateTime": "2016-12-31T23:57:22.8606813-08:00",
    "lastAppSyncStatus": "credentialsNotValid",
    "ownerUserPrincipalName": "Owner User Principal Name value",
    "ownerOrganizationName": "Owner Organization Name value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "enrollmentTarget": "all",
    "targetGroupIds": [
      "Target Group Ids value"
    ],
    "deviceOwnerManagementEnabled": true
  }
}
```





