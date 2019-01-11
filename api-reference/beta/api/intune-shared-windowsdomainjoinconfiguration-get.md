---
title: WindowsDomainJoinConfiguration を取得します。
description: WindowsDomainJoinConfiguration オブジェクトのプロパティと関係を参照してください。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d0c4aedf07e8a6e95dc81f440975809e75b85160
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27831333"
---
# <a name="get-windowsdomainjoinconfiguration"></a><span data-ttu-id="6c53c-103">WindowsDomainJoinConfiguration を取得します。</span><span class="sxs-lookup"><span data-stu-id="6c53c-103">Get windowsDomainJoinConfiguration</span></span>

> <span data-ttu-id="6c53c-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6c53c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6c53c-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6c53c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6c53c-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="6c53c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6c53c-107">[WindowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6c53c-107">Read properties and relationships of the [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6c53c-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="6c53c-108">Prerequisites</span></span>

<span data-ttu-id="6c53c-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6c53c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6c53c-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6c53c-111">Permission type</span></span>|<span data-ttu-id="6c53c-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="6c53c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6c53c-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6c53c-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="6c53c-114">&nbsp; &nbsp; **デバイス構成**</span><span class="sxs-lookup"><span data-stu-id="6c53c-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="6c53c-115">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6c53c-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="6c53c-116">&nbsp; &nbsp; **登録**</span><span class="sxs-lookup"><span data-stu-id="6c53c-116">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="6c53c-117">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="6c53c-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
|<span data-ttu-id="6c53c-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6c53c-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6c53c-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6c53c-119">Not supported.</span></span>|
|<span data-ttu-id="6c53c-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6c53c-120">Application</span></span>|<span data-ttu-id="6c53c-121">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6c53c-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6c53c-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6c53c-122">HTTP Request</span></span>
<span data-ttu-id="6c53c-123">**デバイス構成**</span><span class="sxs-lookup"><span data-stu-id="6c53c-123">**Device configuration**</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

<span data-ttu-id="6c53c-124">**登録**</span><span class="sxs-lookup"><span data-stu-id="6c53c-124">**Enrollment**</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/microsoft.graph.activeDirectoryWindowsAutopilotDeploymentProfile/domainJoinConfiguration
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6c53c-125">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="6c53c-125">Optional query parameters</span></span>

<span data-ttu-id="6c53c-126">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="6c53c-126">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6c53c-127">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6c53c-127">Request headers</span></span>

|<span data-ttu-id="6c53c-128">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6c53c-128">Header</span></span>|<span data-ttu-id="6c53c-129">値</span><span class="sxs-lookup"><span data-stu-id="6c53c-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6c53c-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="6c53c-130">Authorization</span></span>|<span data-ttu-id="6c53c-131">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="6c53c-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6c53c-132">Accept</span><span class="sxs-lookup"><span data-stu-id="6c53c-132">Accept</span></span>|<span data-ttu-id="6c53c-133">application/json</span><span class="sxs-lookup"><span data-stu-id="6c53c-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6c53c-134">要求本文</span><span class="sxs-lookup"><span data-stu-id="6c53c-134">Request body</span></span>

<span data-ttu-id="6c53c-135">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="6c53c-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6c53c-136">応答</span><span class="sxs-lookup"><span data-stu-id="6c53c-136">Response</span></span>

<span data-ttu-id="6c53c-137">かどうかは成功すると、このメソッドが返されます、 `200 OK` 、応答の本体で応答コードと[windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md)のオブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="6c53c-137">If successful, this method returns a `200 OK` response code and [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6c53c-138">例</span><span class="sxs-lookup"><span data-stu-id="6c53c-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="6c53c-139">要求</span><span class="sxs-lookup"><span data-stu-id="6c53c-139">Request</span></span>

<span data-ttu-id="6c53c-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6c53c-140">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="6c53c-141">応答</span><span class="sxs-lookup"><span data-stu-id="6c53c-141">Response</span></span>

<span data-ttu-id="6c53c-142">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="6c53c-142">Here is an example of the response.</span></span> <span data-ttu-id="6c53c-143">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="6c53c-143">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="6c53c-144">実際の呼び出しから返されるプロパティは、コンテキストに依存します。</span><span class="sxs-lookup"><span data-stu-id="6c53c-144">Properties returned from an actual call depend on the context.</span></span>

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 560

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsDomainJoinConfiguration",
    "id": "40118d08-8d08-4011-088d-1140088d1140",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "computerNameStaticPrefix": "Computer Name Static Prefix value",
    "computerNameSuffixRandomCharCount": 1,
    "activeDirectoryDomainName": "Active Directory Domain Name value"
  }
}
```



