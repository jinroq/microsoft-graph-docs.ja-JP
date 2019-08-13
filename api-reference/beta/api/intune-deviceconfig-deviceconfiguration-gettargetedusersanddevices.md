---
title: getTargetedUsersAndDevices アクション
description: まだ文書化されていません
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f6fbed2f2dce6da3637b4a4921b84834d04dfb60
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36346038"
---
# <a name="gettargetedusersanddevices-action"></a><span data-ttu-id="6ab5a-103">getTargetedUsersAndDevices アクション</span><span class="sxs-lookup"><span data-stu-id="6ab5a-103">getTargetedUsersAndDevices action</span></span>

> <span data-ttu-id="6ab5a-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6ab5a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6ab5a-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6ab5a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6ab5a-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="6ab5a-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6ab5a-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="6ab5a-107">Prerequisites</span></span>
<span data-ttu-id="6ab5a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6ab5a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6ab5a-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6ab5a-110">Permission type</span></span>|<span data-ttu-id="6ab5a-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="6ab5a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6ab5a-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6ab5a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="6ab5a-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6ab5a-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="6ab5a-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6ab5a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6ab5a-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6ab5a-115">Not supported.</span></span>|
|<span data-ttu-id="6ab5a-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6ab5a-116">Application</span></span>|<span data-ttu-id="6ab5a-117">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6ab5a-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6ab5a-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6ab5a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/getTargetedUsersAndDevices
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/getTargetedUsersAndDevices
```

## <a name="request-headers"></a><span data-ttu-id="6ab5a-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6ab5a-119">Request headers</span></span>
|<span data-ttu-id="6ab5a-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6ab5a-120">Header</span></span>|<span data-ttu-id="6ab5a-121">値</span><span class="sxs-lookup"><span data-stu-id="6ab5a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6ab5a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="6ab5a-122">Authorization</span></span>|<span data-ttu-id="6ab5a-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="6ab5a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6ab5a-124">承諾</span><span class="sxs-lookup"><span data-stu-id="6ab5a-124">Accept</span></span>|<span data-ttu-id="6ab5a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="6ab5a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6ab5a-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="6ab5a-126">Request body</span></span>
<span data-ttu-id="6ab5a-127">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="6ab5a-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="6ab5a-128">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="6ab5a-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="6ab5a-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6ab5a-129">Property</span></span>|<span data-ttu-id="6ab5a-130">型</span><span class="sxs-lookup"><span data-stu-id="6ab5a-130">Type</span></span>|<span data-ttu-id="6ab5a-131">説明</span><span class="sxs-lookup"><span data-stu-id="6ab5a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6ab5a-132">deviceConfigurationIds</span><span class="sxs-lookup"><span data-stu-id="6ab5a-132">deviceConfigurationIds</span></span>|<span data-ttu-id="6ab5a-133">String コレクション</span><span class="sxs-lookup"><span data-stu-id="6ab5a-133">String collection</span></span>|<span data-ttu-id="6ab5a-134">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="6ab5a-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="6ab5a-135">応答</span><span class="sxs-lookup"><span data-stu-id="6ab5a-135">Response</span></span>
<span data-ttu-id="6ab5a-136">成功した場合、このアクション`200 OK`は応答コードと、応答本文で[deviceConfigurationTargetedUserAndDevice](../resources/intune-deviceconfig-deviceconfigurationtargeteduseranddevice.md)コレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="6ab5a-136">If successful, this action returns a `200 OK` response code and a [deviceConfigurationTargetedUserAndDevice](../resources/intune-deviceconfig-deviceconfigurationtargeteduseranddevice.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6ab5a-137">例</span><span class="sxs-lookup"><span data-stu-id="6ab5a-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="6ab5a-138">要求</span><span class="sxs-lookup"><span data-stu-id="6ab5a-138">Request</span></span>
<span data-ttu-id="6ab5a-139">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6ab5a-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/getTargetedUsersAndDevices

Content-type: application/json
Content-length: 78

{
  "deviceConfigurationIds": [
    "Device Configuration Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="6ab5a-140">応答</span><span class="sxs-lookup"><span data-stu-id="6ab5a-140">Response</span></span>
<span data-ttu-id="6ab5a-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="6ab5a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 409

{
  "value": [
    {
      "@odata.type": "microsoft.graph.deviceConfigurationTargetedUserAndDevice",
      "deviceId": "Device Id value",
      "deviceName": "Device Name value",
      "userId": "User Id value",
      "userDisplayName": "User Display Name value",
      "userPrincipalName": "User Principal Name value",
      "lastCheckinDateTime": "2017-01-01T00:02:46.0431416-08:00"
    }
  ]
}
```






