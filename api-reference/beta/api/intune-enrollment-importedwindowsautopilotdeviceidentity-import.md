---
title: インポートアクション
description: まだ文書化されていません
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4da744d7acd78b31b27238805fb63aa9cb7e3186
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/16/2019
ms.locfileid: "35730000"
---
# <a name="import-action"></a><span data-ttu-id="63836-103">インポートアクション</span><span class="sxs-lookup"><span data-stu-id="63836-103">import action</span></span>

> <span data-ttu-id="63836-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="63836-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="63836-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="63836-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="63836-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="63836-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="63836-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="63836-107">Prerequisites</span></span>
<span data-ttu-id="63836-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="63836-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="63836-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="63836-110">Permission type</span></span>|<span data-ttu-id="63836-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="63836-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="63836-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="63836-112">Delegated (work or school account)</span></span>|<span data-ttu-id="63836-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63836-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="63836-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="63836-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="63836-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="63836-115">Not supported.</span></span>|
|<span data-ttu-id="63836-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="63836-116">Application</span></span>|<span data-ttu-id="63836-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="63836-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="63836-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="63836-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/importedWindowsAutopilotDeviceIdentities/import
```

## <a name="request-headers"></a><span data-ttu-id="63836-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="63836-119">Request headers</span></span>
|<span data-ttu-id="63836-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="63836-120">Header</span></span>|<span data-ttu-id="63836-121">値</span><span class="sxs-lookup"><span data-stu-id="63836-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="63836-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="63836-122">Authorization</span></span>|<span data-ttu-id="63836-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="63836-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="63836-124">承諾</span><span class="sxs-lookup"><span data-stu-id="63836-124">Accept</span></span>|<span data-ttu-id="63836-125">application/json</span><span class="sxs-lookup"><span data-stu-id="63836-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="63836-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="63836-126">Request body</span></span>
<span data-ttu-id="63836-127">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="63836-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="63836-128">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="63836-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="63836-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="63836-129">Property</span></span>|<span data-ttu-id="63836-130">型</span><span class="sxs-lookup"><span data-stu-id="63836-130">Type</span></span>|<span data-ttu-id="63836-131">説明</span><span class="sxs-lookup"><span data-stu-id="63836-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="63836-132">importedWindowsAutopilotDeviceIdentities</span><span class="sxs-lookup"><span data-stu-id="63836-132">importedWindowsAutopilotDeviceIdentities</span></span>|<span data-ttu-id="63836-133">[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="63836-133">[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) collection</span></span>|<span data-ttu-id="63836-134">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="63836-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="63836-135">応答</span><span class="sxs-lookup"><span data-stu-id="63836-135">Response</span></span>
<span data-ttu-id="63836-136">成功した場合、このアクション`200 OK`は応答コードと、応答本文で[importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md)コレクションを返します。</span><span class="sxs-lookup"><span data-stu-id="63836-136">If successful, this action returns a `200 OK` response code and a [importedWindowsAutopilotDeviceIdentity](../resources/intune-enrollment-importedwindowsautopilotdeviceidentity.md) collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="63836-137">例</span><span class="sxs-lookup"><span data-stu-id="63836-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="63836-138">要求</span><span class="sxs-lookup"><span data-stu-id="63836-138">Request</span></span>
<span data-ttu-id="63836-139">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="63836-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/importedWindowsAutopilotDeviceIdentities/import

Content-type: application/json
Content-length: 860

{
  "importedWindowsAutopilotDeviceIdentities": [
    {
      "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentity",
      "id": "985b4f49-4f49-985b-494f-5b98494f5b98",
      "orderIdentifier": "Order Identifier value",
      "groupTag": "Group Tag value",
      "serialNumber": "Serial Number value",
      "productKey": "Product Key value",
      "importId": "Import Id value",
      "hardwareIdentifier": "aGFyZHdhcmVJZGVudGlmaWVy",
      "state": {
        "@odata.type": "microsoft.graph.importedWindowsAutopilotDeviceIdentityState",
        "deviceImportStatus": "pending",
        "deviceRegistrationId": "Device Registration Id value",
        "deviceErrorCode": 15,
        "deviceErrorName": "Device Error Name value"
      },
      "assignedUserPrincipalName": "Assigned User Principal Name value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="63836-140">応答</span><span class="sxs-lookup"><span data-stu-id="63836-140">Response</span></span>
<span data-ttu-id="63836-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="63836-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 825

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.importedWindowsAutopilotDeviceIdentity",
      "id": "985b4f49-4f49-985b-494f-5b98494f5b98",
      "orderIdentifier": "Order Identifier value",
      "groupTag": "Group Tag value",
      "serialNumber": "Serial Number value",
      "productKey": "Product Key value",
      "importId": "Import Id value",
      "hardwareIdentifier": "aGFyZHdhcmVJZGVudGlmaWVy",
      "state": {
        "@odata.type": "microsoft.graph.importedWindowsAutopilotDeviceIdentityState",
        "deviceImportStatus": "pending",
        "deviceRegistrationId": "Device Registration Id value",
        "deviceErrorCode": 15,
        "deviceErrorName": "Device Error Name value"
      },
      "assignedUserPrincipalName": "Assigned User Principal Name value"
    }
  ]
}
```





