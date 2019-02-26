---
title: assignUserToDevice アクション
description: ユーザーを自動操縦装置に割り当てます。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c996bbd846ad7a93609a7c79e6e5d4b4497a992c
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30141511"
---
# <a name="assignusertodevice-action"></a><span data-ttu-id="258ed-103">assignUserToDevice アクション</span><span class="sxs-lookup"><span data-stu-id="258ed-103">assignUserToDevice action</span></span>

> <span data-ttu-id="258ed-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="258ed-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="258ed-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="258ed-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="258ed-106">ユーザーを自動操縦装置に割り当てます。</span><span class="sxs-lookup"><span data-stu-id="258ed-106">Assigns user to Autopilot devices.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="258ed-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="258ed-107">Prerequisites</span></span>
<span data-ttu-id="258ed-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="258ed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="258ed-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="258ed-110">Permission type</span></span>|<span data-ttu-id="258ed-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="258ed-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="258ed-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="258ed-112">Delegated (work or school account)</span></span>|<span data-ttu-id="258ed-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="258ed-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="258ed-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="258ed-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="258ed-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="258ed-115">Not supported.</span></span>|
|<span data-ttu-id="258ed-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="258ed-116">Application</span></span>|<span data-ttu-id="258ed-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="258ed-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="258ed-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="258ed-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/assignUserToDevice
POST /deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/deploymentProfile/assignedDevices/{windowsAutopilotDeviceIdentityId}/assignUserToDevice
```

## <a name="request-headers"></a><span data-ttu-id="258ed-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="258ed-119">Request headers</span></span>
|<span data-ttu-id="258ed-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="258ed-120">Header</span></span>|<span data-ttu-id="258ed-121">値</span><span class="sxs-lookup"><span data-stu-id="258ed-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="258ed-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="258ed-122">Authorization</span></span>|<span data-ttu-id="258ed-123">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="258ed-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="258ed-124">承諾</span><span class="sxs-lookup"><span data-stu-id="258ed-124">Accept</span></span>|<span data-ttu-id="258ed-125">application/json</span><span class="sxs-lookup"><span data-stu-id="258ed-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="258ed-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="258ed-126">Request body</span></span>
<span data-ttu-id="258ed-127">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="258ed-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="258ed-128">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="258ed-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="258ed-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="258ed-129">Property</span></span>|<span data-ttu-id="258ed-130">型</span><span class="sxs-lookup"><span data-stu-id="258ed-130">Type</span></span>|<span data-ttu-id="258ed-131">説明</span><span class="sxs-lookup"><span data-stu-id="258ed-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="258ed-132">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="258ed-132">userPrincipalName</span></span>|<span data-ttu-id="258ed-133">String</span><span class="sxs-lookup"><span data-stu-id="258ed-133">String</span></span>|<span data-ttu-id="258ed-134">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="258ed-134">Not yet documented</span></span>|
|<span data-ttu-id="258ed-135">addressableusername</span><span class="sxs-lookup"><span data-stu-id="258ed-135">addressableUserName</span></span>|<span data-ttu-id="258ed-136">String</span><span class="sxs-lookup"><span data-stu-id="258ed-136">String</span></span>|<span data-ttu-id="258ed-137">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="258ed-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="258ed-138">応答</span><span class="sxs-lookup"><span data-stu-id="258ed-138">Response</span></span>
<span data-ttu-id="258ed-139">成功した場合、このアクションは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="258ed-139">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="258ed-140">例</span><span class="sxs-lookup"><span data-stu-id="258ed-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="258ed-141">要求</span><span class="sxs-lookup"><span data-stu-id="258ed-141">Request</span></span>
<span data-ttu-id="258ed-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="258ed-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotDeviceIdentities/{windowsAutopilotDeviceIdentityId}/assignUserToDevice

Content-type: application/json
Content-length: 113

{
  "userPrincipalName": "User Principal Name value",
  "addressableUserName": "Addressable User Name value"
}
```

### <a name="response"></a><span data-ttu-id="258ed-143">応答</span><span class="sxs-lookup"><span data-stu-id="258ed-143">Response</span></span>
<span data-ttu-id="258ed-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="258ed-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




