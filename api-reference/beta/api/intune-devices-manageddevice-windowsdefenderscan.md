---
title: windowsDefenderScan アクション
description: まだ文書化されていません
author: tfitzmac
ms.openlocfilehash: d64ce1e595717d99608547ff4622d35d22d18552
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27305090"
---
# <a name="windowsdefenderscan-action"></a><span data-ttu-id="4e002-103">windowsDefenderScan アクション</span><span class="sxs-lookup"><span data-stu-id="4e002-103">windowsDefenderScan action</span></span>

> <span data-ttu-id="4e002-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4e002-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4e002-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4e002-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="4e002-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="4e002-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="4e002-107">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="4e002-107">Not yet documented</span></span>
## <a name="prerequisites"></a><span data-ttu-id="4e002-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="4e002-108">Prerequisites</span></span>
<span data-ttu-id="4e002-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4e002-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4e002-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4e002-111">Permission type</span></span>|<span data-ttu-id="4e002-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="4e002-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4e002-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4e002-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4e002-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="4e002-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="4e002-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4e002-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4e002-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4e002-116">Not supported.</span></span>|
|<span data-ttu-id="4e002-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4e002-117">Application</span></span>|<span data-ttu-id="4e002-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4e002-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4e002-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4e002-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/windowsDefenderScan
POST /deviceManagement/managedDevices/{managedDeviceId}/windowsDefenderScan
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/windowsDefenderScan
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/windowsDefenderScan
```

## <a name="request-headers"></a><span data-ttu-id="4e002-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4e002-120">Request headers</span></span>
|<span data-ttu-id="4e002-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4e002-121">Header</span></span>|<span data-ttu-id="4e002-122">値</span><span class="sxs-lookup"><span data-stu-id="4e002-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4e002-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4e002-123">Authorization</span></span>|<span data-ttu-id="4e002-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="4e002-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4e002-125">Accept</span><span class="sxs-lookup"><span data-stu-id="4e002-125">Accept</span></span>|<span data-ttu-id="4e002-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4e002-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4e002-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="4e002-127">Request body</span></span>
<span data-ttu-id="4e002-128">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="4e002-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="4e002-129">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="4e002-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="4e002-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4e002-130">Property</span></span>|<span data-ttu-id="4e002-131">種類</span><span class="sxs-lookup"><span data-stu-id="4e002-131">Type</span></span>|<span data-ttu-id="4e002-132">説明</span><span class="sxs-lookup"><span data-stu-id="4e002-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4e002-133">quickScan</span><span class="sxs-lookup"><span data-stu-id="4e002-133">quickScan</span></span>|<span data-ttu-id="4e002-134">Boolean</span><span class="sxs-lookup"><span data-stu-id="4e002-134">Boolean</span></span>|<span data-ttu-id="4e002-135">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="4e002-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="4e002-136">応答</span><span class="sxs-lookup"><span data-stu-id="4e002-136">Response</span></span>
<span data-ttu-id="4e002-137">成功した場合、このアクションは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="4e002-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="4e002-138">例</span><span class="sxs-lookup"><span data-stu-id="4e002-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="4e002-139">要求</span><span class="sxs-lookup"><span data-stu-id="4e002-139">Request</span></span>
<span data-ttu-id="4e002-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4e002-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/managedDevices/{managedDeviceId}/windowsDefenderScan

Content-type: application/json
Content-length: 25

{
  "quickScan": true
}
```

### <a name="response"></a><span data-ttu-id="4e002-141">応答</span><span class="sxs-lookup"><span data-stu-id="4e002-141">Response</span></span>
<span data-ttu-id="4e002-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4e002-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





