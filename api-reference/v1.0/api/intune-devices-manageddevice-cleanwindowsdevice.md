---
title: cleanWindowsDevice アクション
description: Windows デバイスをクリーンにします
author: tfitzmac
ms.openlocfilehash: 9d19b71f200381c10b7501eadf9007162ff9fff3
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27301765"
---
# <a name="cleanwindowsdevice-action"></a><span data-ttu-id="2886c-103">cleanWindowsDevice アクション</span><span class="sxs-lookup"><span data-stu-id="2886c-103">cleanWindowsDevice action</span></span>

> <span data-ttu-id="2886c-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="2886c-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2886c-105">Windows デバイスをクリーンにします</span><span class="sxs-lookup"><span data-stu-id="2886c-105">Clean Windows device</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2886c-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="2886c-106">Prerequisites</span></span>
<span data-ttu-id="2886c-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2886c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2886c-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="2886c-109">Permission type</span></span>|<span data-ttu-id="2886c-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="2886c-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2886c-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="2886c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2886c-112">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="2886c-112">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="2886c-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="2886c-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2886c-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2886c-114">Not supported.</span></span>|
|<span data-ttu-id="2886c-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="2886c-115">Application</span></span>|<span data-ttu-id="2886c-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2886c-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2886c-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="2886c-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/cleanWindowsDevice
POST /deviceManagement/managedDevices/{managedDeviceId}/cleanWindowsDevice
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/cleanWindowsDevice
```

## <a name="request-headers"></a><span data-ttu-id="2886c-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2886c-118">Request headers</span></span>
|<span data-ttu-id="2886c-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2886c-119">Header</span></span>|<span data-ttu-id="2886c-120">値</span><span class="sxs-lookup"><span data-stu-id="2886c-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2886c-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2886c-121">Authorization</span></span>|<span data-ttu-id="2886c-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="2886c-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2886c-123">Accept</span><span class="sxs-lookup"><span data-stu-id="2886c-123">Accept</span></span>|<span data-ttu-id="2886c-124">application/json</span><span class="sxs-lookup"><span data-stu-id="2886c-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2886c-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="2886c-125">Request body</span></span>
<span data-ttu-id="2886c-126">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="2886c-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="2886c-127">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="2886c-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="2886c-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2886c-128">Property</span></span>|<span data-ttu-id="2886c-129">種類</span><span class="sxs-lookup"><span data-stu-id="2886c-129">Type</span></span>|<span data-ttu-id="2886c-130">説明</span><span class="sxs-lookup"><span data-stu-id="2886c-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2886c-131">keepUserData</span><span class="sxs-lookup"><span data-stu-id="2886c-131">keepUserData</span></span>|<span data-ttu-id="2886c-132">Boolean</span><span class="sxs-lookup"><span data-stu-id="2886c-132">Boolean</span></span>|<span data-ttu-id="2886c-133">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="2886c-133">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="2886c-134">応答</span><span class="sxs-lookup"><span data-stu-id="2886c-134">Response</span></span>
<span data-ttu-id="2886c-135">成功した場合、このアクションは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="2886c-135">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2886c-136">例</span><span class="sxs-lookup"><span data-stu-id="2886c-136">Example</span></span>
### <a name="request"></a><span data-ttu-id="2886c-137">要求</span><span class="sxs-lookup"><span data-stu-id="2886c-137">Request</span></span>
<span data-ttu-id="2886c-138">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="2886c-138">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}/cleanWindowsDevice

Content-type: application/json
Content-length: 28

{
  "keepUserData": true
}
```

### <a name="response"></a><span data-ttu-id="2886c-139">応答</span><span class="sxs-lookup"><span data-stu-id="2886c-139">Response</span></span>
<span data-ttu-id="2886c-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="2886c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```


