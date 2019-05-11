---
title: deviceCompliancePolicySettingStateSummaries のリスト
description: deviceCompliancePolicySettingStateSummary オブジェクトのプロパティとリレーションシップをリストします。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fca9b4ac1d58ef4784870403466f871eadb19610
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33927693"
---
# <a name="list-devicecompliancepolicysettingstatesummaries"></a><span data-ttu-id="b9970-103">deviceCompliancePolicySettingStateSummaries のリスト</span><span class="sxs-lookup"><span data-stu-id="b9970-103">List deviceCompliancePolicySettingStateSummaries</span></span>

> <span data-ttu-id="b9970-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b9970-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b9970-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b9970-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b9970-106">[deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="b9970-106">List properties and relationships of the [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b9970-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="b9970-107">Prerequisites</span></span>
<span data-ttu-id="b9970-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b9970-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9970-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="b9970-110">Permission type</span></span>|<span data-ttu-id="b9970-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="b9970-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b9970-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="b9970-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b9970-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b9970-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="b9970-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="b9970-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b9970-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b9970-115">Not supported.</span></span>|
|<span data-ttu-id="b9970-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="b9970-116">Application</span></span>|<span data-ttu-id="b9970-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b9970-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b9970-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="b9970-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicySettingStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="b9970-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b9970-119">Request headers</span></span>
|<span data-ttu-id="b9970-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="b9970-120">Header</span></span>|<span data-ttu-id="b9970-121">値</span><span class="sxs-lookup"><span data-stu-id="b9970-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b9970-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b9970-122">Authorization</span></span>|<span data-ttu-id="b9970-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="b9970-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b9970-124">承諾</span><span class="sxs-lookup"><span data-stu-id="b9970-124">Accept</span></span>|<span data-ttu-id="b9970-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b9970-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b9970-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="b9970-126">Request body</span></span>
<span data-ttu-id="b9970-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="b9970-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b9970-128">応答</span><span class="sxs-lookup"><span data-stu-id="b9970-128">Response</span></span>
<span data-ttu-id="b9970-129">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="b9970-129">If successful, this method returns a `200 OK` response code and a collection of [deviceCompliancePolicySettingStateSummary](../resources/intune-deviceconfig-devicecompliancepolicysettingstatesummary.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9970-130">例</span><span class="sxs-lookup"><span data-stu-id="b9970-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="b9970-131">要求</span><span class="sxs-lookup"><span data-stu-id="b9970-131">Request</span></span>
<span data-ttu-id="b9970-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="b9970-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicySettingStateSummaries
```

### <a name="response"></a><span data-ttu-id="b9970-133">応答</span><span class="sxs-lookup"><span data-stu-id="b9970-133">Response</span></span>
<span data-ttu-id="b9970-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="b9970-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 532

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceCompliancePolicySettingStateSummary",
      "id": "7474d6d5-d6d5-7474-d5d6-7474d5d67474",
      "setting": "Setting value",
      "settingName": "Setting Name value",
      "platformType": "androidForWork",
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




