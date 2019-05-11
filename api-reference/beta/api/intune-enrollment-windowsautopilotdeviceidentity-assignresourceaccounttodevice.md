---
title: assignResourceAccountToDevice アクション
description: リソースアカウントを自動操縦デバイスに割り当てます。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ed4f876e0544b7a2e07d616c6f7549cab3bfb386
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33908238"
---
# <a name="assignresourceaccounttodevice-action"></a><span data-ttu-id="43850-103">assignResourceAccountToDevice アクション</span><span class="sxs-lookup"><span data-stu-id="43850-103">assignResourceAccountToDevice action</span></span>

> <span data-ttu-id="43850-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="43850-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="43850-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="43850-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="43850-106">リソースアカウントを自動操縦デバイスに割り当てます。</span><span class="sxs-lookup"><span data-stu-id="43850-106">Assigns resource account to Autopilot devices.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="43850-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="43850-107">Prerequisites</span></span>
<span data-ttu-id="43850-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="43850-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="43850-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="43850-110">Permission type</span></span>|<span data-ttu-id="43850-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="43850-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="43850-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="43850-112">Delegated (work or school account)</span></span>|<span data-ttu-id="43850-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43850-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="43850-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="43850-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="43850-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="43850-115">Not supported.</span></span>|
|<span data-ttu-id="43850-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="43850-116">Application</span></span>|<span data-ttu-id="43850-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="43850-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="43850-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="43850-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/assignResourceAccountToDevice
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices/{windowsAutopilotDeviceIdentityId}/assignResourceAccountToDevice
```

## <a name="request-headers"></a><span data-ttu-id="43850-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="43850-119">Request headers</span></span>
|<span data-ttu-id="43850-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="43850-120">Header</span></span>|<span data-ttu-id="43850-121">値</span><span class="sxs-lookup"><span data-stu-id="43850-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="43850-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="43850-122">Authorization</span></span>|<span data-ttu-id="43850-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="43850-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="43850-124">承諾</span><span class="sxs-lookup"><span data-stu-id="43850-124">Accept</span></span>|<span data-ttu-id="43850-125">application/json</span><span class="sxs-lookup"><span data-stu-id="43850-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="43850-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="43850-126">Request body</span></span>
<span data-ttu-id="43850-127">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="43850-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="43850-128">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="43850-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="43850-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="43850-129">Property</span></span>|<span data-ttu-id="43850-130">型</span><span class="sxs-lookup"><span data-stu-id="43850-130">Type</span></span>|<span data-ttu-id="43850-131">説明</span><span class="sxs-lookup"><span data-stu-id="43850-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="43850-132">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="43850-132">userPrincipalName</span></span>|<span data-ttu-id="43850-133">String</span><span class="sxs-lookup"><span data-stu-id="43850-133">String</span></span>|<span data-ttu-id="43850-134">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="43850-134">Not yet documented</span></span>|
|<span data-ttu-id="43850-135">addressableUserName</span><span class="sxs-lookup"><span data-stu-id="43850-135">addressableUserName</span></span>|<span data-ttu-id="43850-136">String</span><span class="sxs-lookup"><span data-stu-id="43850-136">String</span></span>|<span data-ttu-id="43850-137">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="43850-137">Not yet documented</span></span>|
|<span data-ttu-id="43850-138">resourceAccountName</span><span class="sxs-lookup"><span data-stu-id="43850-138">resourceAccountName</span></span>|<span data-ttu-id="43850-139">String</span><span class="sxs-lookup"><span data-stu-id="43850-139">String</span></span>|<span data-ttu-id="43850-140">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="43850-140">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="43850-141">応答</span><span class="sxs-lookup"><span data-stu-id="43850-141">Response</span></span>
<span data-ttu-id="43850-142">成功した場合、このアクションは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="43850-142">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="43850-143">例</span><span class="sxs-lookup"><span data-stu-id="43850-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="43850-144">要求</span><span class="sxs-lookup"><span data-stu-id="43850-144">Request</span></span>
<span data-ttu-id="43850-145">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="43850-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/assignResourceAccountToDevice

Content-type: application/json
Content-length: 170

{
  "userPrincipalName": "User Principal Name value",
  "addressableUserName": "Addressable User Name value",
  "resourceAccountName": "Resource Account Name value"
}
```

### <a name="response"></a><span data-ttu-id="43850-146">応答</span><span class="sxs-lookup"><span data-stu-id="43850-146">Response</span></span>
<span data-ttu-id="43850-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="43850-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




