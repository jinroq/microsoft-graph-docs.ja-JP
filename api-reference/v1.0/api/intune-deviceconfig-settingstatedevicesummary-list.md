---
title: settingStateDeviceSummaries のリスト
description: settingStateDeviceSummary オブジェクトのプロパティとリレーションシップをリストします。
ms.openlocfilehash: 390af97482f0499923cad7850801eb2181de47ab
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27024080"
---
# <a name="list-settingstatedevicesummaries"></a><span data-ttu-id="1aba4-103">settingStateDeviceSummaries のリスト</span><span class="sxs-lookup"><span data-stu-id="1aba4-103">List settingStateDeviceSummaries</span></span>

> <span data-ttu-id="1aba4-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="1aba4-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1aba4-105">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="1aba4-105">List properties and relationships of the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1aba4-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="1aba4-106">Prerequisites</span></span>
<span data-ttu-id="1aba4-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1aba4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1aba4-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1aba4-109">Permission type</span></span>|<span data-ttu-id="1aba4-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="1aba4-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1aba4-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1aba4-111">Delegated (work or school account)</span></span>|<span data-ttu-id="1aba4-112">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="1aba4-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="1aba4-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1aba4-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1aba4-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1aba4-114">Not supported.</span></span>|
|<span data-ttu-id="1aba4-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1aba4-115">Application</span></span>|<span data-ttu-id="1aba4-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1aba4-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1aba4-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1aba4-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceSettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="1aba4-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1aba4-118">Request headers</span></span>
|<span data-ttu-id="1aba4-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1aba4-119">Header</span></span>|<span data-ttu-id="1aba4-120">値</span><span class="sxs-lookup"><span data-stu-id="1aba4-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1aba4-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1aba4-121">Authorization</span></span>|<span data-ttu-id="1aba4-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="1aba4-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1aba4-123">Accept</span><span class="sxs-lookup"><span data-stu-id="1aba4-123">Accept</span></span>|<span data-ttu-id="1aba4-124">application/json</span><span class="sxs-lookup"><span data-stu-id="1aba4-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1aba4-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="1aba4-125">Request body</span></span>
<span data-ttu-id="1aba4-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="1aba4-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1aba4-127">応答</span><span class="sxs-lookup"><span data-stu-id="1aba4-127">Response</span></span>
<span data-ttu-id="1aba4-128">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="1aba4-128">If successful, this method returns a `200 OK` response code and a collection of [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1aba4-129">例</span><span class="sxs-lookup"><span data-stu-id="1aba4-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="1aba4-130">要求</span><span class="sxs-lookup"><span data-stu-id="1aba4-130">Request</span></span>
<span data-ttu-id="1aba4-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1aba4-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries
```

### <a name="response"></a><span data-ttu-id="1aba4-132">応答</span><span class="sxs-lookup"><span data-stu-id="1aba4-132">Response</span></span>
<span data-ttu-id="1aba4-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1aba4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 486

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.settingStateDeviceSummary",
      "id": "3e2d4526-4526-3e2d-2645-2d3e26452d3e",
      "settingName": "Setting Name value",
      "instancePath": "Instance Path value",
      "unknownDeviceCount": 2,
      "notApplicableDeviceCount": 8,
      "compliantDeviceCount": 4,
      "remediatedDeviceCount": 5,
      "nonCompliantDeviceCount": 7,
      "errorDeviceCount": 0,
      "conflictDeviceCount": 3
    }
  ]
}
```


