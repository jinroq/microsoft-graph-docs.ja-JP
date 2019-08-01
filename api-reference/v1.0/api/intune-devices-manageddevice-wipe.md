---
title: wipe action
description: デバイスをワイプする
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8d9bf6cfae1182bf9e63317db09843b86ee1a42c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36020879"
---
# <a name="wipe-action"></a><span data-ttu-id="55274-103">ワイプ アクション</span><span class="sxs-lookup"><span data-stu-id="55274-103">wipe action</span></span>

> <span data-ttu-id="55274-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="55274-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="55274-105">デバイスをワイプする</span><span class="sxs-lookup"><span data-stu-id="55274-105">Wipe a device</span></span>

## <a name="prerequisites"></a><span data-ttu-id="55274-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="55274-106">Prerequisites</span></span>
<span data-ttu-id="55274-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="55274-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="55274-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="55274-109">Permission type</span></span>|<span data-ttu-id="55274-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="55274-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="55274-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="55274-111">Delegated (work or school account)</span></span>|<span data-ttu-id="55274-112">Devicemanagementmanageddevices all、DeviceManagementManagedDevices. すべて</span><span class="sxs-lookup"><span data-stu-id="55274-112">DeviceManagementManagedDevices.PriviligedOperation.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="55274-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="55274-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="55274-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="55274-114">Not supported.</span></span>|
|<span data-ttu-id="55274-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="55274-115">Application</span></span>|<span data-ttu-id="55274-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="55274-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="55274-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="55274-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/wipe
POST /deviceManagement/managedDevices/{managedDeviceId}/wipe
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/wipe
```

## <a name="request-headers"></a><span data-ttu-id="55274-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="55274-118">Request headers</span></span>
|<span data-ttu-id="55274-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="55274-119">Header</span></span>|<span data-ttu-id="55274-120">値</span><span class="sxs-lookup"><span data-stu-id="55274-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="55274-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="55274-121">Authorization</span></span>|<span data-ttu-id="55274-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="55274-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="55274-123">承諾</span><span class="sxs-lookup"><span data-stu-id="55274-123">Accept</span></span>|<span data-ttu-id="55274-124">application/json</span><span class="sxs-lookup"><span data-stu-id="55274-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="55274-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="55274-125">Request body</span></span>
<span data-ttu-id="55274-126">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="55274-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="55274-127">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="55274-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="55274-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="55274-128">Property</span></span>|<span data-ttu-id="55274-129">型</span><span class="sxs-lookup"><span data-stu-id="55274-129">Type</span></span>|<span data-ttu-id="55274-130">説明</span><span class="sxs-lookup"><span data-stu-id="55274-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="55274-131">keepEnrollmentData</span><span class="sxs-lookup"><span data-stu-id="55274-131">keepEnrollmentData</span></span>|<span data-ttu-id="55274-132">ブール型 (Boolean)</span><span class="sxs-lookup"><span data-stu-id="55274-132">Boolean</span></span>|<span data-ttu-id="55274-133">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="55274-133">Not yet documented</span></span>|
|<span data-ttu-id="55274-134">keepUserData</span><span class="sxs-lookup"><span data-stu-id="55274-134">keepUserData</span></span>|<span data-ttu-id="55274-135">ブール値</span><span class="sxs-lookup"><span data-stu-id="55274-135">Boolean</span></span>|<span data-ttu-id="55274-136">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="55274-136">Not yet documented</span></span>|
|<span data-ttu-id="55274-137">macOsUnlockCode</span><span class="sxs-lookup"><span data-stu-id="55274-137">macOsUnlockCode</span></span>|<span data-ttu-id="55274-138">文字列</span><span class="sxs-lookup"><span data-stu-id="55274-138">String</span></span>|<span data-ttu-id="55274-139">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="55274-139">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="55274-140">応答</span><span class="sxs-lookup"><span data-stu-id="55274-140">Response</span></span>
<span data-ttu-id="55274-141">成功した場合、このアクションは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="55274-141">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="55274-142">例</span><span class="sxs-lookup"><span data-stu-id="55274-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="55274-143">要求</span><span class="sxs-lookup"><span data-stu-id="55274-143">Request</span></span>
<span data-ttu-id="55274-144">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="55274-144">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}/wipe

Content-type: application/json
Content-length: 109

{
  "keepEnrollmentData": true,
  "keepUserData": true,
  "macOsUnlockCode": "Mac Os Unlock Code value"
}
```

### <a name="response"></a><span data-ttu-id="55274-145">応答</span><span class="sxs-lookup"><span data-stu-id="55274-145">Response</span></span>
<span data-ttu-id="55274-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="55274-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



