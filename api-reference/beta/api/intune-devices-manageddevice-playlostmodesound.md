---
title: playLostModeSound アクション
description: リモート ロック
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5d68be90221644defb4761ca41dfa00d4bfede02
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34958383"
---
# <a name="playlostmodesound-action"></a><span data-ttu-id="02f56-103">playLostModeSound アクション</span><span class="sxs-lookup"><span data-stu-id="02f56-103">playLostModeSound action</span></span>

> <span data-ttu-id="02f56-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="02f56-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="02f56-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="02f56-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="02f56-106">リモート ロック</span><span class="sxs-lookup"><span data-stu-id="02f56-106">Remote lock</span></span>

## <a name="prerequisites"></a><span data-ttu-id="02f56-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="02f56-107">Prerequisites</span></span>
<span data-ttu-id="02f56-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="02f56-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02f56-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="02f56-110">Permission type</span></span>|<span data-ttu-id="02f56-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="02f56-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="02f56-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="02f56-112">Delegated (work or school account)</span></span>|<span data-ttu-id="02f56-113">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="02f56-113">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="02f56-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="02f56-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="02f56-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="02f56-115">Not supported.</span></span>|
|<span data-ttu-id="02f56-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="02f56-116">Application</span></span>|<span data-ttu-id="02f56-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="02f56-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="02f56-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="02f56-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/playLostModeSound
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/playLostModeSound
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/playLostModeSound
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/playLostModeSound
```

## <a name="request-headers"></a><span data-ttu-id="02f56-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="02f56-119">Request headers</span></span>
|<span data-ttu-id="02f56-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="02f56-120">Header</span></span>|<span data-ttu-id="02f56-121">値</span><span class="sxs-lookup"><span data-stu-id="02f56-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="02f56-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="02f56-122">Authorization</span></span>|<span data-ttu-id="02f56-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="02f56-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="02f56-124">承諾</span><span class="sxs-lookup"><span data-stu-id="02f56-124">Accept</span></span>|<span data-ttu-id="02f56-125">application/json</span><span class="sxs-lookup"><span data-stu-id="02f56-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="02f56-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="02f56-126">Request body</span></span>
<span data-ttu-id="02f56-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="02f56-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="02f56-128">応答</span><span class="sxs-lookup"><span data-stu-id="02f56-128">Response</span></span>
<span data-ttu-id="02f56-129">成功した場合、このアクションは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="02f56-129">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="02f56-130">例</span><span class="sxs-lookup"><span data-stu-id="02f56-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="02f56-131">要求</span><span class="sxs-lookup"><span data-stu-id="02f56-131">Request</span></span>
<span data-ttu-id="02f56-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="02f56-132">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/playLostModeSound
```

### <a name="response"></a><span data-ttu-id="02f56-133">応答</span><span class="sxs-lookup"><span data-stu-id="02f56-133">Response</span></span>
<span data-ttu-id="02f56-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="02f56-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





