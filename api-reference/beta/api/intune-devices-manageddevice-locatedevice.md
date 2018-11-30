---
title: locateDevice アクション
description: デバイスを検索する
ms.openlocfilehash: 8e92e236ff52a00ee9a5390b062f6c48917a2e24
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27070351"
---
# <a name="locatedevice-action"></a><span data-ttu-id="c81ab-103">locateDevice アクション</span><span class="sxs-lookup"><span data-stu-id="c81ab-103">locateDevice action</span></span>

> <span data-ttu-id="c81ab-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c81ab-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c81ab-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c81ab-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c81ab-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="c81ab-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c81ab-107">デバイスを検索する</span><span class="sxs-lookup"><span data-stu-id="c81ab-107">Locate a device</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c81ab-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="c81ab-108">Prerequisites</span></span>
<span data-ttu-id="c81ab-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c81ab-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c81ab-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="c81ab-111">Permission type</span></span>|<span data-ttu-id="c81ab-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="c81ab-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c81ab-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="c81ab-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c81ab-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="c81ab-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="c81ab-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="c81ab-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c81ab-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c81ab-116">Not supported.</span></span>|
|<span data-ttu-id="c81ab-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="c81ab-117">Application</span></span>|<span data-ttu-id="c81ab-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="c81ab-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c81ab-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="c81ab-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/locateDevice
POST /deviceManagement/managedDevices/{managedDeviceId}/locateDevice
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/locateDevice
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/locateDevice
```

## <a name="request-headers"></a><span data-ttu-id="c81ab-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c81ab-120">Request headers</span></span>
|<span data-ttu-id="c81ab-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c81ab-121">Header</span></span>|<span data-ttu-id="c81ab-122">値</span><span class="sxs-lookup"><span data-stu-id="c81ab-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c81ab-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c81ab-123">Authorization</span></span>|<span data-ttu-id="c81ab-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="c81ab-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c81ab-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c81ab-125">Accept</span></span>|<span data-ttu-id="c81ab-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c81ab-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c81ab-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="c81ab-127">Request body</span></span>
<span data-ttu-id="c81ab-128">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="c81ab-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c81ab-129">応答</span><span class="sxs-lookup"><span data-stu-id="c81ab-129">Response</span></span>
<span data-ttu-id="c81ab-130">成功した場合、このアクションは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="c81ab-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c81ab-131">例</span><span class="sxs-lookup"><span data-stu-id="c81ab-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="c81ab-132">要求</span><span class="sxs-lookup"><span data-stu-id="c81ab-132">Request</span></span>
<span data-ttu-id="c81ab-133">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="c81ab-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/managedDevices/{managedDeviceId}/locateDevice
```

### <a name="response"></a><span data-ttu-id="c81ab-134">応答</span><span class="sxs-lookup"><span data-stu-id="c81ab-134">Response</span></span>
<span data-ttu-id="c81ab-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="c81ab-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





