---
title: enableLostMode アクション
description: 失われるモードを有効にします。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 0bd7d58a70d60b040b25dcb38574e16edb309599
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27934325"
---
# <a name="enablelostmode-action"></a><span data-ttu-id="56dac-103">enableLostMode アクション</span><span class="sxs-lookup"><span data-stu-id="56dac-103">enableLostMode action</span></span>

> <span data-ttu-id="56dac-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="56dac-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="56dac-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="56dac-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="56dac-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="56dac-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="56dac-107">失われるモードを有効にします。</span><span class="sxs-lookup"><span data-stu-id="56dac-107">Enable lost mode</span></span>
## <a name="prerequisites"></a><span data-ttu-id="56dac-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="56dac-108">Prerequisites</span></span>
<span data-ttu-id="56dac-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="56dac-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="56dac-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="56dac-111">Permission type</span></span>|<span data-ttu-id="56dac-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="56dac-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="56dac-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="56dac-113">Delegated (work or school account)</span></span>|<span data-ttu-id="56dac-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="56dac-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="56dac-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="56dac-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="56dac-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="56dac-116">Not supported.</span></span>|
|<span data-ttu-id="56dac-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="56dac-117">Application</span></span>|<span data-ttu-id="56dac-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="56dac-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="56dac-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="56dac-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/enableLostMode
POST /deviceManagement/managedDevices/{managedDeviceId}/enableLostMode
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/enableLostMode
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/enableLostMode
```

## <a name="request-headers"></a><span data-ttu-id="56dac-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="56dac-120">Request headers</span></span>
|<span data-ttu-id="56dac-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="56dac-121">Header</span></span>|<span data-ttu-id="56dac-122">値</span><span class="sxs-lookup"><span data-stu-id="56dac-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="56dac-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="56dac-123">Authorization</span></span>|<span data-ttu-id="56dac-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="56dac-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="56dac-125">Accept</span><span class="sxs-lookup"><span data-stu-id="56dac-125">Accept</span></span>|<span data-ttu-id="56dac-126">application/json</span><span class="sxs-lookup"><span data-stu-id="56dac-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="56dac-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="56dac-127">Request body</span></span>
<span data-ttu-id="56dac-128">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="56dac-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="56dac-129">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="56dac-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="56dac-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="56dac-130">Property</span></span>|<span data-ttu-id="56dac-131">型</span><span class="sxs-lookup"><span data-stu-id="56dac-131">Type</span></span>|<span data-ttu-id="56dac-132">説明</span><span class="sxs-lookup"><span data-stu-id="56dac-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="56dac-133">message</span><span class="sxs-lookup"><span data-stu-id="56dac-133">message</span></span>|<span data-ttu-id="56dac-134">String</span><span class="sxs-lookup"><span data-stu-id="56dac-134">String</span></span>|<span data-ttu-id="56dac-135">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="56dac-135">Not yet documented</span></span>|
|<span data-ttu-id="56dac-136">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="56dac-136">phoneNumber</span></span>|<span data-ttu-id="56dac-137">String</span><span class="sxs-lookup"><span data-stu-id="56dac-137">String</span></span>|<span data-ttu-id="56dac-138">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="56dac-138">Not yet documented</span></span>|
|<span data-ttu-id="56dac-139">フッター</span><span class="sxs-lookup"><span data-stu-id="56dac-139">footer</span></span>|<span data-ttu-id="56dac-140">String</span><span class="sxs-lookup"><span data-stu-id="56dac-140">String</span></span>|<span data-ttu-id="56dac-141">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="56dac-141">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="56dac-142">応答</span><span class="sxs-lookup"><span data-stu-id="56dac-142">Response</span></span>
<span data-ttu-id="56dac-143">成功した場合、このアクションは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="56dac-143">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="56dac-144">例</span><span class="sxs-lookup"><span data-stu-id="56dac-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="56dac-145">要求</span><span class="sxs-lookup"><span data-stu-id="56dac-145">Request</span></span>
<span data-ttu-id="56dac-146">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="56dac-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/managedDevices/{managedDeviceId}/enableLostMode

Content-type: application/json
Content-length: 103

{
  "message": "Message value",
  "phoneNumber": "Phone Number value",
  "footer": "Footer value"
}
```

### <a name="response"></a><span data-ttu-id="56dac-147">応答</span><span class="sxs-lookup"><span data-stu-id="56dac-147">Response</span></span>
<span data-ttu-id="56dac-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="56dac-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





