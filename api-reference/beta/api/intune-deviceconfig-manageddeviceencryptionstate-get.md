---
title: ManagedDeviceEncryptionState の取得
description: ManagedDeviceEncryptionState オブジェクトのプロパティとリレーションシップを読み取ります。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: fb36d0e3b3132cde541604b8256c54576e4d1d63
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35715341"
---
# <a name="get-manageddeviceencryptionstate"></a><span data-ttu-id="ff2e4-103">ManagedDeviceEncryptionState の取得</span><span class="sxs-lookup"><span data-stu-id="ff2e4-103">Get managedDeviceEncryptionState</span></span>

> <span data-ttu-id="ff2e4-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ff2e4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ff2e4-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ff2e4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff2e4-106">[Manageddeviceencryptionstate](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="ff2e4-106">Read properties and relationships of the [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ff2e4-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="ff2e4-107">Prerequisites</span></span>
<span data-ttu-id="ff2e4-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ff2e4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff2e4-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ff2e4-110">Permission type</span></span>|<span data-ttu-id="ff2e4-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ff2e4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ff2e4-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ff2e4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ff2e4-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="ff2e4-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="ff2e4-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ff2e4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ff2e4-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ff2e4-115">Not supported.</span></span>|
|<span data-ttu-id="ff2e4-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ff2e4-116">Application</span></span>|<span data-ttu-id="ff2e4-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ff2e4-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ff2e4-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ff2e4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managedDeviceEncryptionStates/{managedDeviceEncryptionStateId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ff2e4-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="ff2e4-119">Optional query parameters</span></span>
<span data-ttu-id="ff2e4-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="ff2e4-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ff2e4-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ff2e4-121">Request headers</span></span>
|<span data-ttu-id="ff2e4-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ff2e4-122">Header</span></span>|<span data-ttu-id="ff2e4-123">値</span><span class="sxs-lookup"><span data-stu-id="ff2e4-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ff2e4-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="ff2e4-124">Authorization</span></span>|<span data-ttu-id="ff2e4-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="ff2e4-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ff2e4-126">承諾</span><span class="sxs-lookup"><span data-stu-id="ff2e4-126">Accept</span></span>|<span data-ttu-id="ff2e4-127">application/json</span><span class="sxs-lookup"><span data-stu-id="ff2e4-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ff2e4-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="ff2e4-128">Request body</span></span>
<span data-ttu-id="ff2e4-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="ff2e4-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ff2e4-130">応答</span><span class="sxs-lookup"><span data-stu-id="ff2e4-130">Response</span></span>
<span data-ttu-id="ff2e4-131">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[Manageddeviceencryptionstate](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ff2e4-131">If successful, this method returns a `200 OK` response code and [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ff2e4-132">例</span><span class="sxs-lookup"><span data-stu-id="ff2e4-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="ff2e4-133">要求</span><span class="sxs-lookup"><span data-stu-id="ff2e4-133">Request</span></span>
<span data-ttu-id="ff2e4-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ff2e4-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managedDeviceEncryptionStates/{managedDeviceEncryptionStateId}
```

### <a name="response"></a><span data-ttu-id="ff2e4-135">応答</span><span class="sxs-lookup"><span data-stu-id="ff2e4-135">Response</span></span>
<span data-ttu-id="ff2e4-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ff2e4-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 810

{
  "value": {
    "@odata.type": "#microsoft.graph.managedDeviceEncryptionState",
    "id": "f09b4ab6-4ab6-f09b-b64a-9bf0b64a9bf0",
    "userPrincipalName": "User Principal Name value",
    "deviceType": "windowsRT",
    "osVersion": "Os Version value",
    "tpmSpecificationVersion": "Tpm Specification Version value",
    "deviceName": "Device Name value",
    "encryptionReadinessState": "ready",
    "encryptionState": "encrypted",
    "encryptionPolicySettingState": "notApplicable",
    "advancedBitLockerStates": "noUserConsent",
    "fileVaultStates": "driveEncryptedByUser",
    "policyDetails": [
      {
        "@odata.type": "microsoft.graph.encryptionReportPolicyDetails",
        "policyId": "Policy Id value",
        "policyName": "Policy Name value"
      }
    ]
  }
}
```





