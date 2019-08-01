---
title: windowsDefenderUpdateSignatures アクション
description: まだ文書化されていません
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: dcfca492381f08b38c9803df858a344b8ab12083
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36020893"
---
# <a name="windowsdefenderupdatesignatures-action"></a><span data-ttu-id="a3195-103">windowsDefenderUpdateSignatures アクション</span><span class="sxs-lookup"><span data-stu-id="a3195-103">windowsDefenderUpdateSignatures action</span></span>

> <span data-ttu-id="a3195-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a3195-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a3195-105">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="a3195-105">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a3195-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="a3195-106">Prerequisites</span></span>
<span data-ttu-id="a3195-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a3195-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3195-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a3195-109">Permission type</span></span>|<span data-ttu-id="a3195-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a3195-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a3195-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a3195-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a3195-112">DeviceManagementManagedDevices.PriviligedOperation.All</span><span class="sxs-lookup"><span data-stu-id="a3195-112">DeviceManagementManagedDevices.PriviligedOperation.All</span></span>|
|<span data-ttu-id="a3195-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a3195-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a3195-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a3195-114">Not supported.</span></span>|
|<span data-ttu-id="a3195-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a3195-115">Application</span></span>|<span data-ttu-id="a3195-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a3195-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a3195-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a3195-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /users/{usersId}/managedDevices/{managedDeviceId}/windowsDefenderUpdateSignatures
POST /deviceManagement/managedDevices/{managedDeviceId}/windowsDefenderUpdateSignatures
POST /deviceManagement/detectedApps/{detectedAppId}/managedDevices/{managedDeviceId}/windowsDefenderUpdateSignatures
```

## <a name="request-headers"></a><span data-ttu-id="a3195-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a3195-118">Request headers</span></span>
|<span data-ttu-id="a3195-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a3195-119">Header</span></span>|<span data-ttu-id="a3195-120">値</span><span class="sxs-lookup"><span data-stu-id="a3195-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a3195-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a3195-121">Authorization</span></span>|<span data-ttu-id="a3195-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="a3195-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a3195-123">承諾</span><span class="sxs-lookup"><span data-stu-id="a3195-123">Accept</span></span>|<span data-ttu-id="a3195-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a3195-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a3195-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="a3195-125">Request body</span></span>
<span data-ttu-id="a3195-126">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="a3195-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a3195-127">応答</span><span class="sxs-lookup"><span data-stu-id="a3195-127">Response</span></span>
<span data-ttu-id="a3195-128">成功した場合、このアクションは `204 No Content` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="a3195-128">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="a3195-129">例</span><span class="sxs-lookup"><span data-stu-id="a3195-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="a3195-130">要求</span><span class="sxs-lookup"><span data-stu-id="a3195-130">Request</span></span>
<span data-ttu-id="a3195-131">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a3195-131">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/users/{usersId}/managedDevices/{managedDeviceId}/windowsDefenderUpdateSignatures
```

### <a name="response"></a><span data-ttu-id="a3195-132">応答</span><span class="sxs-lookup"><span data-stu-id="a3195-132">Response</span></span>
<span data-ttu-id="a3195-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a3195-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



