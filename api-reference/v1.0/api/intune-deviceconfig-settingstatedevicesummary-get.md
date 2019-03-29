---
title: Get settingStateDeviceSummary
description: settingStateDeviceSummary オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0957e81ecb901eb2c88dc59603b3c62bab7cd393
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30971830"
---
# <a name="get-settingstatedevicesummary"></a><span data-ttu-id="d2d20-103">Get settingStateDeviceSummary</span><span class="sxs-lookup"><span data-stu-id="d2d20-103">Get settingStateDeviceSummary</span></span>

> <span data-ttu-id="d2d20-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d2d20-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d2d20-105">[settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="d2d20-105">Read properties and relationships of the [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d2d20-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="d2d20-106">Prerequisites</span></span>
<span data-ttu-id="d2d20-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d2d20-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d2d20-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d2d20-109">Permission type</span></span>|<span data-ttu-id="d2d20-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="d2d20-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d2d20-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d2d20-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d2d20-112">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d2d20-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="d2d20-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d2d20-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d2d20-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d2d20-114">Not supported.</span></span>|
|<span data-ttu-id="d2d20-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d2d20-115">Application</span></span>|<span data-ttu-id="d2d20-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d2d20-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d2d20-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d2d20-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d2d20-118">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="d2d20-118">Optional query parameters</span></span>
<span data-ttu-id="d2d20-119">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="d2d20-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d2d20-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d2d20-120">Request headers</span></span>
|<span data-ttu-id="d2d20-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d2d20-121">Header</span></span>|<span data-ttu-id="d2d20-122">値</span><span class="sxs-lookup"><span data-stu-id="d2d20-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d2d20-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d2d20-123">Authorization</span></span>|<span data-ttu-id="d2d20-124">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="d2d20-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d2d20-125">承諾</span><span class="sxs-lookup"><span data-stu-id="d2d20-125">Accept</span></span>|<span data-ttu-id="d2d20-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d2d20-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d2d20-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="d2d20-127">Request body</span></span>
<span data-ttu-id="d2d20-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="d2d20-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d2d20-129">応答</span><span class="sxs-lookup"><span data-stu-id="d2d20-129">Response</span></span>
<span data-ttu-id="d2d20-130">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d2d20-130">If successful, this method returns a `200 OK` response code and [settingStateDeviceSummary](../resources/intune-deviceconfig-settingstatedevicesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d2d20-131">例</span><span class="sxs-lookup"><span data-stu-id="d2d20-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="d2d20-132">要求</span><span class="sxs-lookup"><span data-stu-id="d2d20-132">Request</span></span>
<span data-ttu-id="d2d20-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d2d20-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}/deviceSettingStateSummaries/{settingStateDeviceSummaryId}
```

### <a name="response"></a><span data-ttu-id="d2d20-134">応答</span><span class="sxs-lookup"><span data-stu-id="d2d20-134">Response</span></span>
<span data-ttu-id="d2d20-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d2d20-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



