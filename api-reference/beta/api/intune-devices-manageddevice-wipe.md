---
title: wipe action
description: デバイスをワイプする
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: c0d3ce629d27efe481f87a4c88a7c1518889d58c
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27924966"
---
# <a name="wipe-action"></a><span data-ttu-id="05515-103">wipe action</span><span class="sxs-lookup"><span data-stu-id="05515-103">wipe action</span></span>

> <span data-ttu-id="05515-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="05515-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="05515-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="05515-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="05515-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="05515-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="05515-107">デバイスをワイプする</span><span class="sxs-lookup"><span data-stu-id="05515-107">Wipe a device</span></span>
## <a name="prerequisites"></a><span data-ttu-id="05515-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="05515-108">Prerequisites</span></span>
<span data-ttu-id="05515-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="05515-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="05515-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="05515-111">Permission type</span></span>|<span data-ttu-id="05515-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="05515-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="05515-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="05515-113">Delegated (work or school account)</span></span>|<span data-ttu-id="05515-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="05515-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="05515-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="05515-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="05515-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="05515-116">Not supported.</span></span>|
|<span data-ttu-id="05515-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="05515-117">Application</span></span>|<span data-ttu-id="05515-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="05515-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="05515-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="05515-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/wipe
POST /deviceManagement/managedDevices/{managedDeviceId}/wipe
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/wipe
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/wipe
```

## <a name="request-headers"></a><span data-ttu-id="05515-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="05515-120">Request headers</span></span>
|<span data-ttu-id="05515-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="05515-121">Header</span></span>|<span data-ttu-id="05515-122">値</span><span class="sxs-lookup"><span data-stu-id="05515-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="05515-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="05515-123">Authorization</span></span>|<span data-ttu-id="05515-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="05515-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="05515-125">Accept</span><span class="sxs-lookup"><span data-stu-id="05515-125">Accept</span></span>|<span data-ttu-id="05515-126">application/json</span><span class="sxs-lookup"><span data-stu-id="05515-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="05515-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="05515-127">Request body</span></span>
<span data-ttu-id="05515-128">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="05515-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="05515-129">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="05515-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="05515-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="05515-130">Property</span></span>|<span data-ttu-id="05515-131">種類</span><span class="sxs-lookup"><span data-stu-id="05515-131">Type</span></span>|<span data-ttu-id="05515-132">説明</span><span class="sxs-lookup"><span data-stu-id="05515-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="05515-133">keepEnrollmentData</span><span class="sxs-lookup"><span data-stu-id="05515-133">keepEnrollmentData</span></span>|<span data-ttu-id="05515-134">ブール値</span><span class="sxs-lookup"><span data-stu-id="05515-134">Boolean</span></span>|<span data-ttu-id="05515-135">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="05515-135">Not yet documented</span></span>|
|<span data-ttu-id="05515-136">keepUserData</span><span class="sxs-lookup"><span data-stu-id="05515-136">keepUserData</span></span>|<span data-ttu-id="05515-137">ブール値</span><span class="sxs-lookup"><span data-stu-id="05515-137">Boolean</span></span>|<span data-ttu-id="05515-138">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="05515-138">Not yet documented</span></span>|
|<span data-ttu-id="05515-139">macOsUnlockCode</span><span class="sxs-lookup"><span data-stu-id="05515-139">macOsUnlockCode</span></span>|<span data-ttu-id="05515-140">文字列</span><span class="sxs-lookup"><span data-stu-id="05515-140">String</span></span>|<span data-ttu-id="05515-141">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="05515-141">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="05515-142">応答</span><span class="sxs-lookup"><span data-stu-id="05515-142">Response</span></span>
<span data-ttu-id="05515-143">成功した場合、このアクションは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="05515-143">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="05515-144">例</span><span class="sxs-lookup"><span data-stu-id="05515-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="05515-145">要求</span><span class="sxs-lookup"><span data-stu-id="05515-145">Request</span></span>
<span data-ttu-id="05515-146">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="05515-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/managedDevices/{managedDeviceId}/wipe

Content-type: application/json
Content-length: 109

{
  "keepEnrollmentData": true,
  "keepUserData": true,
  "macOsUnlockCode": "Mac Os Unlock Code value"
}
```

### <a name="response"></a><span data-ttu-id="05515-147">応答</span><span class="sxs-lookup"><span data-stu-id="05515-147">Response</span></span>
<span data-ttu-id="05515-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="05515-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





