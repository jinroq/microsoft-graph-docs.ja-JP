---
title: WindowsDomainJoinConfiguration の取得
description: WindowsDomainJoinConfiguration オブジェクトのプロパティとリレーションシップを読み取ります。
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e4564ad51af079543a192762a781110a91117524
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36350546"
---
# <a name="get-windowsdomainjoinconfiguration"></a><span data-ttu-id="4551b-103">WindowsDomainJoinConfiguration の取得</span><span class="sxs-lookup"><span data-stu-id="4551b-103">Get windowsDomainJoinConfiguration</span></span>

> <span data-ttu-id="4551b-104">**重要:** Microsoft Graph の/ベータ版の Api は変更される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="4551b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="4551b-105">実稼働アプリケーションでは、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4551b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4551b-106">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4551b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4551b-107">[Windowsdomainjoinconfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="4551b-107">Read properties and relationships of the [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4551b-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="4551b-108">Prerequisites</span></span>

<span data-ttu-id="4551b-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4551b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4551b-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4551b-111">Permission type</span></span>|<span data-ttu-id="4551b-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="4551b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4551b-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4551b-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="4551b-114">&nbsp; &nbsp; **デバイス構成**</span><span class="sxs-lookup"><span data-stu-id="4551b-114">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="4551b-115">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="4551b-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="4551b-116">&nbsp;&nbsp; **登録**</span><span class="sxs-lookup"><span data-stu-id="4551b-116">&nbsp; &nbsp; **Enrollment**</span></span> | <span data-ttu-id="4551b-117">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="4551b-117">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span> |
|<span data-ttu-id="4551b-118">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4551b-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4551b-119">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4551b-119">Not supported.</span></span>|
|<span data-ttu-id="4551b-120">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4551b-120">Application</span></span>|<span data-ttu-id="4551b-121">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4551b-121">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4551b-122">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4551b-122">HTTP Request</span></span>
<span data-ttu-id="4551b-123">**デバイス構成**</span><span class="sxs-lookup"><span data-stu-id="4551b-123">**Device configuration**</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

<span data-ttu-id="4551b-124">**登録**</span><span class="sxs-lookup"><span data-stu-id="4551b-124">**Enrollment**</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/microsoft.graph.activeDirectoryWindowsAutopilotDeploymentProfile/domainJoinConfiguration
```

## <a name="optional-query-parameters"></a><span data-ttu-id="4551b-125">オプションのクエリ パラメーター</span><span class="sxs-lookup"><span data-stu-id="4551b-125">Optional query parameters</span></span>

<span data-ttu-id="4551b-126">このメソッドは、応答をカスタマイズするための [OData クエリ パラメーター](https://developer.microsoft.com/graph/docs/concepts/query_parameters)をサポートします。</span><span class="sxs-lookup"><span data-stu-id="4551b-126">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="4551b-127">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4551b-127">Request headers</span></span>

|<span data-ttu-id="4551b-128">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4551b-128">Header</span></span>|<span data-ttu-id="4551b-129">値</span><span class="sxs-lookup"><span data-stu-id="4551b-129">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4551b-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="4551b-130">Authorization</span></span>|<span data-ttu-id="4551b-131">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="4551b-131">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4551b-132">承諾</span><span class="sxs-lookup"><span data-stu-id="4551b-132">Accept</span></span>|<span data-ttu-id="4551b-133">application/json</span><span class="sxs-lookup"><span data-stu-id="4551b-133">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4551b-134">要求本文</span><span class="sxs-lookup"><span data-stu-id="4551b-134">Request body</span></span>

<span data-ttu-id="4551b-135">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="4551b-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4551b-136">応答</span><span class="sxs-lookup"><span data-stu-id="4551b-136">Response</span></span>

<span data-ttu-id="4551b-137">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で[Windowsdomainjoinconfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="4551b-137">If successful, this method returns a `200 OK` response code and [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4551b-138">例</span><span class="sxs-lookup"><span data-stu-id="4551b-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="4551b-139">要求</span><span class="sxs-lookup"><span data-stu-id="4551b-139">Request</span></span>

<span data-ttu-id="4551b-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4551b-140">Here is an example of the request.</span></span>

``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="4551b-141">応答</span><span class="sxs-lookup"><span data-stu-id="4551b-141">Response</span></span>

<span data-ttu-id="4551b-142">以下は、応答の例です。</span><span class="sxs-lookup"><span data-stu-id="4551b-142">Here is an example of the response.</span></span> <span data-ttu-id="4551b-143">注: 簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。</span><span class="sxs-lookup"><span data-stu-id="4551b-143">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="4551b-144">実際の呼び出しから返されるプロパティは、コンテキストによって異なります。</span><span class="sxs-lookup"><span data-stu-id="4551b-144">Properties returned from an actual call depend on the context.</span></span>

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






