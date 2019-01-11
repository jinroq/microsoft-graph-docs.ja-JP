---
title: Get settingStateDeviceSummary
description: settingStateDeviceSummary オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b174e5e262d554493cc1bca11b97e0157b16cb7d
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27811257"
---
# <a name="get-settingstatedevicesummary"></a><span data-ttu-id="87029-103">Get settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="87029-103">Get settingStateDeviceSummary</span></span>

> <span data-ttu-id="87029-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="87029-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="87029-105">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="87029-105">Read properties and relationships of the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="87029-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="87029-106">Prerequisites</span></span>
<span data-ttu-id="87029-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="87029-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="87029-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="87029-109">Permission type</span></span>|<span data-ttu-id="87029-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="87029-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="87029-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="87029-111">Delegated (work or school account)</span></span>|<span data-ttu-id="87029-112">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="87029-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="87029-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="87029-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="87029-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="87029-114">Not supported.</span></span>|
|<span data-ttu-id="87029-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="87029-115">Application</span></span>|<span data-ttu-id="87029-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="87029-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="87029-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="87029-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="87029-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="87029-118">Optional query parameters</span></span>
<span data-ttu-id="87029-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="87029-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="87029-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="87029-120">Request headers</span></span>
|<span data-ttu-id="87029-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="87029-121">Header</span></span>|<span data-ttu-id="87029-122">値</span><span class="sxs-lookup"><span data-stu-id="87029-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="87029-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="87029-123">Authorization</span></span>|<span data-ttu-id="87029-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="87029-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="87029-125">Accept</span><span class="sxs-lookup"><span data-stu-id="87029-125">Accept</span></span>|<span data-ttu-id="87029-126">application/json</span><span class="sxs-lookup"><span data-stu-id="87029-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="87029-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="87029-127">Request body</span></span>
<span data-ttu-id="87029-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="87029-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="87029-129">応答</span><span class="sxs-lookup"><span data-stu-id="87029-129">Response</span></span>
<span data-ttu-id="87029-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="87029-130">If successful, this method returns a `200 OK` response code and [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="87029-131">例</span><span class="sxs-lookup"><span data-stu-id="87029-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="87029-132">要求</span><span class="sxs-lookup"><span data-stu-id="87029-132">Request</span></span>
<span data-ttu-id="87029-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="87029-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
```

### <a name="response"></a><span data-ttu-id="87029-134">応答</span><span class="sxs-lookup"><span data-stu-id="87029-134">Response</span></span>
<span data-ttu-id="87029-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="87029-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 450

{
  "value": {
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
}
```



