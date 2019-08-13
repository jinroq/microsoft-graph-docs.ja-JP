---
title: windowsDefenderScan アクション
description: まだ文書化されていません
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 40397c680f33464c050c67803e834416531bc349
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36348656"
---
# <a name="windowsdefenderscan-action"></a><span data-ttu-id="fde3b-103">windowsDefenderScan アクション</span><span class="sxs-lookup"><span data-stu-id="fde3b-103">windowsDefenderScan action</span></span>

> <span data-ttu-id="fde3b-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fde3b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fde3b-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="fde3b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fde3b-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="fde3b-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fde3b-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="fde3b-107">Prerequisites</span></span>
<span data-ttu-id="fde3b-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fde3b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fde3b-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fde3b-110">Permission type</span></span>|<span data-ttu-id="fde3b-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="fde3b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fde3b-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fde3b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fde3b-113">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="fde3b-113">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="fde3b-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fde3b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fde3b-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fde3b-115">Not supported.</span></span>|
|<span data-ttu-id="fde3b-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fde3b-116">Application</span></span>|<span data-ttu-id="fde3b-117">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="fde3b-117">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fde3b-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fde3b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/windowsDefenderScan
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/windowsDefenderScan
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/windowsDefenderScan
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/windowsDefenderScan
```

## <a name="request-headers"></a><span data-ttu-id="fde3b-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fde3b-119">Request headers</span></span>
|<span data-ttu-id="fde3b-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fde3b-120">Header</span></span>|<span data-ttu-id="fde3b-121">値</span><span class="sxs-lookup"><span data-stu-id="fde3b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fde3b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="fde3b-122">Authorization</span></span>|<span data-ttu-id="fde3b-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="fde3b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fde3b-124">承諾</span><span class="sxs-lookup"><span data-stu-id="fde3b-124">Accept</span></span>|<span data-ttu-id="fde3b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fde3b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fde3b-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="fde3b-126">Request body</span></span>
<span data-ttu-id="fde3b-127">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="fde3b-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="fde3b-128">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="fde3b-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="fde3b-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fde3b-129">Property</span></span>|<span data-ttu-id="fde3b-130">型</span><span class="sxs-lookup"><span data-stu-id="fde3b-130">Type</span></span>|<span data-ttu-id="fde3b-131">説明</span><span class="sxs-lookup"><span data-stu-id="fde3b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fde3b-132">quickScan</span><span class="sxs-lookup"><span data-stu-id="fde3b-132">quickScan</span></span>|<span data-ttu-id="fde3b-133">Boolean</span><span class="sxs-lookup"><span data-stu-id="fde3b-133">Boolean</span></span>|<span data-ttu-id="fde3b-134">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="fde3b-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="fde3b-135">応答</span><span class="sxs-lookup"><span data-stu-id="fde3b-135">Response</span></span>
<span data-ttu-id="fde3b-136">成功した場合、このアクションは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="fde3b-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="fde3b-137">例</span><span class="sxs-lookup"><span data-stu-id="fde3b-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="fde3b-138">要求</span><span class="sxs-lookup"><span data-stu-id="fde3b-138">Request</span></span>
<span data-ttu-id="fde3b-139">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="fde3b-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/windowsDefenderScan

Content-type: application/json
Content-length: 25

{
  "quickScan": true
}
```

### <a name="response"></a><span data-ttu-id="fde3b-140">応答</span><span class="sxs-lookup"><span data-stu-id="fde3b-140">Response</span></span>
<span data-ttu-id="fde3b-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="fde3b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






