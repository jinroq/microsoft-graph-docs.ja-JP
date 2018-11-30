---
title: Get iosUpdateConfiguration
description: iosUpdateConfiguration オブジェクトのプロパティとリレーションシップを読み取ります。
ms.openlocfilehash: 5a3e83db1c402cc0707978b598e0d1a9454713f2
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27069465"
---
# <a name="get-iosupdateconfiguration"></a><span data-ttu-id="84709-103">Get iosUpdateConfiguration</span><span class="sxs-lookup"><span data-stu-id="84709-103">Get iosUpdateConfiguration</span></span>

> <span data-ttu-id="84709-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="84709-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="84709-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="84709-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="84709-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="84709-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="84709-107">[iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="84709-107">Read properties and relationships of the [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="84709-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="84709-108">Prerequisites</span></span>
<span data-ttu-id="84709-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="84709-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="84709-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="84709-111">Permission type</span></span>|<span data-ttu-id="84709-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="84709-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="84709-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="84709-113">Delegated (work or school account)</span></span>|<span data-ttu-id="84709-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="84709-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="84709-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="84709-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="84709-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="84709-116">Not supported.</span></span>|
|<span data-ttu-id="84709-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="84709-117">Application</span></span>|<span data-ttu-id="84709-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="84709-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="84709-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="84709-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="84709-120">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="84709-120">Optional query parameters</span></span>
<span data-ttu-id="84709-121">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="84709-121">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="84709-122">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="84709-122">Request headers</span></span>
|<span data-ttu-id="84709-123">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="84709-123">Header</span></span>|<span data-ttu-id="84709-124">値</span><span class="sxs-lookup"><span data-stu-id="84709-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="84709-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="84709-125">Authorization</span></span>|<span data-ttu-id="84709-126">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="84709-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="84709-127">Accept</span><span class="sxs-lookup"><span data-stu-id="84709-127">Accept</span></span>|<span data-ttu-id="84709-128">application/json</span><span class="sxs-lookup"><span data-stu-id="84709-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="84709-129">要求本文</span><span class="sxs-lookup"><span data-stu-id="84709-129">Request body</span></span>
<span data-ttu-id="84709-130">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="84709-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="84709-131">応答</span><span class="sxs-lookup"><span data-stu-id="84709-131">Response</span></span>
<span data-ttu-id="84709-132">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="84709-132">If successful, this method returns a `200 OK` response code and [iosUpdateConfiguration](../resources/intune-deviceconfig-iosupdateconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="84709-133">例</span><span class="sxs-lookup"><span data-stu-id="84709-133">Example</span></span>
### <a name="request"></a><span data-ttu-id="84709-134">要求</span><span class="sxs-lookup"><span data-stu-id="84709-134">Request</span></span>
<span data-ttu-id="84709-135">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="84709-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="84709-136">応答</span><span class="sxs-lookup"><span data-stu-id="84709-136">Response</span></span>
<span data-ttu-id="84709-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="84709-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 711

{
  "value": {
    "@odata.type": "#microsoft.graph.iosUpdateConfiguration",
    "id": "321aef09-ef09-321a-09ef-1a3209ef1a32",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "supportsScopeTags": true,
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "isEnabled": true,
    "activeHoursStart": "12:00:05.5020000",
    "activeHoursEnd": "11:59:00.8990000",
    "scheduledInstallDays": [
      "monday"
    ],
    "utcTimeOffsetInMinutes": 6,
    "enforcedSoftwareUpdateDelayInDays": 1
  }
}
```





