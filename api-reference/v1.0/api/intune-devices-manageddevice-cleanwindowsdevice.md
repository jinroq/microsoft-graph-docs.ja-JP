---
title: cleanWindowsDevice アクション
description: Windows デバイスをクリーンにします
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: badddae1181f76f919958fc66a186f51a89c2f30
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35996953"
---
# <a name="cleanwindowsdevice-action"></a><span data-ttu-id="ca9ff-103">cleanWindowsDevice アクション</span><span class="sxs-lookup"><span data-stu-id="ca9ff-103">cleanWindowsDevice action</span></span>

> <span data-ttu-id="ca9ff-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ca9ff-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ca9ff-105">Windows デバイスをクリーンにします</span><span class="sxs-lookup"><span data-stu-id="ca9ff-105">Clean Windows device</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ca9ff-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="ca9ff-106">Prerequisites</span></span>
<span data-ttu-id="ca9ff-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ca9ff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ca9ff-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ca9ff-109">Permission type</span></span>|<span data-ttu-id="ca9ff-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ca9ff-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ca9ff-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ca9ff-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ca9ff-112">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="ca9ff-112">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="ca9ff-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ca9ff-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ca9ff-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ca9ff-114">Not supported.</span></span>|
|<span data-ttu-id="ca9ff-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ca9ff-115">Application</span></span>|<span data-ttu-id="ca9ff-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ca9ff-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ca9ff-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ca9ff-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/cleanWindowsDevice
POST /deviceManagement/managedDevices/{managedDeviceId}/cleanWindowsDevice
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/cleanWindowsDevice
```

## <a name="request-headers"></a><span data-ttu-id="ca9ff-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ca9ff-118">Request headers</span></span>
|<span data-ttu-id="ca9ff-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ca9ff-119">Header</span></span>|<span data-ttu-id="ca9ff-120">値</span><span class="sxs-lookup"><span data-stu-id="ca9ff-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ca9ff-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ca9ff-121">Authorization</span></span>|<span data-ttu-id="ca9ff-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="ca9ff-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ca9ff-123">承諾</span><span class="sxs-lookup"><span data-stu-id="ca9ff-123">Accept</span></span>|<span data-ttu-id="ca9ff-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ca9ff-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ca9ff-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="ca9ff-125">Request body</span></span>
<span data-ttu-id="ca9ff-126">要求本文で、パラメーターの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="ca9ff-126">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="ca9ff-127">次の表に、このアクションで使用できるパラメーターを示します。</span><span class="sxs-lookup"><span data-stu-id="ca9ff-127">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="ca9ff-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ca9ff-128">Property</span></span>|<span data-ttu-id="ca9ff-129">型</span><span class="sxs-lookup"><span data-stu-id="ca9ff-129">Type</span></span>|<span data-ttu-id="ca9ff-130">説明</span><span class="sxs-lookup"><span data-stu-id="ca9ff-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca9ff-131">keepUserData</span><span class="sxs-lookup"><span data-stu-id="ca9ff-131">keepUserData</span></span>|<span data-ttu-id="ca9ff-132">ブール値</span><span class="sxs-lookup"><span data-stu-id="ca9ff-132">Boolean</span></span>|<span data-ttu-id="ca9ff-133">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="ca9ff-133">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="ca9ff-134">応答</span><span class="sxs-lookup"><span data-stu-id="ca9ff-134">Response</span></span>
<span data-ttu-id="ca9ff-135">成功した場合、このアクションは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="ca9ff-135">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ca9ff-136">例</span><span class="sxs-lookup"><span data-stu-id="ca9ff-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="ca9ff-137">要求</span><span class="sxs-lookup"><span data-stu-id="ca9ff-137">Request</span></span>
<span data-ttu-id="ca9ff-138">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ca9ff-138">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}/cleanWindowsDevice

Content-type: application/json
Content-length: 28

{
  "keepUserData": true
}
```

### <a name="response"></a><span data-ttu-id="ca9ff-139">応答</span><span class="sxs-lookup"><span data-stu-id="ca9ff-139">Response</span></span>
<span data-ttu-id="ca9ff-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ca9ff-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



