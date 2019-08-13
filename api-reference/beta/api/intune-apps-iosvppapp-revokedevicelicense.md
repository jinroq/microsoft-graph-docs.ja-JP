---
title: revokeDeviceLicense アクション
description: 指定したアプリに割り当てられた iOS VPP デバイスライセンスを取り消します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9a3a6323621ae1df5f59cd9525d1f9f73a69a4e7
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36337077"
---
# <a name="revokedevicelicense-action"></a><span data-ttu-id="1e45a-103">revokeDeviceLicense アクション</span><span class="sxs-lookup"><span data-stu-id="1e45a-103">revokeDeviceLicense action</span></span>

> <span data-ttu-id="1e45a-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1e45a-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1e45a-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="1e45a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1e45a-106">指定したアプリに割り当てられた iOS VPP デバイスライセンスを取り消します。</span><span class="sxs-lookup"><span data-stu-id="1e45a-106">Revoke assigned iOS VPP device license for given app.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1e45a-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="1e45a-107">Prerequisites</span></span>
<span data-ttu-id="1e45a-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1e45a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1e45a-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1e45a-110">Permission type</span></span>|<span data-ttu-id="1e45a-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="1e45a-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1e45a-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1e45a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1e45a-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e45a-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1e45a-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1e45a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1e45a-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1e45a-115">Not supported.</span></span>|
|<span data-ttu-id="1e45a-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1e45a-116">Application</span></span>|<span data-ttu-id="1e45a-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e45a-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1e45a-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1e45a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/revokeDeviceLicense
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}/app/revokeDeviceLicense
POST /deviceAppManagement/mobileApps/{mobileAppId}/deviceStatuses/{mobileAppInstallStatusId}/app/revokeDeviceLicense
```

## <a name="request-headers"></a><span data-ttu-id="1e45a-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1e45a-119">Request headers</span></span>
|<span data-ttu-id="1e45a-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1e45a-120">Header</span></span>|<span data-ttu-id="1e45a-121">値</span><span class="sxs-lookup"><span data-stu-id="1e45a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1e45a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1e45a-122">Authorization</span></span>|<span data-ttu-id="1e45a-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="1e45a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1e45a-124">承諾</span><span class="sxs-lookup"><span data-stu-id="1e45a-124">Accept</span></span>|<span data-ttu-id="1e45a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="1e45a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1e45a-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="1e45a-126">Request body</span></span>
<span data-ttu-id="1e45a-127">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="1e45a-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="1e45a-128">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="1e45a-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="1e45a-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1e45a-129">Property</span></span>|<span data-ttu-id="1e45a-130">型</span><span class="sxs-lookup"><span data-stu-id="1e45a-130">Type</span></span>|<span data-ttu-id="1e45a-131">説明</span><span class="sxs-lookup"><span data-stu-id="1e45a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e45a-132">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="1e45a-132">managedDeviceId</span></span>|<span data-ttu-id="1e45a-133">String</span><span class="sxs-lookup"><span data-stu-id="1e45a-133">String</span></span>|<span data-ttu-id="1e45a-134">割り当てられたアプリライセンスのうち、失効されるユーザーの DeviceId</span><span class="sxs-lookup"><span data-stu-id="1e45a-134">DeviceId for whom assigned app license is to be revoked</span></span>|
|<span data-ttu-id="1e45a-135">notifyManagedDevices</span><span class="sxs-lookup"><span data-stu-id="1e45a-135">notifyManagedDevices</span></span>|<span data-ttu-id="1e45a-136">Boolean</span><span class="sxs-lookup"><span data-stu-id="1e45a-136">Boolean</span></span>|<span data-ttu-id="1e45a-137">失効通知をデバイスに送信する必要があるかどうかを示すブール値</span><span class="sxs-lookup"><span data-stu-id="1e45a-137">Boolean that indicates if revoke notification should be sent to device</span></span>|



## <a name="response"></a><span data-ttu-id="1e45a-138">応答</span><span class="sxs-lookup"><span data-stu-id="1e45a-138">Response</span></span>
<span data-ttu-id="1e45a-139">成功した場合、このアクションは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="1e45a-139">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="1e45a-140">例</span><span class="sxs-lookup"><span data-stu-id="1e45a-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="1e45a-141">要求</span><span class="sxs-lookup"><span data-stu-id="1e45a-141">Request</span></span>
<span data-ttu-id="1e45a-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1e45a-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/revokeDeviceLicense

Content-type: application/json
Content-length: 85

{
  "managedDeviceId": "Managed Device Id value",
  "notifyManagedDevices": true
}
```

### <a name="response"></a><span data-ttu-id="1e45a-143">応答</span><span class="sxs-lookup"><span data-stu-id="1e45a-143">Response</span></span>
<span data-ttu-id="1e45a-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1e45a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






