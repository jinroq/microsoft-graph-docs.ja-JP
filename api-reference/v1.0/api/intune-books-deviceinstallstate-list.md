---
title: deviceInstallStates のリスト
description: deviceInstallState オブジェクトのプロパティとリレーションシップをリストします。
author: tfitzmac
ms.openlocfilehash: 94c4039e2605ab6139623cfac50343aac5b0b925
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27350786"
---
# <a name="list-deviceinstallstates"></a><span data-ttu-id="8f04a-103">deviceInstallStates のリスト</span><span class="sxs-lookup"><span data-stu-id="8f04a-103">List deviceInstallStates</span></span>

> <span data-ttu-id="8f04a-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="8f04a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="8f04a-105">[deviceInstallState](../resources/intune-books-deviceinstallstate.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="8f04a-105">List properties and relationships of the [deviceInstallState](../resources/intune-books-deviceinstallstate.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="8f04a-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="8f04a-106">Prerequisites</span></span>
<span data-ttu-id="8f04a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8f04a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8f04a-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8f04a-109">Permission type</span></span>|<span data-ttu-id="8f04a-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="8f04a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8f04a-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8f04a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8f04a-112">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="8f04a-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="8f04a-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8f04a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8f04a-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8f04a-114">Not supported.</span></span>|
|<span data-ttu-id="8f04a-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8f04a-115">Application</span></span>|<span data-ttu-id="8f04a-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8f04a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8f04a-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8f04a-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates
GET /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}/deviceStates
```

## <a name="request-headers"></a><span data-ttu-id="8f04a-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8f04a-118">Request headers</span></span>
|<span data-ttu-id="8f04a-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8f04a-119">Header</span></span>|<span data-ttu-id="8f04a-120">値</span><span class="sxs-lookup"><span data-stu-id="8f04a-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8f04a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="8f04a-121">Authorization</span></span>|<span data-ttu-id="8f04a-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="8f04a-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8f04a-123">Accept</span><span class="sxs-lookup"><span data-stu-id="8f04a-123">Accept</span></span>|<span data-ttu-id="8f04a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="8f04a-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8f04a-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="8f04a-125">Request body</span></span>
<span data-ttu-id="8f04a-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="8f04a-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8f04a-127">応答</span><span class="sxs-lookup"><span data-stu-id="8f04a-127">Response</span></span>
<span data-ttu-id="8f04a-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [deviceInstallState](../resources/intune-books-deviceinstallstate.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="8f04a-128">If successful, this method returns a `200 OK` response code and a collection of [deviceInstallState](../resources/intune-books-deviceinstallstate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8f04a-129">例</span><span class="sxs-lookup"><span data-stu-id="8f04a-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="8f04a-130">要求</span><span class="sxs-lookup"><span data-stu-id="8f04a-130">Request</span></span>
<span data-ttu-id="8f04a-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8f04a-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/deviceStates
```

### <a name="response"></a><span data-ttu-id="8f04a-132">応答</span><span class="sxs-lookup"><span data-stu-id="8f04a-132">Response</span></span>
<span data-ttu-id="8f04a-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8f04a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 496

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceInstallState",
      "id": "b9feb68f-b68f-b9fe-8fb6-feb98fb6feb9",
      "deviceName": "Device Name value",
      "deviceId": "Device Id value",
      "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
      "installState": "installed",
      "errorCode": "Error Code value",
      "osVersion": "Os Version value",
      "osDescription": "Os Description value",
      "userName": "User Name value"
    }
  ]
}
```



