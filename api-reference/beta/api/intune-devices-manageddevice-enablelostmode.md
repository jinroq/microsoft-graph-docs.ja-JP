---
title: enableLostMode アクション
description: 削除モードを有効にする
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 22f75fb0c9dd4405717584de77b06a89eaf33bb8
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34958481"
---
# <a name="enablelostmode-action"></a><span data-ttu-id="ecaef-103">enableLostMode アクション</span><span class="sxs-lookup"><span data-stu-id="ecaef-103">enableLostMode action</span></span>

> <span data-ttu-id="ecaef-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ecaef-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ecaef-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ecaef-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ecaef-106">削除モードを有効にする</span><span class="sxs-lookup"><span data-stu-id="ecaef-106">Enable lost mode</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ecaef-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="ecaef-107">Prerequisites</span></span>
<span data-ttu-id="ecaef-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ecaef-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ecaef-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ecaef-110">Permission type</span></span>|<span data-ttu-id="ecaef-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ecaef-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ecaef-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ecaef-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ecaef-113">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="ecaef-113">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="ecaef-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ecaef-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ecaef-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ecaef-115">Not supported.</span></span>|
|<span data-ttu-id="ecaef-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ecaef-116">Application</span></span>|<span data-ttu-id="ecaef-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ecaef-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ecaef-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ecaef-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/enableLostMode
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/enableLostMode
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/enableLostMode
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/enableLostMode
```

## <a name="request-headers"></a><span data-ttu-id="ecaef-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ecaef-119">Request headers</span></span>
|<span data-ttu-id="ecaef-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ecaef-120">Header</span></span>|<span data-ttu-id="ecaef-121">値</span><span class="sxs-lookup"><span data-stu-id="ecaef-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ecaef-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ecaef-122">Authorization</span></span>|<span data-ttu-id="ecaef-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="ecaef-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ecaef-124">承諾</span><span class="sxs-lookup"><span data-stu-id="ecaef-124">Accept</span></span>|<span data-ttu-id="ecaef-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ecaef-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ecaef-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="ecaef-126">Request body</span></span>
<span data-ttu-id="ecaef-127">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="ecaef-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="ecaef-128">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="ecaef-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="ecaef-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ecaef-129">Property</span></span>|<span data-ttu-id="ecaef-130">型</span><span class="sxs-lookup"><span data-stu-id="ecaef-130">Type</span></span>|<span data-ttu-id="ecaef-131">説明</span><span class="sxs-lookup"><span data-stu-id="ecaef-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ecaef-132">メッセージ​​</span><span class="sxs-lookup"><span data-stu-id="ecaef-132">message</span></span>|<span data-ttu-id="ecaef-133">String</span><span class="sxs-lookup"><span data-stu-id="ecaef-133">String</span></span>|<span data-ttu-id="ecaef-134">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="ecaef-134">Not yet documented</span></span>|
|<span data-ttu-id="ecaef-135">phoneNumber</span><span class="sxs-lookup"><span data-stu-id="ecaef-135">phoneNumber</span></span>|<span data-ttu-id="ecaef-136">String</span><span class="sxs-lookup"><span data-stu-id="ecaef-136">String</span></span>|<span data-ttu-id="ecaef-137">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="ecaef-137">Not yet documented</span></span>|
|<span data-ttu-id="ecaef-138">フッター</span><span class="sxs-lookup"><span data-stu-id="ecaef-138">footer</span></span>|<span data-ttu-id="ecaef-139">String</span><span class="sxs-lookup"><span data-stu-id="ecaef-139">String</span></span>|<span data-ttu-id="ecaef-140">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="ecaef-140">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="ecaef-141">応答</span><span class="sxs-lookup"><span data-stu-id="ecaef-141">Response</span></span>
<span data-ttu-id="ecaef-142">成功した場合、このアクションは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="ecaef-142">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ecaef-143">例</span><span class="sxs-lookup"><span data-stu-id="ecaef-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="ecaef-144">要求</span><span class="sxs-lookup"><span data-stu-id="ecaef-144">Request</span></span>
<span data-ttu-id="ecaef-145">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ecaef-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/enableLostMode

Content-type: application/json
Content-length: 103

{
  "message": "Message value",
  "phoneNumber": "Phone Number value",
  "footer": "Footer value"
}
```

### <a name="response"></a><span data-ttu-id="ecaef-146">応答</span><span class="sxs-lookup"><span data-stu-id="ecaef-146">Response</span></span>
<span data-ttu-id="ecaef-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ecaef-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





