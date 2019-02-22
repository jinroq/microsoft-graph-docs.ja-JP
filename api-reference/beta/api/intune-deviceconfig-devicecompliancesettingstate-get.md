---
title: Get deviceComplianceSettingState
description: deviceComplianceSettingState オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b7e446e051474b2b911221cbb0090c8ebbace1db
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30158605"
---
# <a name="get-devicecompliancesettingstate"></a><span data-ttu-id="b7a83-103">Get deviceComplianceSettingState</span><span class="sxs-lookup"><span data-stu-id="b7a83-103">Get deviceComplianceSettingState</span></span>

> <span data-ttu-id="b7a83-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b7a83-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b7a83-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b7a83-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b7a83-106">[deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="b7a83-106">Read properties and relationships of the [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b7a83-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="b7a83-107">Prerequisites</span></span>
<span data-ttu-id="b7a83-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b7a83-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b7a83-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b7a83-110">Permission type</span></span>|<span data-ttu-id="b7a83-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="b7a83-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b7a83-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b7a83-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b7a83-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b7a83-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="b7a83-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b7a83-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b7a83-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b7a83-115">Not supported.</span></span>|
|<span data-ttu-id="b7a83-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b7a83-116">Application</span></span>|<span data-ttu-id="b7a83-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b7a83-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b7a83-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b7a83-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates/{deviceComplianceSettingStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b7a83-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="b7a83-119">Optional query parameters</span></span>
<span data-ttu-id="b7a83-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="b7a83-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b7a83-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b7a83-121">Request headers</span></span>
|<span data-ttu-id="b7a83-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b7a83-122">Header</span></span>|<span data-ttu-id="b7a83-123">値</span><span class="sxs-lookup"><span data-stu-id="b7a83-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b7a83-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="b7a83-124">Authorization</span></span>|<span data-ttu-id="b7a83-125">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="b7a83-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b7a83-126">承諾</span><span class="sxs-lookup"><span data-stu-id="b7a83-126">Accept</span></span>|<span data-ttu-id="b7a83-127">application/json</span><span class="sxs-lookup"><span data-stu-id="b7a83-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b7a83-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="b7a83-128">Request body</span></span>
<span data-ttu-id="b7a83-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="b7a83-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b7a83-130">応答</span><span class="sxs-lookup"><span data-stu-id="b7a83-130">Response</span></span>
<span data-ttu-id="b7a83-131">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="b7a83-131">If successful, this method returns a `200 OK` response code and [deviceComplianceSettingState](../resources/intune-deviceconfig-devicecompliancesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b7a83-132">例</span><span class="sxs-lookup"><span data-stu-id="b7a83-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="b7a83-133">要求</span><span class="sxs-lookup"><span data-stu-id="b7a83-133">Request</span></span>
<span data-ttu-id="b7a83-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b7a83-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicySettingStateSummaries/{deviceCompliancePolicySettingStateSummaryId}/deviceComplianceSettingStates/{deviceComplianceSettingStateId}
```

### <a name="response"></a><span data-ttu-id="b7a83-135">応答</span><span class="sxs-lookup"><span data-stu-id="b7a83-135">Response</span></span>
<span data-ttu-id="b7a83-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b7a83-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 645

{
  "value": {
    "@odata.type": "#microsoft.graph.deviceComplianceSettingState",
    "id": "9905f955-f955-9905-55f9-059955f90599",
    "platformType": "windowsRT",
    "setting": "Setting value",
    "settingName": "Setting Name value",
    "deviceId": "Device Id value",
    "deviceName": "Device Name value",
    "userId": "User Id value",
    "userEmail": "User Email value",
    "userName": "User Name value",
    "userPrincipalName": "User Principal Name value",
    "deviceModel": "Device Model value",
    "state": "notApplicable",
    "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00"
  }
}
```




