---
title: DeviceManagementIntentUserStates のリスト
description: DeviceManagementIntentUserState オブジェクトのプロパティとリレーションシップをリストします。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 54a46b5c55f7674f6415c1c4a51b743562cce1e9
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36347630"
---
# <a name="list-devicemanagementintentuserstates"></a><span data-ttu-id="442cc-103">DeviceManagementIntentUserStates のリスト</span><span class="sxs-lookup"><span data-stu-id="442cc-103">List deviceManagementIntentUserStates</span></span>

> <span data-ttu-id="442cc-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="442cc-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="442cc-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="442cc-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="442cc-106">[Devicemanagementintentuserstate](../resources/intune-deviceintent-devicemanagementintentuserstate.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="442cc-106">List properties and relationships of the [deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="442cc-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="442cc-107">Prerequisites</span></span>
<span data-ttu-id="442cc-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="442cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="442cc-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="442cc-110">Permission type</span></span>|<span data-ttu-id="442cc-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="442cc-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="442cc-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="442cc-112">Delegated (work or school account)</span></span>|<span data-ttu-id="442cc-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="442cc-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="442cc-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="442cc-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="442cc-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="442cc-115">Not supported.</span></span>|
|<span data-ttu-id="442cc-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="442cc-116">Application</span></span>|<span data-ttu-id="442cc-117">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="442cc-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="442cc-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="442cc-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intents/{deviceManagementIntentId}/userStates
```

## <a name="request-headers"></a><span data-ttu-id="442cc-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="442cc-119">Request headers</span></span>
|<span data-ttu-id="442cc-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="442cc-120">Header</span></span>|<span data-ttu-id="442cc-121">値</span><span class="sxs-lookup"><span data-stu-id="442cc-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="442cc-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="442cc-122">Authorization</span></span>|<span data-ttu-id="442cc-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="442cc-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="442cc-124">承諾</span><span class="sxs-lookup"><span data-stu-id="442cc-124">Accept</span></span>|<span data-ttu-id="442cc-125">application/json</span><span class="sxs-lookup"><span data-stu-id="442cc-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="442cc-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="442cc-126">Request body</span></span>
<span data-ttu-id="442cc-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="442cc-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="442cc-128">応答</span><span class="sxs-lookup"><span data-stu-id="442cc-128">Response</span></span>
<span data-ttu-id="442cc-129">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[Devicemanagementintentuserstate](../resources/intune-deviceintent-devicemanagementintentuserstate.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="442cc-129">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="442cc-130">例</span><span class="sxs-lookup"><span data-stu-id="442cc-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="442cc-131">要求</span><span class="sxs-lookup"><span data-stu-id="442cc-131">Request</span></span>
<span data-ttu-id="442cc-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="442cc-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intents/{deviceManagementIntentId}/userStates
```

### <a name="response"></a><span data-ttu-id="442cc-133">応答</span><span class="sxs-lookup"><span data-stu-id="442cc-133">Response</span></span>
<span data-ttu-id="442cc-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="442cc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 385

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementIntentUserState",
      "id": "0201286a-286a-0201-6a28-01026a280102",
      "userPrincipalName": "User Principal Name value",
      "userName": "User Name value",
      "deviceCount": 11,
      "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
      "state": "notApplicable"
    }
  ]
}
```






