---
title: リスト securityBaselineDeviceStates
description: SecurityBaselineDeviceState オブジェクトのプロパティとリレーションシップをリストします。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 72436d2fed2c8069bfa7d41a111561f7a508ecd5
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34959524"
---
# <a name="list-securitybaselinedevicestates"></a><span data-ttu-id="02d86-103">リスト securityBaselineDeviceStates</span><span class="sxs-lookup"><span data-stu-id="02d86-103">List securityBaselineDeviceStates</span></span>

> <span data-ttu-id="02d86-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="02d86-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="02d86-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="02d86-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="02d86-106">[SecurityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="02d86-106">List properties and relationships of the [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="02d86-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="02d86-107">Prerequisites</span></span>
<span data-ttu-id="02d86-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="02d86-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02d86-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="02d86-110">Permission type</span></span>|<span data-ttu-id="02d86-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="02d86-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="02d86-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="02d86-112">Delegated (work or school account)</span></span>|<span data-ttu-id="02d86-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="02d86-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="02d86-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="02d86-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="02d86-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="02d86-115">Not supported.</span></span>|
|<span data-ttu-id="02d86-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="02d86-116">Application</span></span>|<span data-ttu-id="02d86-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="02d86-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="02d86-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="02d86-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/deviceStates
```

## <a name="request-headers"></a><span data-ttu-id="02d86-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="02d86-119">Request headers</span></span>
|<span data-ttu-id="02d86-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="02d86-120">Header</span></span>|<span data-ttu-id="02d86-121">値</span><span class="sxs-lookup"><span data-stu-id="02d86-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="02d86-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="02d86-122">Authorization</span></span>|<span data-ttu-id="02d86-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="02d86-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="02d86-124">承諾</span><span class="sxs-lookup"><span data-stu-id="02d86-124">Accept</span></span>|<span data-ttu-id="02d86-125">application/json</span><span class="sxs-lookup"><span data-stu-id="02d86-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="02d86-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="02d86-126">Request body</span></span>
<span data-ttu-id="02d86-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="02d86-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="02d86-128">応答</span><span class="sxs-lookup"><span data-stu-id="02d86-128">Response</span></span>
<span data-ttu-id="02d86-129">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md)オブジェクトのコレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="02d86-129">If successful, this method returns a `200 OK` response code and a collection of [securityBaselineDeviceState](../resources/intune-deviceintent-securitybaselinedevicestate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="02d86-130">例</span><span class="sxs-lookup"><span data-stu-id="02d86-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="02d86-131">要求</span><span class="sxs-lookup"><span data-stu-id="02d86-131">Request</span></span>
<span data-ttu-id="02d86-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="02d86-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/templates/{deviceManagementTemplateId}/microsoft.graph.securityBaselineTemplate/deviceStates
```

### <a name="response"></a><span data-ttu-id="02d86-133">応答</span><span class="sxs-lookup"><span data-stu-id="02d86-133">Response</span></span>
<span data-ttu-id="02d86-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="02d86-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 420

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.securityBaselineDeviceState",
      "id": "182749bf-49bf-1827-bf49-2718bf492718",
      "managedDeviceId": "Managed Device Id value",
      "deviceDisplayName": "Device Display Name value",
      "userPrincipalName": "User Principal Name value",
      "state": "secure",
      "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00"
    }
  ]
}
```





