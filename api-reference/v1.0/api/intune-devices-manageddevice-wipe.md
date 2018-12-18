---
title: wipe action
description: デバイスをワイプする
author: tfitzmac
ms.openlocfilehash: 6ac3c21b517523d46cfc2958a661d058a86d708e
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27311418"
---
# <a name="wipe-action"></a><span data-ttu-id="fc763-103">wipe action</span><span class="sxs-lookup"><span data-stu-id="fc763-103">wipe action</span></span>

> <span data-ttu-id="fc763-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="fc763-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fc763-105">デバイスをワイプする</span><span class="sxs-lookup"><span data-stu-id="fc763-105">Wipe a device</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fc763-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="fc763-106">Prerequisites</span></span>
<span data-ttu-id="fc763-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fc763-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fc763-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fc763-109">Permission type</span></span>|<span data-ttu-id="fc763-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="fc763-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fc763-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fc763-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fc763-112">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="fc763-112">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="fc763-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fc763-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fc763-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fc763-114">Not supported.</span></span>|
|<span data-ttu-id="fc763-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fc763-115">Application</span></span>|<span data-ttu-id="fc763-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fc763-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fc763-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fc763-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/wipe
POST /deviceManagement/managedDevices/{managedDeviceId}/wipe
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/wipe
```

## <a name="request-headers"></a><span data-ttu-id="fc763-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fc763-118">Request headers</span></span>
|<span data-ttu-id="fc763-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fc763-119">Header</span></span>|<span data-ttu-id="fc763-120">値</span><span class="sxs-lookup"><span data-stu-id="fc763-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fc763-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="fc763-121">Authorization</span></span>|<span data-ttu-id="fc763-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="fc763-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fc763-123">Accept</span><span class="sxs-lookup"><span data-stu-id="fc763-123">Accept</span></span>|<span data-ttu-id="fc763-124">application/json</span><span class="sxs-lookup"><span data-stu-id="fc763-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fc763-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="fc763-125">Request body</span></span>
<span data-ttu-id="fc763-126">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="fc763-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="fc763-127">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="fc763-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="fc763-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fc763-128">Property</span></span>|<span data-ttu-id="fc763-129">種類</span><span class="sxs-lookup"><span data-stu-id="fc763-129">Type</span></span>|<span data-ttu-id="fc763-130">説明</span><span class="sxs-lookup"><span data-stu-id="fc763-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc763-131">keepEnrollmentData</span><span class="sxs-lookup"><span data-stu-id="fc763-131">keepEnrollmentData</span></span>|<span data-ttu-id="fc763-132">ブール値</span><span class="sxs-lookup"><span data-stu-id="fc763-132">Boolean</span></span>|<span data-ttu-id="fc763-133">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="fc763-133">Not yet documented</span></span>|
|<span data-ttu-id="fc763-134">keepUserData</span><span class="sxs-lookup"><span data-stu-id="fc763-134">keepUserData</span></span>|<span data-ttu-id="fc763-135">Boolean</span><span class="sxs-lookup"><span data-stu-id="fc763-135">Boolean</span></span>|<span data-ttu-id="fc763-136">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="fc763-136">Not yet documented</span></span>|
|<span data-ttu-id="fc763-137">macOsUnlockCode</span><span class="sxs-lookup"><span data-stu-id="fc763-137">macOsUnlockCode</span></span>|<span data-ttu-id="fc763-138">文字列</span><span class="sxs-lookup"><span data-stu-id="fc763-138">String</span></span>|<span data-ttu-id="fc763-139">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="fc763-139">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="fc763-140">応答</span><span class="sxs-lookup"><span data-stu-id="fc763-140">Response</span></span>
<span data-ttu-id="fc763-141">成功した場合、このアクションは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="fc763-141">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="fc763-142">例</span><span class="sxs-lookup"><span data-stu-id="fc763-142">Example</span></span>
### <a name="request"></a><span data-ttu-id="fc763-143">要求</span><span class="sxs-lookup"><span data-stu-id="fc763-143">Request</span></span>
<span data-ttu-id="fc763-144">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="fc763-144">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}/wipe

Content-type: application/json
Content-length: 109

{
  "keepEnrollmentData": true,
  "keepUserData": true,
  "macOsUnlockCode": "Mac Os Unlock Code value"
}
```

### <a name="response"></a><span data-ttu-id="fc763-145">応答</span><span class="sxs-lookup"><span data-stu-id="fc763-145">Response</span></span>
<span data-ttu-id="fc763-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="fc763-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



