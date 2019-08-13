---
title: sendCustomNotificationToCompanyPortal アクション
description: まだ文書化されていません
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 51b776f3ff2633d5b671377e7ef79b4e580fbaae
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36350484"
---
# <a name="sendcustomnotificationtocompanyportal-action"></a><span data-ttu-id="76bcf-103">sendCustomNotificationToCompanyPortal アクション</span><span class="sxs-lookup"><span data-stu-id="76bcf-103">sendCustomNotificationToCompanyPortal action</span></span>

> <span data-ttu-id="76bcf-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="76bcf-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="76bcf-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="76bcf-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="76bcf-106">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="76bcf-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="76bcf-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="76bcf-107">Prerequisites</span></span>
<span data-ttu-id="76bcf-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="76bcf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="76bcf-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="76bcf-110">Permission type</span></span>|<span data-ttu-id="76bcf-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="76bcf-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="76bcf-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="76bcf-112">Delegated (work or school account)</span></span>|<span data-ttu-id="76bcf-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76bcf-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="76bcf-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="76bcf-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="76bcf-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="76bcf-115">Not supported.</span></span>|
|<span data-ttu-id="76bcf-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="76bcf-116">Application</span></span>|<span data-ttu-id="76bcf-117">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="76bcf-117">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="76bcf-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="76bcf-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managedDevices/{managedDeviceId}/sendCustomNotificationToCompanyPortal
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/sendCustomNotificationToCompanyPortal
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/users/{userId}/managedDevices/{managedDeviceId}/sendCustomNotificationToCompanyPortal
POST /deviceManagement/deviceManagementScripts/{deviceManagementScriptId}/deviceRunStates/{deviceManagementScriptDeviceStateId}/managedDevice/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/sendCustomNotificationToCompanyPortal
```

## <a name="request-headers"></a><span data-ttu-id="76bcf-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="76bcf-119">Request headers</span></span>
|<span data-ttu-id="76bcf-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="76bcf-120">Header</span></span>|<span data-ttu-id="76bcf-121">値</span><span class="sxs-lookup"><span data-stu-id="76bcf-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="76bcf-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="76bcf-122">Authorization</span></span>|<span data-ttu-id="76bcf-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="76bcf-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="76bcf-124">承諾</span><span class="sxs-lookup"><span data-stu-id="76bcf-124">Accept</span></span>|<span data-ttu-id="76bcf-125">application/json</span><span class="sxs-lookup"><span data-stu-id="76bcf-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="76bcf-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="76bcf-126">Request body</span></span>
<span data-ttu-id="76bcf-127">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="76bcf-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="76bcf-128">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="76bcf-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="76bcf-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="76bcf-129">Property</span></span>|<span data-ttu-id="76bcf-130">型</span><span class="sxs-lookup"><span data-stu-id="76bcf-130">Type</span></span>|<span data-ttu-id="76bcf-131">説明</span><span class="sxs-lookup"><span data-stu-id="76bcf-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="76bcf-132">notificationTitle</span><span class="sxs-lookup"><span data-stu-id="76bcf-132">notificationTitle</span></span>|<span data-ttu-id="76bcf-133">String</span><span class="sxs-lookup"><span data-stu-id="76bcf-133">String</span></span>|<span data-ttu-id="76bcf-134">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="76bcf-134">Not yet documented</span></span>|
|<span data-ttu-id="76bcf-135">notificationBody</span><span class="sxs-lookup"><span data-stu-id="76bcf-135">notificationBody</span></span>|<span data-ttu-id="76bcf-136">String</span><span class="sxs-lookup"><span data-stu-id="76bcf-136">String</span></span>|<span data-ttu-id="76bcf-137">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="76bcf-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="76bcf-138">応答</span><span class="sxs-lookup"><span data-stu-id="76bcf-138">Response</span></span>
<span data-ttu-id="76bcf-139">成功した場合、このアクションは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="76bcf-139">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="76bcf-140">例</span><span class="sxs-lookup"><span data-stu-id="76bcf-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="76bcf-141">要求</span><span class="sxs-lookup"><span data-stu-id="76bcf-141">Request</span></span>
<span data-ttu-id="76bcf-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="76bcf-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/sendCustomNotificationToCompanyPortal

Content-type: application/json
Content-length: 105

{
  "notificationTitle": "Notification Title value",
  "notificationBody": "Notification Body value"
}
```

### <a name="response"></a><span data-ttu-id="76bcf-143">応答</span><span class="sxs-lookup"><span data-stu-id="76bcf-143">Response</span></span>
<span data-ttu-id="76bcf-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="76bcf-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






