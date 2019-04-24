---
title: disableLostMode アクション
description: 紛失モードの無効化
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a377869d236f06921bd2a3d7fe5d5dea8659c81a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32584832"
---
# <a name="disablelostmode-action"></a><span data-ttu-id="6291e-103">disableLostMode アクション</span><span class="sxs-lookup"><span data-stu-id="6291e-103">disableLostMode action</span></span>

> <span data-ttu-id="6291e-104">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="6291e-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6291e-105">紛失モードの無効化</span><span class="sxs-lookup"><span data-stu-id="6291e-105">Disable lost mode</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6291e-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="6291e-106">Prerequisites</span></span>
<span data-ttu-id="6291e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="6291e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6291e-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="6291e-109">Permission type</span></span>|<span data-ttu-id="6291e-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="6291e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6291e-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="6291e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6291e-112">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="6291e-112">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="6291e-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="6291e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6291e-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6291e-114">Not supported.</span></span>|
|<span data-ttu-id="6291e-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="6291e-115">Application</span></span>|<span data-ttu-id="6291e-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6291e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6291e-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="6291e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/disableLostMode
POST /deviceManagement/managedDevices/{managedDeviceId}/disableLostMode
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/disableLostMode
```

## <a name="request-headers"></a><span data-ttu-id="6291e-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6291e-118">Request headers</span></span>
|<span data-ttu-id="6291e-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="6291e-119">Header</span></span>|<span data-ttu-id="6291e-120">値</span><span class="sxs-lookup"><span data-stu-id="6291e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6291e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6291e-121">Authorization</span></span>|<span data-ttu-id="6291e-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="6291e-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6291e-123">承諾</span><span class="sxs-lookup"><span data-stu-id="6291e-123">Accept</span></span>|<span data-ttu-id="6291e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="6291e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6291e-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="6291e-125">Request body</span></span>
<span data-ttu-id="6291e-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="6291e-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6291e-127">応答</span><span class="sxs-lookup"><span data-stu-id="6291e-127">Response</span></span>
<span data-ttu-id="6291e-128">成功した場合、このアクションは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="6291e-128">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="6291e-129">例</span><span class="sxs-lookup"><span data-stu-id="6291e-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="6291e-130">要求</span><span class="sxs-lookup"><span data-stu-id="6291e-130">Request</span></span>
<span data-ttu-id="6291e-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="6291e-131">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}/disableLostMode
```

### <a name="response"></a><span data-ttu-id="6291e-132">応答</span><span class="sxs-lookup"><span data-stu-id="6291e-132">Response</span></span>
<span data-ttu-id="6291e-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="6291e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



