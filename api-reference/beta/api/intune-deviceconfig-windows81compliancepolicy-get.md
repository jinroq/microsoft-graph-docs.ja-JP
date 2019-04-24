---
title: Get windows81CompliancePolicy
description: windows81CompliancePolicy オブジェクトのプロパティとリレーションシップを読み取ります。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2e97162681df00d5728006d363ed3c242be244ff
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32515408"
---
# <a name="get-windows81compliancepolicy"></a><span data-ttu-id="68486-103">Get windows81CompliancePolicy</span><span class="sxs-lookup"><span data-stu-id="68486-103">Get windows81CompliancePolicy</span></span>

> <span data-ttu-id="68486-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="68486-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="68486-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="68486-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="68486-106">[windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="68486-106">Read properties and relationships of the [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="68486-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="68486-107">Prerequisites</span></span>
<span data-ttu-id="68486-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="68486-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="68486-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="68486-110">Permission type</span></span>|<span data-ttu-id="68486-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="68486-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="68486-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="68486-112">Delegated (work or school account)</span></span>|<span data-ttu-id="68486-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="68486-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="68486-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="68486-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="68486-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="68486-115">Not supported.</span></span>|
|<span data-ttu-id="68486-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="68486-116">Application</span></span>|<span data-ttu-id="68486-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="68486-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="68486-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="68486-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="68486-119">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="68486-119">Optional query parameters</span></span>
<span data-ttu-id="68486-120">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://docs.microsoft.com/en-us/graph/query-parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="68486-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="68486-121">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="68486-121">Request headers</span></span>
|<span data-ttu-id="68486-122">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="68486-122">Header</span></span>|<span data-ttu-id="68486-123">値</span><span class="sxs-lookup"><span data-stu-id="68486-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="68486-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="68486-124">Authorization</span></span>|<span data-ttu-id="68486-125">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="68486-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="68486-126">承諾</span><span class="sxs-lookup"><span data-stu-id="68486-126">Accept</span></span>|<span data-ttu-id="68486-127">application/json</span><span class="sxs-lookup"><span data-stu-id="68486-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="68486-128">要求本文</span><span class="sxs-lookup"><span data-stu-id="68486-128">Request body</span></span>
<span data-ttu-id="68486-129">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="68486-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="68486-130">応答</span><span class="sxs-lookup"><span data-stu-id="68486-130">Response</span></span>
<span data-ttu-id="68486-131">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="68486-131">If successful, this method returns a `200 OK` response code and [windows81CompliancePolicy](../resources/intune-deviceconfig-windows81compliancepolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="68486-132">例</span><span class="sxs-lookup"><span data-stu-id="68486-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="68486-133">要求</span><span class="sxs-lookup"><span data-stu-id="68486-133">Request</span></span>
<span data-ttu-id="68486-134">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="68486-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}
```

### <a name="response"></a><span data-ttu-id="68486-135">応答</span><span class="sxs-lookup"><span data-stu-id="68486-135">Response</span></span>
<span data-ttu-id="68486-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="68486-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 897

{
  "value": {
    "@odata.type": "#microsoft.graph.windows81CompliancePolicy",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "id": "6bb4b7e0-b7e0-6bb4-e0b7-b46be0b7b46b",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "displayName": "Display Name value",
    "version": 7,
    "passwordRequired": true,
    "passwordBlockSimple": true,
    "passwordExpirationDays": 6,
    "passwordMinimumLength": 5,
    "passwordMinutesOfInactivityBeforeLock": 5,
    "passwordMinimumCharacterSetCount": 0,
    "passwordRequiredType": "alphanumeric",
    "passwordPreviousPasswordBlockCount": 2,
    "osMinimumVersion": "Os Minimum Version value",
    "osMaximumVersion": "Os Maximum Version value",
    "storageRequireEncryption": true
  }
}
```





