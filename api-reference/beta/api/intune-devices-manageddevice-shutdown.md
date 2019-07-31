---
title: shutDown action アクション
description: デバイスをシャットダウンする
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0d5f6285cb1618bd2f119cdaac7897bf002f0aa9
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35987132"
---
# <a name="shutdown-action"></a><span data-ttu-id="1448d-103">shutDown action アクション</span><span class="sxs-lookup"><span data-stu-id="1448d-103">shutDown action</span></span>

> <span data-ttu-id="1448d-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1448d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1448d-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="1448d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1448d-106">デバイスをシャットダウンする</span><span class="sxs-lookup"><span data-stu-id="1448d-106">Shut down device</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1448d-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="1448d-107">Prerequisites</span></span>
<span data-ttu-id="1448d-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1448d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1448d-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1448d-110">Permission type</span></span>|<span data-ttu-id="1448d-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="1448d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1448d-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1448d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1448d-113">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="1448d-113">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="1448d-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1448d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1448d-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1448d-115">Not supported.</span></span>|
|<span data-ttu-id="1448d-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1448d-116">Application</span></span>|<span data-ttu-id="1448d-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1448d-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1448d-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1448d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/shutDown
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/shutDown
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/shutDown
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/shutDown
```

## <a name="request-headers"></a><span data-ttu-id="1448d-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1448d-119">Request headers</span></span>
|<span data-ttu-id="1448d-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1448d-120">Header</span></span>|<span data-ttu-id="1448d-121">値</span><span class="sxs-lookup"><span data-stu-id="1448d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1448d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1448d-122">Authorization</span></span>|<span data-ttu-id="1448d-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="1448d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1448d-124">承諾</span><span class="sxs-lookup"><span data-stu-id="1448d-124">Accept</span></span>|<span data-ttu-id="1448d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1448d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1448d-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="1448d-126">Request body</span></span>
<span data-ttu-id="1448d-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="1448d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1448d-128">応答</span><span class="sxs-lookup"><span data-stu-id="1448d-128">Response</span></span>
<span data-ttu-id="1448d-129">成功した場合、このアクションは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="1448d-129">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="1448d-130">例</span><span class="sxs-lookup"><span data-stu-id="1448d-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="1448d-131">要求</span><span class="sxs-lookup"><span data-stu-id="1448d-131">Request</span></span>
<span data-ttu-id="1448d-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1448d-132">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/shutDown
```

### <a name="response"></a><span data-ttu-id="1448d-133">応答</span><span class="sxs-lookup"><span data-stu-id="1448d-133">Response</span></span>
<span data-ttu-id="1448d-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1448d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





