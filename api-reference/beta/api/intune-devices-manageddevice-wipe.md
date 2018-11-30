---
title: wipe action
description: デバイスをワイプする
ms.openlocfilehash: 841a0c5e968cb3fa9816b604cc3d2e335ca75a4c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070049"
---
# <a name="wipe-action"></a><span data-ttu-id="56aa9-103">wipe action</span><span class="sxs-lookup"><span data-stu-id="56aa9-103">wipe action</span></span>

> <span data-ttu-id="56aa9-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="56aa9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="56aa9-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="56aa9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="56aa9-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="56aa9-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="56aa9-107">デバイスをワイプする</span><span class="sxs-lookup"><span data-stu-id="56aa9-107">Wipe a device</span></span>
## <a name="prerequisites"></a><span data-ttu-id="56aa9-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="56aa9-108">Prerequisites</span></span>
<span data-ttu-id="56aa9-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="56aa9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="56aa9-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="56aa9-111">Permission type</span></span>|<span data-ttu-id="56aa9-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="56aa9-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="56aa9-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="56aa9-113">Delegated (work or school account)</span></span>|<span data-ttu-id="56aa9-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="56aa9-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="56aa9-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="56aa9-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="56aa9-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="56aa9-116">Not supported.</span></span>|
|<span data-ttu-id="56aa9-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="56aa9-117">Application</span></span>|<span data-ttu-id="56aa9-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="56aa9-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="56aa9-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="56aa9-119">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="56aa9-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="56aa9-120">Request headers</span></span>
|<span data-ttu-id="56aa9-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="56aa9-121">Header</span></span>|<span data-ttu-id="56aa9-122">値</span><span class="sxs-lookup"><span data-stu-id="56aa9-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="56aa9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="56aa9-123">Authorization</span></span>|<span data-ttu-id="56aa9-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="56aa9-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="56aa9-125">Accept</span><span class="sxs-lookup"><span data-stu-id="56aa9-125">Accept</span></span>|<span data-ttu-id="56aa9-126">application/json</span><span class="sxs-lookup"><span data-stu-id="56aa9-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="56aa9-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="56aa9-127">Request body</span></span>
<span data-ttu-id="56aa9-128">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="56aa9-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="56aa9-129">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="56aa9-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="56aa9-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="56aa9-130">Property</span></span>|<span data-ttu-id="56aa9-131">型</span><span class="sxs-lookup"><span data-stu-id="56aa9-131">Type</span></span>|<span data-ttu-id="56aa9-132">説明</span><span class="sxs-lookup"><span data-stu-id="56aa9-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="56aa9-133">keepEnrollmentData</span><span class="sxs-lookup"><span data-stu-id="56aa9-133">keepEnrollmentData</span></span>|<span data-ttu-id="56aa9-134">ブール値</span><span class="sxs-lookup"><span data-stu-id="56aa9-134">Boolean</span></span>|<span data-ttu-id="56aa9-135">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="56aa9-135">Not yet documented</span></span>|
|<span data-ttu-id="56aa9-136">keepUserData</span><span class="sxs-lookup"><span data-stu-id="56aa9-136">keepUserData</span></span>|<span data-ttu-id="56aa9-137">ブール値</span><span class="sxs-lookup"><span data-stu-id="56aa9-137">Boolean</span></span>|<span data-ttu-id="56aa9-138">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="56aa9-138">Not yet documented</span></span>|
|<span data-ttu-id="56aa9-139">macOsUnlockCode</span><span class="sxs-lookup"><span data-stu-id="56aa9-139">macOsUnlockCode</span></span>|<span data-ttu-id="56aa9-140">文字列</span><span class="sxs-lookup"><span data-stu-id="56aa9-140">String</span></span>|<span data-ttu-id="56aa9-141">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="56aa9-141">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="56aa9-142">応答</span><span class="sxs-lookup"><span data-stu-id="56aa9-142">Response</span></span>
<span data-ttu-id="56aa9-143">成功した場合、このアクションは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="56aa9-143">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="56aa9-144">例</span><span class="sxs-lookup"><span data-stu-id="56aa9-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="56aa9-145">要求</span><span class="sxs-lookup"><span data-stu-id="56aa9-145">Request</span></span>
<span data-ttu-id="56aa9-146">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="56aa9-146">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="56aa9-147">応答</span><span class="sxs-lookup"><span data-stu-id="56aa9-147">Response</span></span>
<span data-ttu-id="56aa9-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="56aa9-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





