---
title: deleteUserFromSharedAppleDevice アクション
description: 共有の Apple デバイスからユーザーを削除する
author: tfitzmac
ms.openlocfilehash: 68b3e9b700e70c9c5d16c97d20edf6471f7d1fbb
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27347986"
---
# <a name="deleteuserfromsharedappledevice-action"></a><span data-ttu-id="fd52a-103">deleteUserFromSharedAppleDevice アクション</span><span class="sxs-lookup"><span data-stu-id="fd52a-103">deleteUserFromSharedAppleDevice action</span></span>

> <span data-ttu-id="fd52a-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="fd52a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fd52a-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fd52a-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fd52a-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="fd52a-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fd52a-107">共有の Apple デバイスからユーザーを削除する</span><span class="sxs-lookup"><span data-stu-id="fd52a-107">Delete user from shared Apple device</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fd52a-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="fd52a-108">Prerequisites</span></span>
<span data-ttu-id="fd52a-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="fd52a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fd52a-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="fd52a-111">Permission type</span></span>|<span data-ttu-id="fd52a-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="fd52a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fd52a-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="fd52a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fd52a-114">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="fd52a-114">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="fd52a-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="fd52a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fd52a-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fd52a-116">Not supported.</span></span>|
|<span data-ttu-id="fd52a-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="fd52a-117">Application</span></span>|<span data-ttu-id="fd52a-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="fd52a-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fd52a-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="fd52a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/deleteUserFromSharedAppleDevice
POST /deviceManagement/managedDevices/{managedDeviceId}/deleteUserFromSharedAppleDevice
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/deleteUserFromSharedAppleDevice
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/deleteUserFromSharedAppleDevice
```

## <a name="request-headers"></a><span data-ttu-id="fd52a-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fd52a-120">Request headers</span></span>
|<span data-ttu-id="fd52a-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="fd52a-121">Header</span></span>|<span data-ttu-id="fd52a-122">値</span><span class="sxs-lookup"><span data-stu-id="fd52a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fd52a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fd52a-123">Authorization</span></span>|<span data-ttu-id="fd52a-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="fd52a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fd52a-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fd52a-125">Accept</span></span>|<span data-ttu-id="fd52a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fd52a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fd52a-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="fd52a-127">Request body</span></span>
<span data-ttu-id="fd52a-128">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="fd52a-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="fd52a-129">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="fd52a-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="fd52a-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="fd52a-130">Property</span></span>|<span data-ttu-id="fd52a-131">種類</span><span class="sxs-lookup"><span data-stu-id="fd52a-131">Type</span></span>|<span data-ttu-id="fd52a-132">説明</span><span class="sxs-lookup"><span data-stu-id="fd52a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fd52a-133">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="fd52a-133">userPrincipalName</span></span>|<span data-ttu-id="fd52a-134">String</span><span class="sxs-lookup"><span data-stu-id="fd52a-134">String</span></span>|<span data-ttu-id="fd52a-135">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="fd52a-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="fd52a-136">応答</span><span class="sxs-lookup"><span data-stu-id="fd52a-136">Response</span></span>
<span data-ttu-id="fd52a-137">成功した場合、このアクションは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="fd52a-137">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="fd52a-138">例</span><span class="sxs-lookup"><span data-stu-id="fd52a-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="fd52a-139">要求</span><span class="sxs-lookup"><span data-stu-id="fd52a-139">Request</span></span>
<span data-ttu-id="fd52a-140">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="fd52a-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/users/{usersId}/managedDevices/{managedDeviceId}/deleteUserFromSharedAppleDevice

Content-type: application/json
Content-length: 56

{
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="fd52a-141">応答</span><span class="sxs-lookup"><span data-stu-id="fd52a-141">Response</span></span>
<span data-ttu-id="fd52a-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="fd52a-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





