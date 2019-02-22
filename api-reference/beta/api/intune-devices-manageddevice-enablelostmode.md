---
title: enableLostMode アクション
description: 削除モードを有効にする
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c3e72cd3620407dc44f2dbd7d3516ded2b641633
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30168622"
---
# <a name="enablelostmode-action"></a><span data-ttu-id="81f28-103">enableLostMode アクション</span><span class="sxs-lookup"><span data-stu-id="81f28-103">enableLostMode action</span></span>

> <span data-ttu-id="81f28-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="81f28-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="81f28-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="81f28-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="81f28-106">削除モードを有効にする</span><span class="sxs-lookup"><span data-stu-id="81f28-106">Enable lost mode</span></span>

## <a name="prerequisites"></a><span data-ttu-id="81f28-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="81f28-107">Prerequisites</span></span>
<span data-ttu-id="81f28-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="81f28-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="81f28-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="81f28-110">Permission type</span></span>|<span data-ttu-id="81f28-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="81f28-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="81f28-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="81f28-112">Delegated (work or school account)</span></span>|<span data-ttu-id="81f28-113">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="81f28-113">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="81f28-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="81f28-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="81f28-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="81f28-115">Not supported.</span></span>|
|<span data-ttu-id="81f28-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="81f28-116">Application</span></span>|<span data-ttu-id="81f28-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="81f28-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="81f28-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="81f28-118">HTTP Request</span></span>
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

## <a name="request-headers"></a><span data-ttu-id="81f28-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="81f28-119">Request headers</span></span>
|<span data-ttu-id="81f28-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="81f28-120">Header</span></span>|<span data-ttu-id="81f28-121">値</span><span class="sxs-lookup"><span data-stu-id="81f28-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="81f28-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="81f28-122">Authorization</span></span>|<span data-ttu-id="81f28-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="81f28-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="81f28-124">承諾</span><span class="sxs-lookup"><span data-stu-id="81f28-124">Accept</span></span>|<span data-ttu-id="81f28-125">application/json</span><span class="sxs-lookup"><span data-stu-id="81f28-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="81f28-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="81f28-126">Request body</span></span>
<span data-ttu-id="81f28-127">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="81f28-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="81f28-128">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="81f28-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="81f28-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="81f28-129">Property</span></span>|<span data-ttu-id="81f28-130">型</span><span class="sxs-lookup"><span data-stu-id="81f28-130">Type</span></span>|<span data-ttu-id="81f28-131">説明</span><span class="sxs-lookup"><span data-stu-id="81f28-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="81f28-132">message</span><span class="sxs-lookup"><span data-stu-id="81f28-132">message</span></span>|<span data-ttu-id="81f28-133">文字列</span><span class="sxs-lookup"><span data-stu-id="81f28-133">String</span></span>|<span data-ttu-id="81f28-134">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="81f28-134">Not yet documented</span></span>|
|<span data-ttu-id="81f28-135">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="81f28-135">phoneNumber</span></span>|<span data-ttu-id="81f28-136">String</span><span class="sxs-lookup"><span data-stu-id="81f28-136">String</span></span>|<span data-ttu-id="81f28-137">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="81f28-137">Not yet documented</span></span>|
|<span data-ttu-id="81f28-138">フッター</span><span class="sxs-lookup"><span data-stu-id="81f28-138">footer</span></span>|<span data-ttu-id="81f28-139">String</span><span class="sxs-lookup"><span data-stu-id="81f28-139">String</span></span>|<span data-ttu-id="81f28-140">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="81f28-140">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="81f28-141">応答</span><span class="sxs-lookup"><span data-stu-id="81f28-141">Response</span></span>
<span data-ttu-id="81f28-142">成功した場合、このアクションは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="81f28-142">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="81f28-143">例</span><span class="sxs-lookup"><span data-stu-id="81f28-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="81f28-144">要求</span><span class="sxs-lookup"><span data-stu-id="81f28-144">Request</span></span>
<span data-ttu-id="81f28-145">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="81f28-145">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="81f28-146">応答</span><span class="sxs-lookup"><span data-stu-id="81f28-146">Response</span></span>
<span data-ttu-id="81f28-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="81f28-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




